# Propeller Aero (propeller-aero)

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
