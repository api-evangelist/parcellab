# parcelLab

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

parcelLab connects delivery promises, shipment tracking, customer communications, and returns through APIs and AI agents. Retailers can show delivery dates before checkout, keep customers informed after purchase, and build branded tracking and returns experiences. Developers can integrate these capabilities into storefronts, order and warehouse systems, customer service tools, and AI assistants.

The platform offers REST APIs, shipment and return event integrations, an Agents API, and hosted Model Context Protocol (MCP) servers. Agents can work with order and return flows and, with the required permissions, configure the customer experience through MCP tools.

**Areas** · Delivery Promise · Order Management · Shipment Tracking · Returns and Exchanges · Customer Communications · AI Agents · MCP · E-Commerce

The coverage notes below were contributed for review on **2026-11-06**. They link to the public v4 specification, MCP discovery documents, and parcelLab developer guides. Guide descriptions were also checked against local documentation and implementation sources. Public verification results are recorded below to support catalog corrections and a new assessment.

## Start here

- [Interactive API v4 reference](https://product-api.parcellab.com/v4/docs/)
- [OpenAPI specification](https://product-api.parcellab.com/v4/openapi/?format=json)
- [Markdown API reference for developers and agents](https://product-api.parcellab.com/v4/docs/markdown/)
- [Developer guides for API v4](https://docs.parcellab.com/developers/v4)
- [Developer guides for API v2 LTS](https://docs.parcellab.com/developers/v2)
- [MCP connection and access](#mcp-for-ai-assistants)
- [Agents API](#agents-api)

## API v4 coverage

The public specification contains **75 operations across 56 paths and 16 tag groups**, checked on 2026-11-06. Each group is listed below. Translations appear under two tags, so group counts overlap. Access depends on the operation, account configuration, and permissions. Use the linked operation reference for request fields, authentication, and response schemas.

| API group | What developers can build | Operations | Reference |
| --- | --- | ---: | --- |
| Agents | Embed configured agents in applications and support channels. Start executions, read thread status and messages, and continue conversations. | 3 | [API reference](https://product-api.parcellab.com/v4/docs/markdown/agents/) |
| Apps | Render Order Status Page plugins and invoke deployed app ingress webhooks. | 2 | [API reference](https://product-api.parcellab.com/v4/docs/markdown/apps/) |
| Campaign | Evaluate campaign targeting and record campaign redirect activity. | 2 | [API reference](https://product-api.parcellab.com/v4/docs/markdown/campaign/) |
| Customer Portals | Retrieve the customer portals available for an account. | 1 | [API reference](https://product-api.parcellab.com/v4/docs/markdown/customer-portals/) |
| Events | Send shop and warehouse events into the shipment lifecycle. | 1 | [API reference](https://product-api.parcellab.com/v4/docs/markdown/events/) |
| Order | Create, update, list, and look up orders and trackings. Retrieve shipment status and an order status widget. | 6 | [API reference](https://product-api.parcellab.com/v4/docs/markdown/order/) |
| Order Status Page Theme | Create and edit branded tracking themes and assets, then publish them. | 11 | [API reference](https://product-api.parcellab.com/v4/docs/markdown/order-status-page-theme/) |
| Place Info | Find pickup and drop-off locations. List, retrieve, upsert, and remove account location records. | 5 | [API reference](https://product-api.parcellab.com/v4/docs/markdown/place-info/) |
| Promise | Calculate delivery date predictions for product pages and checkout. | 1 | [API reference](https://product-api.parcellab.com/v4/docs/markdown/promise/) |
| Return Configuration Set | Retrieve return configurations and document templates, and read or update translations. | 5 | [API reference](https://product-api.parcellab.com/v4/docs/markdown/return-configuration-set/) |
| Return Registration | Build headless returns and exchanges, from order lookup and item validation through return options, pickup availability, submission, labels, receipt, and lifecycle updates. | 19 | [Interactive API reference](https://product-api.parcellab.com/v4/docs/) |
| Size Recommender | List articles with fit information and retrieve size recommendations. | 3 | [API reference](https://product-api.parcellab.com/v4/docs/markdown/size-recommender/) |
| Survey | Retrieve surveys and themes, and read or submit survey answers. | 4 | [API reference](https://product-api.parcellab.com/v4/docs/markdown/survey/) |
| Theme | Create and edit Returns Portal themes and assets, then publish them. | 11 | [API reference](https://product-api.parcellab.com/v4/docs/markdown/theme/) |
| Translation | Retrieve return translations and update translation strings. | 2 | [API reference](https://product-api.parcellab.com/v4/docs/markdown/translation/) |
| Voucher | Check voucher availability. | 1 | [API reference](https://product-api.parcellab.com/v4/docs/markdown/voucher/) |

### Promise from checkout to delivery

The Promise API returns delivery predictions for the account's configured delivery methods. Integrations can use destination, carrier, service level, and warehouse information to show an estimated date or date range before purchase. Keep the promise shown at checkout with the order so later communications can refer to that commitment. The v4 entry point is `GET /v4/promise/prediction/predict/`. API v2 LTS also documents `GET /v2/prediction`. [Promise API reference](https://product-api.parcellab.com/v4/docs/markdown/promise/), [Promise integration guide](https://docs.parcellab.com/developers/v4/promise/api).

### Agents API

The Agents API embeds a configured parcelLab agent into a support tool, application, or chat interface. It supports asynchronous execution and continued conversations through three operations.

| Operation | Endpoint |
| --- | --- |
| Start an execution | `POST /v4/agents/{agent_id}/execute/` |
| Read thread status and messages | `GET /v4/agents/{agent_id}/threads/{thread_ref}/` |
| Add a message to a thread | `POST /v4/agents/{agent_id}/threads/{thread_ref}/messages/` |

Use the returned thread reference to poll for completion and continue the conversation. The integration requires an agent configured for the account, API access, and the account's AI opt-in. Follow the response schema for execution status values. [Agents API reference](https://product-api.parcellab.com/v4/docs/markdown/agents/).

## MCP for AI assistants

parcelLab hosts MCP servers that let compatible AI clients use parcelLab through tools. The customer endpoints serve two workflows.

| Endpoint | Use |
| --- | --- |
| `https://agents.parcellab.com/mcp/` | Shopper service workflows, including order status and guided return registration. |
| `https://agents.parcellab.com/admin/mcp/` | Account configuration, including journeys, messages, Returns Portals, Order Status Pages, themes, translations, campaigns, and notifications. |

The configuration endpoint lets teams use an assistant to inspect settings, prepare changes, and publish supported configuration. Available tools depend on the signed-in user's account access and roles. The documented connection requires the account's AI opt-in, OAuth support, and Streamable HTTP. [MCP developer guide](https://docs.parcellab.com/developers/v4/mcp/mcp-server).

For example, connect Claude Code to the configuration endpoint, then complete the parcelLab sign-in and consent flow.

```bash
claude mcp add --transport http parcellab https://agents.parcellab.com/admin/mcp/
```

An assistant can use the shopper endpoint to answer an order status question or guide a return. An authorized configuration user can ask it to inspect a journey or prepare a Returns Portal theme change. Tool permissions determine the actions available to that user. The guide documents read/write tool annotations and an approval step for publishing. [MCP setup and permissions](https://docs.parcellab.com/developers/v4/mcp/mcp-server).

The live server publishes OAuth protected-resource metadata and authorization-server metadata. On 2026-11-06, these advertised authorization-code and refresh-token grants, dynamic client registration, and PKCE with `S256`. Clients can discover the authorization endpoints and supported scopes from these documents. [Protected-resource metadata](https://agents.parcellab.com/.well-known/oauth-protected-resource), [Authorization-server metadata](https://agents.parcellab.com/.well-known/oauth-authorization-server).

### Authentication by interface

| Interface | Credential and flow | Access checks |
| --- | --- | --- |
| REST API, including Agents | Send `Authorization: Parcellab-API-Token <encoded-token>`. The value is `base64(account_id:token)`, with the colon and no trailing newline. The parcelLab App supplies an already encoded value. Copy it directly. | The token needs the scope for the HTTP method and access to the requested account. |
| REST API with provisioned OAuth | Send `Authorization: Bearer <access-token>` for an unbound token. For a DPoP-bound token, send `Authorization: DPoP <access-token>` and a signed `DPoP` proof for each request. | The identity and operation permissions apply. The specification lists `ES256` and `RS256` for DPoP proofs. |
| MCP | Let an OAuth-capable MCP client perform discovery, parcelLab sign-in, consent, and token acquisition. Use Streamable HTTP with either customer endpoint above. | Tool scopes, account access, user roles, and AI opt-in determine available actions. Account API tokens are for REST integrations. |
| Public storefront and Returns Portal operations | Use the operation's documented public parameters or verification flow. | Account configuration, recipient verification, and supported Returns Portal nonces still apply. |

API tokens use the `Parcellab-API-Token` authorization scheme. OAuth access tokens use the scheme defined by their OAuth flow. Keep API tokens in server-side integrations. The [authentication guide](https://docs.parcellab.com/developers/v4/getting-started/authentication) describes token creation and endpoint access. The live contract defines the supported security schemes. [OpenAPI specification](https://product-api.parcellab.com/v4/openapi/?format=json).

For API tokens, order reads accept `read` or `track:read`, and order writes accept `write` or `track:write`. Agent execution and message submission accept `write` or `agents:write`. Reading an agent thread accepts `read` or `agents:read`. The agent must be available to the account, with AI opt-in enabled. [Authentication guide](https://docs.parcellab.com/developers/v4/getting-started/authentication), [Agents API](https://product-api.parcellab.com/v4/docs/markdown/agents/).

Public access is operation-specific. The live specification permits unauthenticated requests for campaign evaluation and redirects, Size Recommender, Promise prediction, return order lookup, and public order status. Required input and account checks still apply. Order status can require recipient email, postal code, or a security hash. Return order lookup uses the Returns Portal's verification rules. Supported subsequent return actions can use `x-parcellab-nonce`. [Authentication guide](https://docs.parcellab.com/developers/v4/getting-started/authentication), [Live operation contracts](https://product-api.parcellab.com/v4/openapi/?format=json).

In OpenAPI, separate security objects are alternatives. An empty security object `{}` permits unauthenticated access, and `security: []` removes an operation's authentication requirement. When `security` is omitted, the root declaration applies. The current v4 contract has no root-level security requirement. Consult the operation guide for verification rules and Returns Portal nonce flows that are not fully represented by those declarations. [OpenAPI specification](https://product-api.parcellab.com/v4/openapi/?format=json).

### Verify access

For a server integration, use an account API token with `read` or `track:read` to make a read-only order-list request.

```bash
curl --request GET 'https://api.parcellab.com/v4/track/orders/' \
  --header 'Authorization: Parcellab-API-Token <encoded-token>'
```

A successful response verifies this credential's access to this operation. An account with no orders returns an empty `results` array. HTTP `401` indicates an authentication problem, and HTTP `403` indicates an access or permission problem. Read the response's error details to identify the cause. For MCP, finish sign-in and invoke a read-only tool on an authorized account. Tool availability and write permission require their own checks. [Authentication guide](https://docs.parcellab.com/developers/v4/getting-started/authentication).

OpenAPI and OAuth discovery documents are accessible without signing in. Reading them verifies the published contracts and discovery configuration. The verification steps above check credential access. Developers and agents can also use the [Markdown API reference](https://product-api.parcellab.com/v4/docs/markdown/) for operation details, schemas, and documented errors.

## Additional documented integration services

API v2 LTS and the integration guides cover services beyond the public v4 specification. The Backend route definitions were cross-checked against these guides. Use the guide for each service's access requirements and setup.

| Service | Coverage | Documentation |
| --- | --- | --- |
| Orders and tracking ingestion | Send order and shipment data through the documented LTS APIs. | [Orders and trackings](https://docs.parcellab.com/developers/v2/orders/trackings-orders) |
| Tracking search and checkpoints | Search recent trackings and retrieve shipment status and checkpoint history. | [Search](https://docs.parcellab.com/developers/v2/orders/search), [Checkpoints](https://docs.parcellab.com/developers/v2/status-updates/checkpoints) |
| Notification history | Retrieve sent notifications for a tracking. | [Tracking notifications](https://docs.parcellab.com/developers/v2/status-updates/checkpoints) |
| Files and attachments | Upload data files and tracking attachments. | [Files and attachments](https://docs.parcellab.com/developers/v2/orders/files-and-attachments) |
| Customer communications | Trigger and re-trigger messages for a tracking. | [Trigger messages](https://docs.parcellab.com/developers/v2/orders/trigger-messages) |
| Shipment webhooks | Receive configured shipment events and status data at an HTTPS receiver. | [Tracking webhooks](https://docs.parcellab.com/developers/v2/data-elements/get-status-updates/webhooks) |
| Return events and RMA actions | Receive return data and manage returns, labels, and pickup actions. | [Return data](https://docs.parcellab.com/developers/v2/returns/receive-data), [RMA actions](https://docs.parcellab.com/developers/v2/returns/rma-actions-api) |
| Claims | Submit a claim for a tracking. | [Claims](https://docs.parcellab.com/developers/v2/orders/claim) |
| Carrier data integration | Supply scans, status events, and live location data through documented carrier integrations. | [Carrier integration](https://docs.parcellab.com/developers/v2/data-elements/carrier-integration) |
| Apple Wallet | Integrate parcel tracking with Apple Wallet. | [Apple Wallet](https://docs.parcellab.com/developers/v2/status-updates/apple-wallet) |
| Data protection | Request disclosure or erasure through account-authorized APIs. | [Data protection](https://docs.parcellab.com/developers/v2/security/data-protection) |
| Barcode generation | Generate barcodes for supported formats. | [Barcodes](https://docs.parcellab.com/developers/v2/utility-services/barcodes) |

### Source verification

On 2026-11-06, the public OpenAPI specification, interactive API reference, and MCP OAuth discovery documents returned HTTP 200 without credentials. The specification supplies the v4 operation coverage and REST security declarations above. MCP metadata supplies the authorization, registration, and PKCE evidence.

The documentation host returned HTTP 403 to the review client. Guide descriptions were checked locally, and the linked guide paths follow the GitBook site configuration. These guide links still need an independent public check. The Markdown return-registration page returned HTTP 500, so its table entry links to the interactive reference. This review checked documentation and discovery metadata.

## parcelLab on APIs.io

API Evangelist publishes its derived catalog artifacts on APIs.io. The coverage sections above describe additional APIs and capabilities for catalog review. [Provider profile](https://apis.io/providers/parcellab/).

### Catalog entries (8)

- [parcelLab MCP Server](https://apis.io/apis/parcellab/parcellab-mcp/) — Hosted MCP access for AI assistants. The shopper endpoint supports order and return workflows, and the configuration endpoint supports authorized account setup changes. See [MCP coverage](#mcp-for-ai-assistants).
- [parcelLab Campaigns API](https://apis.io/apis/parcellab/parcellab-campaigns-api/) — Evaluate campaign targeting and redirect analytics events.
- [parcelLab Events API](https://apis.io/apis/parcellab/parcellab-events-api/) — Send custom shop or warehouse events into the tracking timeline.
- [parcelLab Orders API](https://apis.io/apis/parcellab/parcellab-orders-api/) — Create, update, and inspect orders and their trackings.
- [parcelLab Place Info API](https://apis.io/apis/parcellab/parcellab-place-info-api/) — Look up nearby pickup and drop-off (PUDO) locations.
- [parcelLab Promise API](https://apis.io/apis/parcellab/parcellab-promise-api/) — Pre-checkout delivery date predictions.
- [parcelLab Returns API](https://apis.io/apis/parcellab/parcellab-returns-api/) — Return registrations, configurations, and document templates.
- [parcelLab Surveys API](https://apis.io/apis/parcellab/parcellab-surveys-api/) — Retrieve survey definitions and submit responses.

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### Arazzo workflows (11)

Multi-step workflows that chain operations into a business task.

- [parcelLab Create and Fetch Return](https://apis.io/arazzos/parcellab/parcellab-create-and-fetch-return-workflow/)
- [parcelLab Evaluate Campaign and Log Redirect](https://apis.io/arazzos/parcellab/parcellab-evaluate-campaign-and-redirect-workflow/)
- [parcelLab List and Get Return](https://apis.io/arazzos/parcellab/parcellab-list-and-get-return-workflow/)
- [parcelLab Predict Delivery and Create Order](https://apis.io/arazzos/parcellab/parcellab-predict-then-create-order-workflow/)
- [parcelLab PUDO Lookup and Register Return](https://apis.io/arazzos/parcellab/parcellab-pudo-lookup-and-register-return-workflow/)
- [parcelLab Register Return and Collect Survey](https://apis.io/arazzos/parcellab/parcellab-register-return-and-survey-workflow/)
- [parcelLab Resolve Config and Register Return](https://apis.io/arazzos/parcellab/parcellab-resolve-config-and-register-return-workflow/)
- [parcelLab Send Event and Refresh Status](https://apis.io/arazzos/parcellab/parcellab-send-event-and-refresh-workflow/)
- [parcelLab Survey Fetch and Submit](https://apis.io/arazzos/parcellab/parcellab-survey-fetch-and-submit-workflow/)
- [parcelLab Track and Target Campaign](https://apis.io/arazzos/parcellab/parcellab-track-and-target-campaign-workflow/)
- [parcelLab Create Order and Track](https://apis.io/arazzos/parcellab/parcellab-upsert-order-and-track-workflow/)

#### Agentic access (1)

Which operations an agent can call, which act, and which need a human in the loop.

- [parcelLab Agentic Access](https://apis.io/agentic-access/parcellab/parcellab-agentic-access/)

#### JSON Schema (6)

The data models the API reads and writes.

- [parcelLab Address](https://apis.io/schemas/parcellab/parcellab-address/)
- [parcelLab Line Item](https://apis.io/schemas/parcellab/parcellab-line-item/)
- [parcelLab Order](https://apis.io/schemas/parcellab/parcellab-order/)
- [parcelLab Promise Prediction](https://apis.io/schemas/parcellab/parcellab-promise-prediction/)
- [parcelLab Return Registration](https://apis.io/schemas/parcellab/parcellab-return-registration/)
- [parcelLab Tracking](https://apis.io/schemas/parcellab/parcellab-tracking/)

#### JSON Structure (2)

Data models expressed in JSON Structure.

- [parcelLab Order Structure](https://apis.io/json-structure/parcellab/parcellab-order-structure/)
- [parcelLab Return Registration Structure](https://apis.io/json-structure/parcellab/parcellab-return-registration-structure/)

#### JSON-LD (1)

Linked-data contexts for the provider's vocabulary.

- [parcelLab Context](https://apis.io/jsonld/parcellab/parcellab-context/)

#### Vocabulary (1)

The provider's domain terms, defined.

- [parcelLab Vocabulary](https://apis.io/vocabularies/parcellab/parcellab-vocabulary/)

#### Examples (5)

Example requests and responses.

- [parcelLab Create Return Registration Example](https://apis.io/examples/parcellab/parcellab-create-return-registration-example/)
- [parcelLab Get Order Info Example](https://apis.io/examples/parcellab/parcellab-get-order-info-example/)
- [parcelLab Predict Delivery Example](https://apis.io/examples/parcellab/parcellab-predict-delivery-example/)
- [parcelLab Pudo Lookup Example](https://apis.io/examples/parcellab/parcellab-pudo-lookup-example/)
- [parcelLab Upsert Order Example](https://apis.io/examples/parcellab/parcellab-upsert-order-example/)

#### Collections (9)

Postman and Open Collection request collections.

- [parcelLab API](https://apis.io/collections/parcellab/open-parcellab/)
- [parcelLab Campaigns API](https://apis.io/collections/parcellab/open-parcellab-campaigns-api/)
- [parcelLab Events API](https://apis.io/collections/parcellab/open-parcellab-events-api/)
- [parcelLab Orders API](https://apis.io/collections/parcellab/open-parcellab-orders-api/)
- [parcelLab Place Info API](https://apis.io/collections/parcellab/open-parcellab-place-info-api/)
- [parcelLab Promise API](https://apis.io/collections/parcellab/open-parcellab-promise-api/)
- [parcelLab Returns API](https://apis.io/collections/parcellab/open-parcellab-returns-api/)
- [parcelLab Surveys API](https://apis.io/collections/parcellab/open-parcellab-surveys-api/)
- [parcelLab API](https://apis.io/collections/parcellab/postman-parcellab/)

#### Governance rules (2)

Spectral rulesets for the provider's contracts.

- [parcelLab — jsonschema rules](https://apis.io/rules/parcellab/parcellab-jsonschema-spectral-rules/)
- [parcelLab API Rules](https://apis.io/rules/parcellab/parcellab-rules/)

#### Security (3)

Authentication, trust centre, and vulnerability disclosure.

- [parcelLab Authentication](https://apis.io/security/parcellab/parcellab-authentication/)
- [parcelLab Domain Security](https://apis.io/security/parcellab/parcellab-domain-security/)
- [parcelLab Vulnerability Disclosure](https://apis.io/security/parcellab/parcellab-vulnerability-disclosure/)

#### Plans and pricing (1)

Published plans, tiers and prices.

- [parcelLab Plans Pricing](https://apis.io/plans/parcellab/parcellab-plans-pricing/)

#### Rate limits (1)

Published request limits.

- [parcelLab Rate Limits](https://apis.io/rate-limits/parcellab/parcellab-rate-limits/)

#### FinOps (1)

What the API costs to run, by operation.

- [parcelLab Finops](https://apis.io/finops/parcellab/parcellab-finops/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://parcellab.com)
- [Documentation](https://docs.parcellab.com/)
- [Getting started](https://docs.parcellab.com/developers/v4/getting-started/quickstart-guide)
- [API reference](https://product-api.parcellab.com/v4/docs/)
- [OpenAPI](https://product-api.parcellab.com/v4/openapi/?format=json)
- [MCP documentation](https://docs.parcellab.com/developers/v4/mcp/mcp-server)
- [Pricing](https://parcellab.com/contact-us)
- [Support](https://parcellab.com/contact-us)
- [Blog](https://parcellab.com/blog/)
- [Terms of service](https://parcellab.com/legal/terms-of-service/)
- [GitHub](https://github.com/parcelLab)
- [Status](https://status.parcellab.com)

## API Evangelist rating

**Kin Score 56.9** — strong · rubric 0.25.0 · scored 2026-10-23

| Facet | Score |
|---|---|
| Discoverability | 66.1 |
| Contract quality | 63.5 |
| Contract governance | 27.3 |
| Operational transparency | 34.2 |
| Developer ergonomics | 75.0 |
| Access clarity | 31.6 |

**Agent readiness 26.3** — agent-aware

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | yes |
| Agentic Access | derived (partial credit) |
| Reversibility Documented | — |
| MCP Server | — |
| Auth Clarity | bearer (partial credit) |
| Idempotency | — |
| Error Semantics | documented (partial credit) |
| OpenAPI Examples | documented (partial credit) |
| Rate Limit Signal | derived (partial credit) |
| Event Surface Described | — |
| Agent Skills | — |
| Well Known Catalog | — |
| Consent Identity | — |
| Agent Card | — |
| Dry Run Mode | — |
| Delegated Identity | — |
| Protected Resource Metadata | — |
| Dynamic Client Registration | — |
| Agentic Commerce | — |
| Pagination Ratio | paginated |
| Operation Distinctiveness | distinct |

**Regulatory alignment 22.5** — Horizontal (data, software, accessibility, platform)

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/parcellab/](https://apis.io/providers/parcellab/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for parcelLab: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/parcellab/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
