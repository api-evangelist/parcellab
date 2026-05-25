# parcelLab (parcellab)

parcelLab is a Munich-headquartered post-purchase experience platform
(parcelLab GmbH) used by retailers including IKEA, Hugo Boss, Dyson, Puma,
and John Lewis to turn delivery and returns into a branded,
revenue-generating part of the customer journey. The platform spans four
modules — Convert (pre-checkout delivery promise), Engage (multichannel
post-purchase communications), Retain (Returns Portal and returns
experience), and Insights (analytics, benchmarking, control tower) —
layered with AI agents (WISMO/R, Insights, Fraud & Abuse) and exposed via
the parcelLab API v4 Enhanced.

**URL:** [Visit APIs.json URL](https://raw.githubusercontent.com/api-evangelist/parcellab/refs/heads/main/apis.yml)

## Scope

- **Type:** Index
- **Kind:** contract
- **Position:** Producer
- **Access:** 3rd-Party

## Tags

- Post-Purchase, E-Commerce, Tracking, Returns, Shipping, Delivery, Customer Experience, Logistics, Communications, Germany

## Timestamps

- **Created:** 2026-05-25
- **Modified:** 2026-05-25

## APIs

### parcelLab API

parcelLab API v4 Enhanced — the unified REST API for ingesting orders and
trackings, retrieving order status, looking up pickup/drop-off locations,
predicting delivery dates (Promise), creating and managing return
registrations against returns configurations, evaluating campaign targeting,
and serving surveys back to customers.

- **Human URL:** [docs.parcellab.com/docs/developers/readme](https://docs.parcellab.com/docs/developers/readme)
- **Base URL:** `https://api.parcellab.com` (global) — also `api.eu.parcellab.com`, `api.us.parcellab.com`

#### Tags

- Orders, Tracking, Returns, Promise, Surveys, Campaigns, PUDO

#### Properties

- [Documentation](https://docs.parcellab.com/docs/developers/readme)
- [APIReference](https://docs.parcellab.com/docs/developers/getting-started/api-reference)
- [Quickstart](https://docs.parcellab.com/docs/developers/getting-started/quickstart-guide)
- [Authentication](https://docs.parcellab.com/docs/developers/getting-started/authentication)
- [OpenAPI](openapi/parcellab-openapi.yml)
- [JSON Schema — Order](json-schema/parcellab-order-schema.json)
- [JSON Schema — Tracking](json-schema/parcellab-tracking-schema.json)
- [JSON Schema — Return Registration](json-schema/parcellab-return-registration-schema.json)
- [JSON Schema — Address](json-schema/parcellab-address-schema.json)
- [JSON Schema — Line Item](json-schema/parcellab-line-item-schema.json)
- [JSON Schema — Promise Prediction](json-schema/parcellab-promise-prediction-schema.json)
- [JSON Structure — Order](json-structure/parcellab-order-structure.json)
- [JSON Structure — Return Registration](json-structure/parcellab-return-registration-structure.json)
- [JSON-LD Context](json-ld/parcellab-context.jsonld)

### parcelLab MCP Server

Hosted Model Context Protocol server exposing the parcelLab order tracking
and returns registration workflow to MCP-compatible agents, authenticated
via OAuth 2.1 bearer tokens with scopes such as `track:orderinfo` and
`returns:registration`.

- **Human URL:** [github.com/parcelLab/parcellab-mcp-server](https://github.com/parcelLab/parcellab-mcp-server)
- **Base URL:** `https://agents.parcellab.com/mcp/`

## Capabilities

### Workflow Capability

| Capability | Description |
|---|---|
| [capabilities/post-purchase-experience.yaml](capabilities/post-purchase-experience.yaml) | End-to-end post-purchase composition (Promise → Orders → Events → PUDO → Returns → Surveys → Campaigns). |

### Per-Surface Capabilities

| Capability | Description |
|---|---|
| [parcellab-orders.yaml](capabilities/parcellab-orders.yaml) | Order upsert and order info retrieval. |
| [parcellab-events.yaml](capabilities/parcellab-events.yaml) | Push custom shop/warehouse events into the tracking timeline. |
| [parcellab-promise.yaml](capabilities/parcellab-promise.yaml) | Pre-checkout delivery date prediction. |
| [parcellab-place-info.yaml](capabilities/parcellab-place-info.yaml) | Pickup/drop-off location lookup. |
| [parcellab-returns.yaml](capabilities/parcellab-returns.yaml) | Return registrations, configurations, and document templates. |
| [parcellab-surveys.yaml](capabilities/parcellab-surveys.yaml) | Survey definitions, prefilled answers, and submissions. |
| [parcellab-campaigns.yaml](capabilities/parcellab-campaigns.yaml) | Campaign targeting evaluation and redirect analytics. |

## Artifacts

| Type | File |
|---|---|
| OpenAPI | [openapi/parcellab-openapi.yml](openapi/parcellab-openapi.yml) |
| JSON Schema | [json-schema/parcellab-order-schema.json](json-schema/parcellab-order-schema.json) |
| JSON Schema | [json-schema/parcellab-tracking-schema.json](json-schema/parcellab-tracking-schema.json) |
| JSON Schema | [json-schema/parcellab-return-registration-schema.json](json-schema/parcellab-return-registration-schema.json) |
| JSON Schema | [json-schema/parcellab-address-schema.json](json-schema/parcellab-address-schema.json) |
| JSON Schema | [json-schema/parcellab-line-item-schema.json](json-schema/parcellab-line-item-schema.json) |
| JSON Schema | [json-schema/parcellab-promise-prediction-schema.json](json-schema/parcellab-promise-prediction-schema.json) |
| JSON Structure | [json-structure/parcellab-order-structure.json](json-structure/parcellab-order-structure.json) |
| JSON Structure | [json-structure/parcellab-return-registration-structure.json](json-structure/parcellab-return-registration-structure.json) |
| JSON-LD | [json-ld/parcellab-context.jsonld](json-ld/parcellab-context.jsonld) |
| Examples | [examples/parcellab-upsert-order-example.json](examples/parcellab-upsert-order-example.json) |
| Examples | [examples/parcellab-get-order-info-example.json](examples/parcellab-get-order-info-example.json) |
| Examples | [examples/parcellab-predict-delivery-example.json](examples/parcellab-predict-delivery-example.json) |
| Examples | [examples/parcellab-create-return-registration-example.json](examples/parcellab-create-return-registration-example.json) |
| Examples | [examples/parcellab-pudo-lookup-example.json](examples/parcellab-pudo-lookup-example.json) |
| Spectral Rules | [rules/parcellab-rules.yml](rules/parcellab-rules.yml) |
| Vocabulary | [vocabulary/parcellab-vocabulary.yml](vocabulary/parcellab-vocabulary.yml) |
| Plans | [plans/parcellab-plans-pricing.yml](plans/parcellab-plans-pricing.yml) |
| Rate Limits | [rate-limits/parcellab-rate-limits.yml](rate-limits/parcellab-rate-limits.yml) |
| FinOps | [finops/parcellab-finops.yml](finops/parcellab-finops.yml) |

## Common Properties

- [Website](https://parcellab.com)
- [Developer Portal](https://docs.parcellab.com/docs/developers/readme)
- [Documentation](https://docs.parcellab.com/docs/readme)
- [Getting Started](https://docs.parcellab.com/docs/onboarding)
- [Authentication](https://docs.parcellab.com/docs/developers/getting-started/authentication)
- [API Reference](https://docs.parcellab.com/docs/developers/getting-started/api-reference)
- [Error Codes](https://docs.parcellab.com/docs/developers/getting-started/error-codes)
- [Sign In](https://app.parcellab.com/signin) — Console at [app.parcellab.com](https://app.parcellab.com)
- [Status Page](https://status.parcellab.com)
- [Pricing / Contact Sales](https://parcellab.com/contact-us)
- [Blog](https://parcellab.com/blog/)
- [Terms of Service](https://parcellab.com/legal/terms-of-service/)
- [Careers](https://parcellab.com/careers)
- [Support](https://parcellab.com/contact-us)
- [GitHub](https://github.com/parcelLab) — [LinkedIn](https://www.linkedin.com/company/parcellab)
- Security & Compliance: [overview](https://docs.parcellab.com/docs/platform/security-compliance), [SSO](https://docs.parcellab.com/docs/platform/security-compliance/single-sign-on), [Data Retention](https://docs.parcellab.com/docs/platform/security-compliance/data-retention-policy)

## SDKs and Tooling

| Repo | Purpose |
|---|---|
| [parcelLab-js-plugin](https://github.com/parcelLab/parcelLab-js-plugin) | JavaScript plugin to retrieve and display trackings on any webpage. |
| [js-plugin-utils](https://github.com/parcelLab/js-plugin-utils) | Utilities for using the JS plugin with React and Vue. |
| [parcellab-embedded-ui-snippets](https://github.com/parcelLab/parcellab-embedded-ui-snippets) | Monorepo for embeddable storefront UI widgets (delivery promise, size recommendation). |
| [regionIdentifier](https://github.com/parcelLab/regionIdentifier) | ISO 3166-2 region lookup from country + zip code. |
| [charts](https://github.com/parcelLab/charts) | parcelLab Helm Charts (Apache-2.0). |
| [parcellab-mcp-server](https://github.com/parcelLab/parcellab-mcp-server) | Model Context Protocol server fronting the parcelLab API. |
| [magento-2-webhook](https://github.com/parcelLab/magento-2-webhook) | Magento 2 integration. |

## Solutions

- **Convert** — Pre-checkout delivery promise.
- **Engage** — Email, SMS, push, webhook, and order status page communications.
- **Retain** — Returns Portal with refunds, exchanges, retention offers, claims.
- **Insights** — Trackings, communications, control tower, benchmarking, premium analytics.
- **AI Agents** — WISMO/R Agent, Insights Agent, Fraud & Abuse Insights.

## Offices

- Munich (HQ) — parcelLab GmbH, Kapellenweg 6, 81371 Munich, Germany
- Boston — 75 State Street, Boston, MA 02109, USA
- London — Moor Place, 1 Fore Street Avenue, London EC2Y 9DT, UK
- Paris — 24-26 Rue De la Pépinière, 75008 Paris, France

## Maintainers

- Kin Lane — kin@apievangelist.com
