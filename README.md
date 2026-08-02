# NextRoll

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
