---
name: Report campaign performance with the GraphQL Reporting API
description: Retrieve AdRoll and AdRoll ABM performance metrics — impressions, clicks,
  CPC, CPA, conversions — for advertisables, campaigns, ad groups and ads in a single
  GraphQL request, and handle NextRoll's non-standard GraphQL error envelope.
api: NextRoll GraphQL Reporting API
base_url: https://services.adroll.com
operations:
- POST /reporting/api/v1/query
generated: '2026-08-01'
method: generated
source: https://apidocs.nextroll.com/graphql-reporting-api/overview.html
grounding: The single route appears verbatim in the published NextRoll HTTP routing
  table. The query below is the provider's own "Your First Query" example.
---

# Report campaign performance with the GraphQL Reporting API

The GraphQL Reporting API replaces the `/report` endpoints of the CRUD API and the
`/report` and `/metrics` endpoints of the Prospecting API. Use it for all reporting.

## Endpoint

```
POST https://services.adroll.com/reporting/api/v1/query?apikey=<APIKEY>
Authorization: Token <TOKEN>
Content-Type: application/json
```

The body is `{"query": "<GraphQL document>"}`. One endpoint serves every query.

## Step 1 — the baseline query

```graphql
query MyFirstQuery {
  advertisable {
    forUser {
      eid
      name
      campaigns {
        eid
        name
        metrics(start: "2017-06-01", end: "2017-06-30") {
          summary {
            impressions
            clicks
            cpc
            cpa
          }
        }
      }
    }
  }
}
```

`advertisable.forUser` returns everything the token can reach; `advertisable.byEID`
narrows to one advertisable. Browse the full schema at
`graphql/nextroll-graphql-reporting-schema.md` or interactively at
`https://app.adroll.com/reporting/graphiql`.

## Step 2 — batch, do not loop

There is no documented limit on GraphQL query size, and the service fans out to the
backing services in parallel. Ask for every advertisable, campaign and date range you
need in **one** query rather than iterating — that is both faster and cheaper against
the daily request quota.

Exception: AdRoll ABM **account** metrics cap each query at a 30-day date range. For
longer windows, issue several queries stepping the range.

## Step 3 — handle the error envelope before you read data

NextRoll does **not** use standard GraphQL error handling.

```json
{
  "data": { "advertisable": { "has_errors": true, "errors": ["E001"] }, "has_errors": true },
  "errors": [ { "id": "E001", "msg": "HTTP request failed" } ],
  "has_errors": true,
  "request": "req46209",
  "version": "2018.09.11-1"
}
```

1. Check the top-level `has_errors` **first**.
2. If true, resolve each object-level error ID against the top-level `errors` array.
3. `has_errors` propagates up the whole object hierarchy, so a true at the root can
   come from one deeply nested object.
4. When `has_errors` is true, either handle it explicitly or discard the result —
   never render a mix of correct and incomplete data.
5. Log the `request` id; support asks for it.

## Step 4 — know when the numbers are final

Reporting is approximately real-time during the day. A day's figures are typically
available within twelve hours of that day closing, and are **not final until 48 hours
after the start of the current UTC day**. Do not treat same-day numbers as settled.

## Rules

- Every request needs `apikey` in the query string plus a Token or Bearer credential.
- HTTP 401 with `Missing 'apikey' query parameter` means the key, not the token, is
  missing.
- All dates are UTC.
