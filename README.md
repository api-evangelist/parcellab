# parcelLab (parcellab)

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
