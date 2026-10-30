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
> **Not from the company, and here with a question?** You are welcome here — we would rather be the
> front line and point you the right way than have a good report go nowhere. What this repository
> can answer is narrow, though, so it is worth knowing who you are actually looking for:
>
> - **A question about how the API works, an account, billing, or a bug in the service** — that is
>   the company's own support, not us. We profile this API; we do not operate it and cannot see
>   your account.
> - **A bug in an open-source project we only catalog** — file it on that project's own repository.
>   This has happened with a real and correct bug report that reached us instead of the people who
>   could fix it, which helped nobody.
> - **Anything about this listing itself** — the description, the tags, the rating, a missing or
>   wrong artifact — is ours. Open an issue here.
> - **Not sure, or something general about API Evangelist or APIs.io** — open an issue on the
>   [APIs.io Inbox](https://github.com/api-search/inbox) and we will route it.
>
> **This repository contains no software, and we will never ask you to download anything.** There is
> no build, release, installer, or binary here — only text and machine-readable API descriptions, so
> there is nothing here that can be "corrupt" or need "repairing". Any issue, comment, or email
> claiming otherwise and offering a download link is not from us and is hostile. Do not follow the
> link; it is a lure. Report it to GitHub and, if you like, tell us at
> [info@apievangelist.com](mailto:info@apievangelist.com) so we can take it down.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

NextRoll, Inc. is a San Francisco-based marketing technology company that operates two brands on a shared machine-learning and identity platform: AdRoll, a cross-channel digital advertising and retargeting platform for ecommerce and D2C marketers, and AdRoll ABM (formerly RollWorks), an account-based marketing platform for B2B demand generation and sales teams. The NextRoll API is the single developer surface behind both brands, served from https://services.adroll.com and split into focused services: a REST CRUD API for organizations, advertisables, campaigns, ad groups, ads, pixels, segments and product feeds; a GraphQL Reporting API that replaces the legacy per-object report endpoints; an Audience API for CRM, custom, composite, lookalike and target-account segments; Prospecting, Geotargeting and User Lists APIs; an ABM Activate/Playbooks API; and a Server-to-Server event API for conversion and engagement events. Developers register applications at developers.nextroll.com and authenticate with OAuth 2.0 or a Personal Access Token plus an application API key. In May 2026 NextRoll launched the AdRoll MCP Server, an OAuth 2.1 protected Model Context Protocol endpoint that exposes AdRoll reporting, draft-first campaign creation and ABM account intelligence to AI assistants and agents.

**Areas:** Company · Advertising · AdTech · Marketing · Account Based Marketing · Retargeting · Audiences · Campaign Management · Analytics · Reporting · MarTech · Agents

## NextRoll on APIs.io

Everything profiled for NextRoll is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/nextroll/](https://apis.io/providers/nextroll/)** — or go straight to one of the APIs or properties below.

### APIs (9)

- [NextRoll CRUD API](https://apis.io/apis/nextroll/nextroll-crud-api/) — The core REST service behind the AdRoll and AdRoll ABM dashboards. Create and manage organizations, advertisables, campaigns, ad groups, ads, pixels, rules,…
- [NextRoll GraphQL Reporting API](https://apis.io/apis/nextroll/nextroll-graphql-reporting-api/) — A single GraphQL endpoint for all AdRoll and AdRoll ABM reporting data — advertisable, campaign, ad group, ad, audience, email and account metrics,…
- [NextRoll Audience API](https://apis.io/apis/nextroll/nextroll-audience-api/) — Create and manage audience segments — CRM (email list), custom (partner user id), composite, impression, user-events, user-attributes and cross-channel…
- [NextRoll Prospecting API](https://apis.io/apis/nextroll/nextroll-prospecting-api/) — Manage AdRoll Prospecting campaigns, ad groups, audiences, flights, geo-targets and advertisable-level prospecting settings, targeting digital profiles…
- [NextRoll User Lists API](https://apis.io/apis/nextroll/nextroll-user-lists-api/) — Retrieve the size of audiences and user lists by ad, ad group, advertisable, segment and audience preview, including exact and CDP+ segment counts.
- [NextRoll Geotargeting API](https://apis.io/apis/nextroll/nextroll-geotargeting-api/) — Search for the geotargeting EIDs used when setting geographic targets on AdRoll and AdRoll ABM campaigns.
- [AdRoll ABM Activate and Playbooks API](https://apis.io/apis/nextroll/adroll-abm-activate-and-playbooks-api/) — The AdRoll ABM (formerly RollWorks) activation surface — create, read and update playbooks, strategies, campaigns and ad groups used to run B2B…
- [NextRoll Server-to-Server (S2S) Event API](https://apis.io/apis/nextroll/nextroll-server-to-server-s2s-event-api/) — Send conversion and engagement events directly from your servers to complement the AdRoll pixel and Mobile Measurement Partner integrations. Accepts batches…
- [AdRoll MCP Server](https://apis.io/apis/nextroll/adroll-mcp-server/) — NextRoll's Model Context Protocol server (open beta, launched May 2026), exposing supported AdRoll and AdRoll ABM data and tools to MCP-compatible AI…

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### AsyncAPI (1)

Event-driven and webhook contracts.

- [Nextroll S2S Events](https://apis.io/asyncapis/nextroll/nextroll-s2s-events/)

#### GraphQL (1)

GraphQL schemas.

- [GraphQL Reporting API Schema](https://apis.io/graphqls/nextroll/nextroll-graphql-reporting-schema/)

#### MCP servers (1)

Model Context Protocol servers that expose the API to agents.

- [adroll](https://apis.io/servers/nextroll/adroll/)

#### Security (4)

Authentication, trust centre, and vulnerability disclosure.

- [Nextroll Authentication](https://apis.io/security/nextroll/nextroll-authentication/)
- [Nextroll Domain Security](https://apis.io/security/nextroll/nextroll-domain-security/)
- [Nextroll Trust Center](https://apis.io/security/nextroll/nextroll-trust-center/)
- [Nextroll Vulnerability Disclosure](https://apis.io/security/nextroll/nextroll-vulnerability-disclosure/)

#### OAuth scopes (1)

The permissions the API asks for.

- [Nextroll Scopes](https://apis.io/scopes/nextroll/nextroll-scopes/)

#### Plans and pricing (1)

Published plans, tiers and prices.

- [Nextroll Plans](https://apis.io/plans/nextroll/nextroll-plans/)

#### Rate limits (1)

Published request limits.

- [Nextroll Rate Limits](https://apis.io/rate-limits/nextroll/nextroll-rate-limits/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://www.nextroll.com/)
- [Documentation](https://apidocs.nextroll.com/)
- [Getting started](https://apidocs.nextroll.com/guides/get-started.html)
- [API reference](https://apidocs.nextroll.com/http-routingtable.html)
- [Pricing](https://www.adroll.com/pricing)
- [Sign up](https://developers.nextroll.com/accounts/create)
- [Support](https://apidocs.nextroll.com/support.html)
- [Blog](https://www.adroll.com/blog)
- [Security](https://security.nextroll.com/)
- [Compliance](https://www.nextroll.com/trust-center)
- [Trust centre](https://security.nextroll.com/)
- [Terms of service](https://www.nextroll.com/terms/api)
- [Privacy policy](https://www.nextroll.com/privacy)
- [GitHub](https://github.com/AdRoll)
- [Status](https://status.adroll.com/)

## API Evangelist rating

**Kin Score 59.7** — strong · rubric 0.25.0 · scored 2026-10-23

| Facet | Score |
|---|---|
| Discoverability | 80.0 |
| Contract quality | 45.3 |
| Contract governance | 18.2 |
| Operational transparency | 57.9 |
| Developer ergonomics | 49.4 |
| Access clarity | 81.6 |

**Agent readiness 52.2** — agent-ready (gated down from agent-native)

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | yes |
| Agentic Access | — |
| Reversibility Documented | — |
| MCP Server | verified |
| Auth Clarity | served (partial credit) |
| Idempotency | — |
| Error Semantics | documented (partial credit) |
| OpenAPI Examples | documented (partial credit) |
| Rate Limit Signal | documented (partial credit) |
| Event Surface Described | yes |
| Agent Skills | derived (partial credit) |
| Well Known Catalog | — |
| Consent Identity | — |
| Agent Card | — |
| Dry Run Mode | — |
| Delegated Identity | served (partial credit) |
| Protected Resource Metadata | verified |
| Dynamic Client Registration | yes |
| Agentic Commerce | — |
| Pagination Ratio | na |
| Operation Distinctiveness | na |

**Regulatory alignment 45.1** — Horizontal (data, software, accessibility, platform)

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/nextroll/](https://apis.io/providers/nextroll/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for NextRoll: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/nextroll/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
