---
name: Manage an AdRoll ABM Target Account List
description: Create a Target Account List, organise it into tiers, sync accounts in and
  out, and reference it from an audience segment so AdRoll ABM campaigns activate
  against it.
api: NextRoll Audience API
base_url: https://services.adroll.com
operations:
- GET /audience/v1/target_accounts
- POST /audience/v1/target_accounts
- GET /audience/v1/target_accounts/(tal_eid)
- POST /audience/v1/target_accounts/(tal_eid)
- DELETE /audience/v1/target_accounts/(tal_eid)
- GET /audience/v1/target_accounts/(tal_eid)/tiers
- POST /audience/v1/target_accounts/(tal_eid)/tiers
- GET /audience/v1/target_accounts/(tal_eid)/tiers/(ta_tier_eid)/items
- POST /audience/v1/target_accounts/(tal_eid)/tiers/(ta_tier_eid)/items
- PUT /audience/v1/target_accounts/(tal_eid)/tiers/(ta_tier_eid)/items
- POST /audience/v1/target_accounts/(tal_eid)/tiers/(ta_tier_eid)/items/delete
- POST /audience/v1/target_accounts/(tal_eid)/tiers/(ta_tier_eid)/items/filter
- GET /audience/v1/target_accounts/domains
- GET /audience/v1/target_accounts/names
- POST /audience/v1/target_accounts/domain_references
- GET /audience/v1/target_accounts/general_exclusions
- PUT /audience/v1/segments/tal_references
generated: '2026-08-01'
method: generated
source: https://apidocs.nextroll.com/guides/target-account-lists.html
grounding: Every path above appears verbatim in the published NextRoll HTTP routing
  table.
---

# Manage an AdRoll ABM Target Account List

Target Account Lists (TALs) are the AdRoll ABM primitive for cross-channel
orchestration: push a dynamic set of accounts into the platform when they show intent,
and pull the current list out to personalise experiences in other systems.

## Step 1 — find or create the list

```
GET  https://services.adroll.com/audience/v1/target_accounts?apikey=<APIKEY>
POST https://services.adroll.com/audience/v1/target_accounts?apikey=<APIKEY>
```

Keep the returned `tal_eid`.

## Step 2 — tier the list

```
GET  /audience/v1/target_accounts/(tal_eid)/tiers
POST /audience/v1/target_accounts/(tal_eid)/tiers
```

Tiers are how a TAL is segmented for prioritisation (for example Tier 1 named
accounts vs Tier 3 expansion).

## Step 3 — sync accounts into a tier

```
POST /audience/v1/target_accounts/(tal_eid)/tiers/(ta_tier_eid)/items      # add
PUT  /audience/v1/target_accounts/(tal_eid)/tiers/(ta_tier_eid)/items      # replace
POST /audience/v1/target_accounts/(tal_eid)/tiers/(ta_tier_eid)/items/delete
POST /audience/v1/target_accounts/(tal_eid)/tiers/(ta_tier_eid)/items/filter
```

Note the shape: **delete and filter are POSTs**, not DELETE and GET, because they take
a request body. Resolve company domains to AdRoll's account identities first with
`POST /audience/v1/target_accounts/domain_references`, and check
`GET /audience/v1/target_accounts/general_exclusions` so you do not push accounts the
organisation has globally excluded.

## Step 4 — activate

Point an audience segment at the list with
`PUT /audience/v1/segments/tal_references`, then attach that segment to an ad group
(`POST /api/v1/adgroup/add_segments`) or to an AdRoll ABM playbook
(`PUT /activate/api/v2/playbooks`).

## Step 5 — read back

`GET /audience/v1/target_accounts/domains` and
`GET /audience/v1/target_accounts/names` give you the current membership to mirror
into a CRM or personalisation platform.

## Rules

- **No idempotency key.** Prefer `PUT …/items` (replace) over `POST …/items` (add) for
  a recurring sync — replace converges on the same state when re-run, append does not.
- EIDs are opaque and untyped; never infer a `tal_eid` from a `ta_tier_eid`.
- On HTTP 405, read the `Allow` header — the delete/filter-as-POST pattern above is the
  usual cause.
