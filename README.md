# Logik.io

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

Logik.io is a headless, composable, API-first CPQ (Configure, Price, Quote) and product-configuration engine. It powers guided configuration, pricing, and quoting for complex products across Salesforce CPQ/Commerce and any headless front end, and computes Sales, Manufacturing, and Custom Bills of Materials. The platform exposes versioned Runtime APIs (start/update/save configurations, access Sets, retrieve BOMs) and Admin APIs (blueprints, fields, rules, managed data tables, jobs), authenticated with HTTP Bearer Runtime and Admin tokens. Logik.io was acquired by ServiceNow and is now also marketed as ServiceNow CPQ / Logik.ai; the developer surface at api-docs.logik.io and github.com/logikioopensource remains live and independent.

**Areas:** Company · Sales Tech · CPQ · Product Configuration · Bill of Materials · E-Commerce · Salesforce · API-First

## Logik.io on APIs.io

Everything profiled for Logik.io is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/logikio/](https://apis.io/providers/logikio/)** — or go straight to one of the APIs or properties below.

### APIs (11)

- [Logik.io Blueprint > Export API](https://apis.io/apis/logikio/logikio-blueprint-export-api/) — Export Blueprints
- [Logik.io Blueprint > Import API](https://apis.io/apis/logikio/logikio-blueprint-import-api/) — Import Blueprints
- [Logik.io BOM API](https://apis.io/apis/logikio/logikio-bom-api/) — APIs to retrieve BOM information
- [Logik.io Configuration API](https://apis.io/apis/logikio/logikio-configuration-api/) — APIs to operate on Configuration blueprint to generate BOM
- [Logik.io Configuration (V2) API](https://apis.io/apis/logikio/logikio-configuration-v2-api/) — Creating new configurations, reconfiguring existing configurations, making updates to a configuration and saving changes.
- [Logik.io Managed Tables > Export Tables API](https://apis.io/apis/logikio/logikio-managed-tables-export-tables-api/) — Export and Download Tables
- [Logik.io Managed Tables > Import Tables API](https://apis.io/apis/logikio/logikio-managed-tables-import-tables-api/) — Import and Replace Tables
- [Logik.io Managed Tables > Metadata API](https://apis.io/apis/logikio/logikio-managed-tables-metadata-api/) — Working with Table Metadata
- [Logik.io Managed Tables > Table Rows API](https://apis.io/apis/logikio/logikio-managed-tables-table-rows-api/) — Working with individual Table Rows
- [Logik.io Managed Tables > Tables API](https://apis.io/apis/logikio/logikio-managed-tables-tables-api/) — Listing all Tables and working with indiviudal Tables
- [Logik.io Runtime - Bill of Materials API](https://apis.io/apis/logikio/logikio-runtime-bill-of-materials-api/) — Get Bill of Materials (BOM) information for a given configuration UUID.

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### MCP servers (1)

Model Context Protocol servers that expose the API to agents.

- [logikio](https://apis.io/servers/logikio/logikio/)

#### Agentic access (1)

Which operations an agent can call, which act, and which need a human in the loop.

- [Logikio Agentic Access](https://apis.io/agentic-access/logikio/logikio-agentic-access/)

#### Collections (12)

Postman and Open Collection request collections.

- [Logik.io Admin API - Blueprint Import/Export Blueprint > Export API](https://apis.io/collections/logikio/open-logikio-blueprint-export-api/)
- [Logik.io Admin API - Blueprint Import/Export Blueprint > Export Blueprint > Import API](https://apis.io/collections/logikio/open-logikio-blueprint-import-api/)
- [Logik.io Admin API - Blueprint Import/Export Blueprint > Export BOM API](https://apis.io/collections/logikio/open-logikio-bom-api/)
- [Logik.io Admin API - Blueprint Import/Export Blueprint > Export Configuration API](https://apis.io/collections/logikio/open-logikio-configuration-api/)
- [Logik.io Admin API - Blueprint Import/Export Blueprint > Export Configuration (V2) API](https://apis.io/collections/logikio/open-logikio-configuration-v2-api/)
- [Logik.io Admin API - Blueprint Import/Export Blueprint > Export Managed Tables > Export Tables API](https://apis.io/collections/logikio/open-logikio-managed-tables-export-tables-api/)
- [Logik.io Admin API - Blueprint Import/Export Blueprint > Export Managed Tables > Import Tables API](https://apis.io/collections/logikio/open-logikio-managed-tables-import-tables-api/)
- [Logik.io Admin API - Blueprint Import/Export Blueprint > Export Managed Tables > Metadata API](https://apis.io/collections/logikio/open-logikio-managed-tables-metadata-api/)
- [Logik.io Admin API - Blueprint Import/Export Blueprint > Export Managed Tables > Table Rows API](https://apis.io/collections/logikio/open-logikio-managed-tables-table-rows-api/)
- [Logik.io Admin API - Blueprint Import/Export Blueprint > Export Managed Tables > Tables API](https://apis.io/collections/logikio/open-logikio-managed-tables-tables-api/)
- [Logik.io Admin API - Blueprint Import/Export Blueprint > Export Runtime - Bill of Materials API](https://apis.io/collections/logikio/open-logikio-runtime-bill-of-materials-api/)
- [Logik Configurator Runtime APIs](https://apis.io/collections/logikio/postman-logikio-runtime/)

#### Overlays (4)

OpenAPI overlays, including conversational phrasing for each operation.

- [Logikio Admin Blueprint Overlay](https://apis.io/overlays/logikio/logikio-admin-blueprint-overlay/)
- [Logikio Admin Managed Tables Overlay](https://apis.io/overlays/logikio/logikio-admin-managed-tables-overlay/)
- [Logikio Runtime V1 Overlay](https://apis.io/overlays/logikio/logikio-runtime-v1-overlay/)
- [Logikio Runtime V2 Overlay](https://apis.io/overlays/logikio/logikio-runtime-v2-overlay/)

#### Security (2)

Authentication, trust centre, and vulnerability disclosure.

- [Logikio Authentication](https://apis.io/security/logikio/logikio-authentication/)
- [Logikio Domain Security](https://apis.io/security/logikio/logikio-domain-security/)

#### Plans and pricing (1)

Published plans, tiers and prices.

- [Logikio Plans Pricing](https://apis.io/plans/logikio/logikio-plans-pricing/)

#### Rate limits (1)

Published request limits.

- [Logikio Rate Limits](https://apis.io/rate-limits/logikio/logikio-rate-limits/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://www.logik.io)
- [Documentation](https://api-docs.logik.io/)
- [API reference](https://api-docs.logik.io/)
- [Support](https://support.logik.io/)
- [GitHub](https://github.com/logikioopensource)

## API Evangelist rating

**Kin Score 33.5** — thin · rubric 0.24.0 · scored 2026-10-17

| Facet | Score |
|---|---|
| Discoverability | 78.6 |
| Contract quality | 50.3 |
| Contract governance | 18.2 |
| Operational transparency | 2.6 |
| Developer ergonomics | 43.5 |
| Access clarity | 7.9 |

**Agent readiness 29.0** — agent-ready

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | yes |
| Agentic Access | derived (partial credit) |
| Reversibility Documented | — |
| MCP Server | — |
| Auth Clarity | bearer (partial credit) |
| Idempotency | — |
| Error Semantics | verified |
| OpenAPI Examples | partial |
| Rate Limit Signal | documented (partial credit) |
| Event Surface Described | — |
| Agent Skills | derived (partial credit) |
| Well Known Catalog | — |
| Consent Identity | — |
| Agent Card | — |
| Dry Run Mode | — |
| Delegated Identity | — |
| Protected Resource Metadata | — |
| Dynamic Client Registration | — |
| Agentic Commerce | — |

**Regulatory alignment 21.6** — Horizontal (data, software, accessibility, platform)

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/logikio/](https://apis.io/providers/logikio/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for Logik.io: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/logikio/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
