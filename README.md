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

parcelLab is a Munich-headquartered post-purchase experience platform (parcelLab GmbH) used by retailers including IKEA, Hugo Boss, Dyson, Puma, and John Lewis to turn delivery and returns into a branded, revenue-generating part of the customer journey. The platform spans four modules — Convert (pre-checkout delivery promise), Engage (multichannel post-purchase communications), Retain (Returns Portal and returns experience), and Insights (analytics, benchmarking, control tower) — layered with AI agents (WISMO/R, Insights, Fraud & Abuse) and exposed via the parcelLab API v4 Enhanced. Global, EU, and US regional endpoints are available; the same data backs a Model Context Protocol server at agents.parcellab.com/mcp/ for agentic clients.

**Areas:** Post-Purchase · E-Commerce · Tracking · Returns · Shipping · Delivery · Customer Experience · Logistics · Communications · Germany

## parcelLab on APIs.io

Everything profiled for parcelLab is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/parcellab/](https://apis.io/providers/parcellab/)** — or go straight to one of the APIs or properties below.

### APIs (8)

- [parcelLab MCP Server](https://apis.io/apis/parcellab/parcellab-mcp/) — Hosted Model Context Protocol server exposing the parcelLab order tracking and returns registration workflow to MCP-compatible agents, authenticated via…
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

- [Parcellab Agentic Access](https://apis.io/agentic-access/parcellab/parcellab-agentic-access/)

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

- [Parcellab Order Structure](https://apis.io/json-structure/parcellab/parcellab-order-structure/)
- [Parcellab Return Registration Structure](https://apis.io/json-structure/parcellab/parcellab-return-registration-structure/)

#### JSON-LD (1)

Linked-data contexts for the provider's vocabulary.

- [Parcellab Context](https://apis.io/jsonld/parcellab/parcellab-context/)

#### Vocabulary (1)

The provider's domain terms, defined.

- [parcelLab Vocabulary](https://apis.io/vocabularies/parcellab/parcellab-vocabulary/)

#### Examples (5)

Example requests and responses.

- [Parcellab Create Return Registration Example](https://apis.io/examples/parcellab/parcellab-create-return-registration-example/)
- [Parcellab Get Order Info Example](https://apis.io/examples/parcellab/parcellab-get-order-info-example/)
- [Parcellab Predict Delivery Example](https://apis.io/examples/parcellab/parcellab-predict-delivery-example/)
- [Parcellab Pudo Lookup Example](https://apis.io/examples/parcellab/parcellab-pudo-lookup-example/)
- [Parcellab Upsert Order Example](https://apis.io/examples/parcellab/parcellab-upsert-order-example/)

#### Collections (9)

Postman and Open Collection request collections.

- [parcelLab API](https://apis.io/collections/parcellab/open-parcellab/)
- [parcelLab Campaigns API](https://apis.io/collections/parcellab/open-parcellab-campaigns-api/)
- [parcelLab Campaigns Events API](https://apis.io/collections/parcellab/open-parcellab-events-api/)
- [parcelLab Campaigns Orders API](https://apis.io/collections/parcellab/open-parcellab-orders-api/)
- [parcelLab Campaigns Place Info API](https://apis.io/collections/parcellab/open-parcellab-place-info-api/)
- [parcelLab Campaigns Promise API](https://apis.io/collections/parcellab/open-parcellab-promise-api/)
- [parcelLab Campaigns Returns API](https://apis.io/collections/parcellab/open-parcellab-returns-api/)
- [parcelLab Campaigns Surveys API](https://apis.io/collections/parcellab/open-parcellab-surveys-api/)
- [parcelLab API](https://apis.io/collections/parcellab/postman-parcellab/)

#### Governance rules (2)

Spectral rulesets for the provider's contracts.

- [parcelLab — jsonschema rules](https://apis.io/rules/parcellab/parcellab-jsonschema-spectral-rules/)
- [parcelLab API Rules](https://apis.io/rules/parcellab/parcellab-rules/)

#### Security (3)

Authentication, trust centre, and vulnerability disclosure.

- [Parcellab Authentication](https://apis.io/security/parcellab/parcellab-authentication/)
- [Parcellab Domain Security](https://apis.io/security/parcellab/parcellab-domain-security/)
- [Parcellab Vulnerability Disclosure](https://apis.io/security/parcellab/parcellab-vulnerability-disclosure/)

#### Plans and pricing (1)

Published plans, tiers and prices.

- [Parcellab Plans Pricing](https://apis.io/plans/parcellab/parcellab-plans-pricing/)

#### Rate limits (1)

Published request limits.

- [Parcellab Rate Limits](https://apis.io/rate-limits/parcellab/parcellab-rate-limits/)

#### FinOps (1)

What the API costs to run, by operation.

- [Parcellab Finops](https://apis.io/finops/parcellab/parcellab-finops/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://parcellab.com)
- [Documentation](https://docs.parcellab.com/docs/readme)
- [Getting started](https://docs.parcellab.com/docs/onboarding)
- [API reference](https://docs.parcellab.com/docs/developers/getting-started/api-reference)
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
