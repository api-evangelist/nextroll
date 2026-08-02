---
name: Create and populate a CRM audience segment
description: Create an AdRoll audience segment from a list of email addresses or
  partner user IDs, add members in bulk, and check the resulting audience size before
  targeting a campaign at it.
api: NextRoll Audience API
base_url: https://services.adroll.com
operations:
- GET /audience/v1/advertisers
- POST /audience/v1/segments
- GET /audience/v1/segments
- GET /audience/v1/segments/(segment_id)
- POST /audience/v1/segments/(segment_id)
- POST /audience/v1/segments/bulk
- POST /audience/v1/segments_bulk/put
- POST /audience/v1/segments/(segment_id)/reactivate
- DELETE /audience/v1/segments/(segment_id)
- GET /user-lists/api/v1/userlists/segment
generated: '2026-08-01'
method: generated
source: https://apidocs.nextroll.com/audience-api/overview.html
grounding: Every path above appears verbatim in the published NextRoll HTTP routing
  table.
---

# Create and populate a CRM audience segment

## Pick the segment type first

The Audience API supports `composite`, `crm`, `custom`, `impression`, `user_events`,
`user_attributes` and `crosschannel_lal`. Anything outside that list has to be created
through the CRUD API instead.

- `crm` — members are **email addresses** (RFC 5322).
- `custom` — members are **partner user IDs** you assign; `duration` sets how many days
  (1–540) a member stays valid.

## Step 1 — resolve the advertisable

Use `GET /api/v1/organization/get_advertisables` (see the authentication skill) or
`GET /audience/v1/advertisers`.

## Step 2 — create the segment

```
POST https://services.adroll.com/audience/v1/segments?apikey=<APIKEY>
Authorization: Token <TOKEN>
```

A created segment returns:

```json
{ "result": "success",
  "segment": { "segment_id": "TESTSEGMENT1234567890X", "type": "crm",
               "name": "TestCRMSegment", "emails": 101 } }
```

Keep `segment_id` — it addresses the segment everywhere else.

## Step 3 — add members

- One segment at a time: `POST /audience/v1/segments/(segment_id)`.
- Many segments in one call: `POST /audience/v1/segments/bulk` or
  `POST /audience/v1/segments_bulk/put`.

A user record is `{"email": "first.last@host.com"}` for `crm`, or
`{"id": "user_identifier_1234"}` for `custom`. Optionally add `"ts"`, a Unix timestamp
marking when the user entered the segment — valid from 540 days in the past to 7 days
in the future. Omitted `ts` means now.

## Step 4 — verify before you target

```
GET https://services.adroll.com/user-lists/api/v1/userlists/segment?apikey=<APIKEY>
```

Also available: `/user-lists/api/v1/userlists/segment/exact`,
`/user-lists/api/v1/userlists/segment/cdp_plus` and
`/user-lists/api/v1/userlists/audience_preview`. Confirm the audience is non-trivial
before attaching it to an ad group with `POST /api/v1/adgroup/add_segments`.

## Rules

- **No idempotency key.** A retried create makes a second segment. If a create times
  out, list with `GET /audience/v1/segments` and match on name before retrying.
- Deletes are `DELETE /audience/v1/segments/(segment_id)`; a deleted segment can be
  brought back with `POST /audience/v1/segments/(segment_id)/reactivate`.
- Handle 400 field errors by reading the `field` name in each `errors[]` entry.
- You are uploading personal data. NextRoll's DPA and privacy terms apply — hash
  emails where your own policy requires it, and confirm you have a lawful basis.
