---
name: Send conversions with the Server-to-Server Event API
description: Capture AdRoll visitor identifiers, then post batches of conversion and
  engagement events straight from your servers to complement the pixel and MMP
  integrations.
api: NextRoll Server-to-Server (S2S) Event API
base_url: https://srv.adroll.com
operations:
- POST https://srv.adroll.com/api?advertisable=<ADVERTISABLE_EID>
- GET /api/v1/advertisable/get_pixel
generated: '2026-08-01'
method: generated
source: https://apidocs.nextroll.com/server-to-server-api/events.html
grounding: The S2S endpoint and event schema are quoted from the provider's own S2S
  reference and events pages; the pixel lookup route appears verbatim in the published
  NextRoll HTTP routing table.
---

# Send conversions with the Server-to-Server Event API

> This API is documented as under active development — "generally stable, it may
> change. Event processing is not yet fully complete." Treat the contract as unstable
> and version your integration defensively.

## Step 0 — get credentials

S2S needs a **Server Access Token (SAT)**, which is not self-service. Ask your NextRoll
account manager; they share it through a one-time 1Password link that expires after
seven days. You also need the Advertisable EID and its pixel EID
(`GET /api/v1/advertisable/get_pixel`).

## Step 1 — capture an identifier at the edge

Every event must carry **at least one** of:

- `adct` — the click token AdRoll appends to your landing-page URL after an ad click.
  If you use a third-party click tracker, make sure `adct` survives to the final
  landing page.
- `first_party_cookie` — read from the pixel with
  `adroll.get_cookie(function (result) { … })`, or generate your own (valid one year)
  using the examples at `https://github.com/AdRoll/server-to-server`.

Add as many of `email`, `email_sha256` (`SHA-256(LOWERCASE(email))`), `email_md5`
(`MD5(LOWERCASE(email))`), `device_id` (IDFA/GAID) and `user_id` as you have — more
identifiers means a higher match rate.

## Step 2 — post the batch

```
POST https://srv.adroll.com/api?advertisable=<ADVERTISABLE_EID>
Content-Type: application/json
```

Body is an **array** of events; keep it to **no more than 100 events per request**.

```json
[{
  "advertisable_eid": "<ADVERTISABLE_EID>",
  "pixel_eid": "<PIXEL_EID>",
  "event_name": "purchase",
  "page_location": "https://example.com/checkout/complete",
  "ip": "203.0.113.10",
  "user_agent": "<USER_AGENT>",
  "conversion_value": 129.99,
  "currency": "USD",
  "timestamp": 1770000000,
  "identifiers": { "adct": "click123", "email_sha256": "<HASH>" },
  "event_attributes": {
    "order_id": "ORD-4471",
    "products": [
      {"product_id": "ABCDEF-12345", "product_group": "womens-fashion",
       "price": "56.78", "quantity": 1, "category": "top-sellers"}
    ]
  }
}]
```

Required on every event: `advertisable_eid`, `pixel_eid`, `event_name`,
`page_location`, `ip`, and at least one identifier.

## Step 3 — use the supported event names

B2C: `pageView`, `homeView`, `productSearch`, `addToCart`, `purchase`.
B2B/ABM: `highValuePage`, `gatedContent`, `demoRequest`, `signupPlan`, `signupTrial`,
`contactSales`, `liveChat`, `formFill`.

These are the same thirteen names the pixel's `adroll.track()` accepts — one vocabulary
across both transports. See `asyncapi/nextroll-s2s-events.yml`.

## Mobile app events

Build a synthetic `page_location` on a domain you control (it does not need to
resolve) and append `device_os`, `device_type`, `package_app_name` and
`package_app_version` as query parameters, so URL audiences can target app behaviour:

```
https://app.example.com?device_os=iOS&device_type=phone&package_app_name=com.example.App&package_app_version=14.1.3
```

## Rules

- **Never send an S2S `pageView` for a page that already has the AdRoll pixel on it.**
  That double-counts traffic.
- `currency` must be a three-letter ISO 4217 code and must match the `price` currency
  in `event_attributes.products`.
- `timestamp` is UTC seconds (decimals allowed for milliseconds); omitted means now.
- **No delivery receipt, no dedup key, no documented retry contract.** Make your sender
  at-most-once for money events, or carry your own `order_id` in
  `event_attributes.order_id` and reconcile downstream.
- `external_data` takes a JSON string for anything else you need to carry.
