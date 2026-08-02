---
name: Authenticate to the NextRoll API and resolve your Advertisable EID
description: Register an application, pick a credential, and make the first call every
  other NextRoll workflow depends on — retrieving the Advertisable EIDs your token can
  reach.
api: NextRoll CRUD API
base_url: https://services.adroll.com
operations:
- GET /api/v1/organization/get
- GET /api/v1/organization/get_advertisables
- GET /api/v1/organization/get_advertisables_paginated
- GET /api/v1/advertisable/get
- GET /api/v1/advertisable/get_pixel
generated: '2026-08-01'
method: generated
source: https://apidocs.nextroll.com/guides/get-started.html
grounding: Every path above appears verbatim in the published NextRoll HTTP routing
  table (https://apidocs.nextroll.com/http-routingtable.html). NextRoll publishes no
  OpenAPI, so routes are cited as method + path, not operationId.
---

# Authenticate to the NextRoll API and resolve your Advertisable EID

## Before you start

1. Create a developer account at `https://developers.nextroll.com/accounts/create`.
2. Create an application at `https://developers.nextroll.com/my-apps/new-app`. Create
   two — one for production, one for testing — so each gets its own OAuth redirect
   URI. There is no sandbox host, so the "testing" application still writes to live
   data. See `sandbox/nextroll-sandbox.yml`.
3. Note the application's consumer key. That key is the `apikey` value.

## Choose a credential

- **Personal Access Token** — for scripts and single-user integrations. Create and
  revoke at `https://app.adroll.com/settings/personal-access-tokens`. Send it as
  `Authorization: Token <TOKEN>`.
- **OAuth 2.0** — for anything acting on behalf of other users. Authorize at
  `https://services.adroll.com/auth/authorize`, exchange at
  `https://services.adroll.com/auth/token`, then send
  `Authorization: Bearer <ACCESS_TOKEN>`.

**Both credentials still require the `apikey` query parameter on every request.** The
`apikey` always goes in the URL query string, never in the body — even for POST, PUT
and PATCH. See `authentication/nextroll-authentication.yml`.

Access tokens expire after 24 hours. Refresh tokens expire after a year *and after a
single use* — store the new refresh token returned with every refresh.

## Step 1 — confirm the credential works

```
GET https://services.adroll.com/api/v1/organization/get?apikey=<APIKEY>
Authorization: Token <TOKEN>
Accept: application/json
```

## Step 2 — list the Advertisables you can reach

```
GET https://services.adroll.com/api/v1/organization/get_advertisables?apikey=<APIKEY>
Authorization: Token <TOKEN>
```

Use `GET /api/v1/organization/get_advertisables_paginated` instead when the
organization is large.

The Advertisable EID returned here is the parameter almost every other NextRoll call
takes. EIDs are opaque alphanumeric strings such as `48F9EA2E5ACAEE24EB766F` and are
**not** type-prefixed — an EID does not tell you what kind of object it addresses, so
carry the type alongside it.

## Step 3 — resolve the pixel for that Advertisable

```
GET https://services.adroll.com/api/v1/advertisable/get_pixel?apikey=<APIKEY>&advertisable=<ADVERTISABLE_EID>
```

You need the pixel EID for any Server-to-Server event work.

## Reading responses

- Success: HTTP 200 with `{"results": …}`.
- Failure: the `errors` array replaces `results`; each entry has `message` plus either
  a numeric `code` (1 INVALID, 2 MISMATCH, 4 NO_DEFAULT, 8 FAIL, 16 NOT_FOUND,
  32 UNSET, 64 INCOMPLETE, 128 EXTERNAL, 256 DUPLICATE, 512 FORBIDDEN) or a `field`
  name. See `errors/nextroll-error-codes.yml`.
- HTTP 405 lists permitted methods in the `Allow` header.

## Rules

- **There is no idempotency key.** No NextRoll write operation is documented as
  retry-safe. Do not blind-retry a create — re-read first with the matching `get`
  route and only then decide. See `conventions/nextroll-conventions.yml`.
- **Rate limits are opaque.** A new application starts at 100 requests per service per
  day; Basic tier is documented at 10,000 calls per day. There are no rate-limit
  response headers — the only signal is HTTP 429. Back off exponentially and request an
  increase through the published form. See `rate-limits/nextroll-rate-limits.yml`.
- **Do not put the access token in the URL.** The OAuth guide permits `access_token` as
  a query parameter; prefer the `Authorization` header so the credential stays out of
  logs and referrers.
- All dates and times are UTC, ISO 8601.
