# parcelLab (parcellab)

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

parcelLab is a Munich-headquartered post-purchase experience platform (parcelLab GmbH) used by retailers including IKEA, Hugo Boss, Dyson, Puma, and John Lewis to turn delivery and returns into a branded, revenue-generating part of the customer journey. The platform spans four modules — Convert (pre-checkout delivery promise), Engage (multichannel post-purchase communications), Retain (Returns Portal and returns experience), and Insights (analytics, benchmarking, control tower) — layered with AI agents (WISMO/R, Insights, Fraud & Abuse) and exposed via the parcelLab API v4 Enhanced. Global, EU, and US regional endpoints are available; the same data backs a Model Context Protocol server at agents.parcellab.com/mcp/ for agentic clients.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/parcellab/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/parcellab/refs/heads/main/apis.yml)

## Scope

- **Type:** Index
- **Position:** Producer
- **Access:** 3rd-Party

## Tags

- Post-Purchase
- E-Commerce
- Tracking
- Returns
- Shipping
- Delivery
- Customer Experience
- Logistics
- Communications
- Germany

## Timestamps

- **Created:** 2026-05-25
- **Modified:** 2026-05-25

## APIs

### parcelLab API

parcelLab API v4 Enhanced — the unified REST API for ingesting orders and trackings, retrieving order status, looking up pickup/drop-off locations, predicting delivery dates (Promise), creating and managing return registrations against returns configurations, evaluating campaign targeting, and serving surveys back to customers.

- **Human URL:** [https://docs.parcellab.com/docs/developers/readme](https://docs.parcellab.com/docs/developers/readme)
- **Base URL:** `https://api.parcellab.com`

#### Tags

- Orders
- Tracking
- Returns
- Promise
- Surveys
- Campaigns
- PUDO

#### Properties

- [Documentation](https://docs.parcellab.com/docs/developers/readme)
- [API Reference](https://docs.parcellab.com/docs/developers/getting-started/api-reference)
- [Quickstart](https://docs.parcellab.com/docs/developers/getting-started/quickstart-guide)
- [Authentication](https://docs.parcellab.com/docs/developers/getting-started/authentication)
- [OpenAPI](openapi/parcellab-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/parcellab.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/parcellab.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [JSON Schema](json-schema/parcellab-order-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/parcellab-tracking-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/parcellab-return-registration-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/parcellab-address-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/parcellab-line-item-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/parcellab-promise-prediction-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Structure](json-structure/parcellab-order-structure.json)
- [JSON Structure](json-structure/parcellab-return-registration-structure.json)
- [JSON-LD](json-ld/parcellab-context.jsonld) — [JSON-LD](https://www.w3.org/TR/json-ld11/)
- [Example](examples/parcellab-upsert-order-example.json)
- [Example](examples/parcellab-get-order-info-example.json)
- [Example](examples/parcellab-predict-delivery-example.json)
- [Example](examples/parcellab-create-return-registration-example.json)
- [Example](examples/parcellab-pudo-lookup-example.json)

### parcelLab MCP Server

Hosted Model Context Protocol server exposing the parcelLab order tracking and returns registration workflow to MCP-compatible agents, authenticated via OAuth 2.1 bearer tokens with scopes such as `track:orderinfo` and `returns:registration`.

- **Human URL:** [https://github.com/parcelLab/parcellab-mcp-server](https://github.com/parcelLab/parcellab-mcp-server)
- **Base URL:** `https://agents.parcellab.com/mcp/`

#### Tags

- MCP
- AI
- Agents
- Tracking
- Returns

#### Properties

- [GitHub Repository](https://github.com/parcelLab/parcellab-mcp-server)
- [Documentation](https://github.com/parcelLab/parcellab-mcp-server)
- [Postman Collection](collections/parcellab.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/parcellab.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [Arazzo Workflows](arazzo/) — [Arazzo Specification](https://spec.openapis.org/arazzo/latest.html)
- [Website](https://parcellab.com)
- [Developer Portal](https://docs.parcellab.com/docs/developers/readme)
- [Documentation](https://docs.parcellab.com/docs/readme)
- [Getting Started](https://docs.parcellab.com/docs/onboarding)
- [Authentication](https://docs.parcellab.com/docs/developers/getting-started/authentication)
- [API Reference](https://docs.parcellab.com/docs/developers/getting-started/api-reference)
- [Error Codes](https://docs.parcellab.com/docs/developers/getting-started/error-codes)
- [Sign Up](https://app.parcellab.com/signin)
- [Console](https://app.parcellab.com)
- [Status Page](https://status.parcellab.com)
- [Pricing](https://parcellab.com/contact-us)
- [Blog](https://parcellab.com/blog/)
- [Terms of Service](https://parcellab.com/legal/terms-of-service/)
- [Careers](https://parcellab.com/careers)
- [Support](https://parcellab.com/contact-us)
- [GitHub Organization](https://github.com/parcelLab)
- [LinkedIn](https://www.linkedin.com/company/parcellab)
- [Security Compliance](https://docs.parcellab.com/docs/platform/security-compliance)
- [Single Sign On](https://docs.parcellab.com/docs/platform/security-compliance/single-sign-on)
- [Data Retention Policy](https://docs.parcellab.com/docs/platform/security-compliance/data-retention-policy)
- [SDK](https://github.com/parcelLab/parcelLab-js-plugin)
- [SDK](https://github.com/parcelLab/js-plugin-utils)
- [SDK](https://github.com/parcelLab/regionIdentifier)
- [SDK](https://github.com/parcelLab/parcellab-embedded-ui-snippets)
- [SDK](https://github.com/parcelLab/charts)
- [Agent S D K](https://github.com/parcelLab/parcellab-mcp-server)
- [Plans](plans/parcellab-plans-pricing.yml)
- [Rate Limits](rate-limits/parcellab-rate-limits.yml)
- [Fin Ops](finops/parcellab-finops.yml)
- [Spectral Rules](rules/parcellab-rules.yml)
- [Vocabulary](vocabulary/parcellab-vocabulary.yml)
- [Features](undefined)
- [Use Cases](undefined)
- [Integrations](undefined)
- [Solutions](undefined)
- [Offices](undefined)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
