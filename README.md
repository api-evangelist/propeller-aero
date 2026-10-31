# Propeller Aero

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

Propeller Aero is a drone survey and earthworks analytics platform for construction, mining, aggregates, and waste sites. Teams fly a drone, process imagery with Propeller's AeroPoints ground control and photogrammetry pipeline, and get accurate 3D site surveys, terrain models, volumes, and progress tracking in the Propeller Platform. The Propeller Public API is a paid, premium feature (available on higher tiers such as Scale) that gives programmatic, read-oriented access to organizations, sites, workspaces, surveys, downloadable survey files (orthophotos, terrain, point clouds), user-defined shapes and their calculated widgets (volumes, distances, areas), and DirtMate position-monitoring data. It is a REST API over HTTPS authenticated with a Bearer access token or via OpenID Connect.

**Areas:** Drone Survey · Geospatial · Earthworks · Construction · Mining · Photogrammetry · Surveying · Analytics

## Propeller Aero on APIs.io

Everything profiled for Propeller Aero is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/propeller-aero/](https://apis.io/providers/propeller-aero/)** — or go straight to one of the APIs or properties below.

### APIs (7)

- [Propeller Aero Organizations API](https://apis.io/apis/propeller-aero/propeller-aero-organizations-api/) — Top-level accounts that own sites, workspaces, and surveys.
- [Propeller Aero Position Monitoring API](https://apis.io/apis/propeller-aero/propeller-aero-position-monitoring-api/) — DirtMate position-monitoring configs and recorded epochs.
- [Propeller Aero Shapes API](https://apis.io/apis/propeller-aero/propeller-aero-shapes-api/) — User-defined polygons, lines, and points drawn in a workspace.
- [Propeller Aero Sites API](https://apis.io/apis/propeller-aero/propeller-aero-sites-api/) — Survey projects (job sites) within an organization.
- [Propeller Aero Surveys API](https://apis.io/apis/propeller-aero/propeller-aero-surveys-api/) — Individual drone survey captures and their downloadable files.
- [Propeller Aero Widgets API](https://apis.io/apis/propeller-aero/propeller-aero-widgets-api/) — Calculated measurements (volumes, distances, areas) tied to a shape.
- [Propeller Aero Workspaces API](https://apis.io/apis/propeller-aero/propeller-aero-workspaces-api/) — Analysis contexts within a site that hold shapes and widgets.

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### Agentic access (1)

Which operations an agent can call, which act, and which need a human in the loop.

- [Propeller Aero Agentic Access](https://apis.io/agentic-access/propeller-aero/propeller-aero-agentic-access/)

#### Collections (7)

Postman and Open Collection request collections.

- [Propeller Public Organizations API](https://apis.io/collections/propeller-aero/open-propeller-aero-organizations-api/)
- [Propeller Public Organizations Position Monitoring API](https://apis.io/collections/propeller-aero/open-propeller-aero-position-monitoring-api/)
- [Propeller Public Organizations Shapes API](https://apis.io/collections/propeller-aero/open-propeller-aero-shapes-api/)
- [Propeller Public Organizations Sites API](https://apis.io/collections/propeller-aero/open-propeller-aero-sites-api/)
- [Propeller Public Organizations Surveys API](https://apis.io/collections/propeller-aero/open-propeller-aero-surveys-api/)
- [Propeller Public Organizations Widgets API](https://apis.io/collections/propeller-aero/open-propeller-aero-widgets-api/)
- [Propeller Public Organizations Workspaces API](https://apis.io/collections/propeller-aero/open-propeller-aero-workspaces-api/)

#### Security (3)

Authentication, trust centre, and vulnerability disclosure.

- [Propeller Aero Authentication](https://apis.io/security/propeller-aero/propeller-aero-authentication/)
- [Propeller Aero Domain Security](https://apis.io/security/propeller-aero/propeller-aero-domain-security/)
- [Propeller Aero Trust Center](https://apis.io/security/propeller-aero/propeller-aero-trust-center/)

#### Plans and pricing (1)

Published plans, tiers and prices.

- [Propeller Aero Plans Pricing](https://apis.io/plans/propeller-aero/propeller-aero-plans-pricing/)

#### Rate limits (1)

Published request limits.

- [Propeller Aero Rate Limits](https://apis.io/rate-limits/propeller-aero/propeller-aero-rate-limits/)

#### FinOps (1)

What the API costs to run, by operation.

- [Propeller Aero Finops](https://apis.io/finops/propeller-aero/propeller-aero-finops/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://www.propelleraero.com/)
- [Documentation](https://propelleraero.readme.io/docs/getting-started)
- [API reference](https://propelleraero.readme.io/reference)
- [Support](https://help.propelleraero.com/hc/en-us/articles/19383843944599-Using-Propeller-API)
- [Blog](https://www.propelleraero.com/blog/)
- [GitHub](https://github.com/PropellerAero)

## API Evangelist rating

**Kin Score 27.6** — thin · rubric 0.24.0 · scored 2026-10-17

| Facet | Score |
|---|---|
| Discoverability | 66.1 |
| Contract quality | 47.2 |
| Contract governance | 0.0 |
| Operational transparency | 7.9 |
| Developer ergonomics | 27.4 |
| Access clarity | 15.8 |

**Agent readiness 22.6** — agent-aware

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | yes |
| Agentic Access | derived (partial credit) |
| Reversibility Documented | — |
| MCP Server | — |
| Auth Clarity | bearer (partial credit) |
| Idempotency | — |
| Error Semantics | — |
| OpenAPI Examples | partial |
| Rate Limit Signal | derived (partial credit) |
| Event Surface Described | — |
| Agent Skills | — |
| Well Known Catalog | — |
| Consent Identity | — |
| Agent Card | — |
| Dry Run Mode | — |
| Delegated Identity | documented (partial credit) |
| Protected Resource Metadata | — |
| Dynamic Client Registration | — |
| Agentic Commerce | — |

**Regulatory alignment 16.7** — Horizontal (data, software, accessibility, platform)

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/propeller-aero/](https://apis.io/providers/propeller-aero/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for Propeller Aero: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/propeller-aero/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
