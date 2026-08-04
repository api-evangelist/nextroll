# NextRoll

<!-- API-EVANGELIST-PROVENANCE:BEGIN -->
> ### About this repository
>
> **This is not our API.** This repository is an independent, third-party profile of a company's
> **publicly available** API surface, maintained by [API Evangelist](https://apievangelist.com).
> API Evangelist does not operate, host, resell, or support this company's APIs, and is not
> affiliated with or endorsed by the company unless stated on the profile.
>
> **Where the information came from.** Everything here is assembled from material a member of the
> public can reach with a browser and no credentials — the company's own website, developer portal
> and documentation, the specifications it publishes for public use (OpenAPI, AsyncAPI, JSON Schema,
> `apis.json`, `llms.txt` and similar), its public repositories, and its public status, pricing and
> changelog pages. **Nothing here is obtained by breaching a system, defeating an access control, or
> using credentials of any kind.**
>
> **The rating is an independent assessment.** The Kin Score and Agent Readiness rating are
> independently calculated scores of a company's *public* API artifacts, produced by API Evangelist
> against a published rubric. They are not certifications, endorsements, security assessments, or
> audits, and they score published artifacts — not the quality, safety, or security of the software.
>
> **Corrections, re-scores, and removal are free.** No partnership, contract, or purchase is
> required, and you do not need to justify the request.
>
> - **Something wrong?** Open an issue on this repository, or email
>   [info@apievangelist.com](mailto:info@apievangelist.com).
> - **Published something new?** Ask for a re-score and we will re-run the rating.
> - **Want the listing taken down?** Say so and we will honor it. The profile is reduced to your
>   company name, a factual description, and a link to your own site, and the company is recorded as
>   **unrated** — never scored zero for having asked.
>
> **Response times.** Acknowledgement within **one business day**; removal or restriction within
> **two business days**; corrections and re-scores within **five business days**.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

NextRoll, Inc. is a San Francisco marketing technology company running two brands on a
shared machine-learning and identity platform — **AdRoll** (cross-channel digital
advertising and retargeting) and **AdRoll ABM**, formerly RollWorks (account-based
marketing for B2B). One developer surface, `https://services.adroll.com`, serves both.

- Company — https://www.nextroll.com/
- Developer portal — https://developers.nextroll.com/
- API documentation — https://apidocs.nextroll.com/
- Path index (192 documented routes) — https://apidocs.nextroll.com/http-routingtable.html
- Status — https://status.adroll.com/
- Trust center — https://security.nextroll.com/

## APIs profiled

| API | Base URL |
|---|---|
| CRUD API | `https://services.adroll.com/api/v1` |
| GraphQL Reporting API | `https://services.adroll.com/reporting/api/v1` |
| Audience API | `https://services.adroll.com/audience/v1` |
| Prospecting API | `https://services.adroll.com/prospecting/api/v2` |
| User Lists API | `https://services.adroll.com/user-lists/api/v1` |
| Geotargeting API | `https://services.adroll.com/geo/api/search/v2` |
| AdRoll ABM Activate / Playbooks API | `https://services.adroll.com/activate/api/v2` |
| Server-to-Server (S2S) Event API | `https://srv.adroll.com/api` |
| AdRoll MCP Server | `https://services.adroll.com/mcp` |

## What this repo holds

Artifacts harvested, probed or derived by the API Evangelist enrichment pipeline:
`authentication/`, `scopes/`, `conventions/`, `errors/`, `lifecycle/`, `conformance/`,
`rate-limits/`, `plans/`, `data-model/`, `components/`, `sandbox/`, `packages/`,
`well-known/`, `security/`, `mcp/`, `graphql/`, `asyncapi/`, `skills/`, `llms/`.

## Notable findings

- **No OpenAPI.** NextRoll publishes no OpenAPI or Swagger document. Probed every
  candidate path on the API host, the docs host and the developer portal — all miss.
  The machine-adjacent contract is a Sphinx `httpdomain` routing table of **192
  documented routes**, plus a full GraphQL schema reference (saved verbatim in
  `graphql/`).
- **A real, modern MCP server.** `https://services.adroll.com/mcp` (open beta since
  2026-05-27) is protected by OAuth 2.1 with S256 PKCE and dynamic client registration,
  and publishes both RFC 8414 authorization-server metadata and RFC 9728
  protected-resource metadata. `tools/list` is auth-gated, so no tool manifest is
  recorded — see `mcp/` for the honest crosswalk.
- **Two OAuth deployments, a decade apart.** The developer API OAuth still offers the
  implicit and resource-owner-password grants and a single `all` scope; the MCP
  deployment is OAuth 2.1 shaped with an `mcp` scope.
- **No idempotency contract, no sandbox, no first-party SDK, no changelog.** All four
  recorded as absent rather than fabricated.
