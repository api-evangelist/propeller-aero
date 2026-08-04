# Propeller Aero (propeller-aero)

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

Propeller Aero is a drone survey and earthworks analytics platform for construction, mining, aggregates, and waste sites. Teams fly a drone, process imagery with Propeller's AeroPoints smart ground control and photogrammetry pipeline, and get accurate 3D site surveys, terrain models, volumes, and progress tracking in the Propeller Platform.

The **Propeller Public API** is a paid, premium feature (bundled into higher tiers such as **Scale**) that gives programmatic, read-oriented access to organizations, sites, workspaces, surveys, downloadable survey files (orthophotos, terrain, point clouds), user-defined shapes and their calculated widgets (volumes, distances, areas), and DirtMate position-monitoring data. It is a REST API over HTTPS at `https://api.propelleraero.com/v1`, authenticated with a Bearer access token (generated under **Settings > Public API** in the Propeller portal) or via **OpenID Connect** (`authorization_code`). The API documentation is public on ReadMe, but exercising the API requires an entitled subscription.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/propeller-aero/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/propeller-aero/refs/heads/main/apis.yml)

## Access Model

- **Public API is paid and plan-gated.** It is a premium feature available on higher Propeller tiers (notably Scale). It is not a free or self-serve API product.
- **Documentation is public.** Endpoint reference and an `llms.txt` index are published on ReadMe ([propelleraero.readme.io](https://propelleraero.readme.io)).
- **Read-oriented.** The documented surface is primarily `GET` (discovery and download) plus a widget `calculate` (`POST`) for measurements. It is designed to pull site/survey data and processed files into GIS tools, shared drives, and downstream systems - not to author survey projects.
- **Authentication.** Bearer access token, or OpenID Connect authorization_code flow (discovery at `https://api.propelleraero.com/auth/oidc/.well-known/openid-configuration`).
- **Endpoint paths are confirmed** from Propeller's public reference / `llms.txt`; the OpenAPI **schemas are modeled** from the public docs (`x-endpointsModeled: true`) and are not a byte-exact contract.

## Tags

- Drone Survey
- Geospatial
- Earthworks
- Construction
- Mining
- Photogrammetry
- Surveying
- Analytics

## Timestamps

- **Created:** 2026-07-04
- **Modified:** 2026-07-04

## APIs

### Propeller Organizations API

List the organizations the authenticated user can access and retrieve details for a single organization. Organizations are the top-level container for sites, workspaces, and surveys.

- **Human URL:** [https://propelleraero.readme.io/reference](https://propelleraero.readme.io/reference)
- **Base URL:** `https://api.propelleraero.com/v1`

### Propeller Sites API

List the sites (survey projects) within an organization and retrieve a single site's details, including a sample-elevation endpoint for the ground elevation at a coordinate on the current surface model.

- **Human URL:** [https://propelleraero.readme.io/reference](https://propelleraero.readme.io/reference)
- **Base URL:** `https://api.propelleraero.com/v1`

### Propeller Surveys API

List the surveys captured for a site, retrieve an individual survey, and list processed survey files available for download - orthophotos, digital terrain models, and point clouds.

- **Human URL:** [https://propelleraero.readme.io/reference](https://propelleraero.readme.io/reference)
- **Base URL:** `https://api.propelleraero.com/v1`

### Propeller Workspaces API

List the workspaces within a site and retrieve a single workspace. Workspaces are the analysis contexts that hold shapes and calculated widgets.

- **Human URL:** [https://propelleraero.readme.io/reference](https://propelleraero.readme.io/reference)
- **Base URL:** `https://api.propelleraero.com/v1`

### Propeller Shapes & Widgets API

List and retrieve user-defined shapes (polygons, lines, points) in a workspace, and calculate a widget against a shape to return volumes (cut/fill), distances, and areas tied to a chosen survey.

- **Human URL:** [https://propelleraero.readme.io/reference](https://propelleraero.readme.io/reference)
- **Base URL:** `https://api.propelleraero.com/v1`

### Propeller Position Monitoring API

List and retrieve DirtMate position-monitoring configurations and their recorded epochs (individual position measurements over time) for tracking ground movement and asset positions between surveys.

- **Human URL:** [https://propelleraero.readme.io/reference](https://propelleraero.readme.io/reference)
- **Base URL:** `https://api.propelleraero.com/v1`

## Common Properties

- [LinkedIn](https://www.linkedin.com/company/propeller-aero)
- [Website](https://www.propelleraero.com/)
- [GitHub Organization](https://github.com/PropellerAero)
- [Documentation](https://propelleraero.readme.io/docs/getting-started)
- [API Reference](https://propelleraero.readme.io/reference)
- [Support](https://help.propelleraero.com/hc/en-us/articles/19383843944599-Using-Propeller-API)
- [Plans](plans/propeller-aero-plans-pricing.yml)
- [Rate Limits](rate-limits/propeller-aero-rate-limits.yml)
- [Fin Ops](finops/propeller-aero-finops.yml)
- [Blog](https://www.propelleraero.com/blog/)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
