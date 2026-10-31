# Obol

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

Obol builds distributed validator infrastructure for Ethereum, letting a validator be run across multiple independent operators and machines (a Distributed Validator, or DV) instead of a single node, which removes single points of failure in proof-of-stake staking. Its core software is Charon, a Go middleware client that coordinates the operators, plus the DV Launchpad dapp, the Obol Splits smart contracts, and the Obol API (api.obol.tech) with a TypeScript SDK for creating and managing clusters. The Obol API exposes cluster definitions, cluster locks, validator states, exits, deposits, fee recipients, effectiveness, peer scores, Techne credentials, and network staking metrics.

**Areas:** Company · Cryptocurrency · Ethereum · Staking · Distributed Validators · Blockchain Infrastructure · Web3

## Obol on APIs.io

Everything profiled for Obol is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/obol/](https://apis.io/providers/obol/)** — or go straight to one of the APIs or properties below.

### APIs (17)

- [Obol Address API](https://apis.io/apis/obol/obol-address-api/) — The Address API from Obol — 7 operation(s) for address.
- [Obol Cluster Definition API](https://apis.io/apis/obol/obol-cluster-definition-api/) — The Cluster Definition API from Obol — 4 operation(s) for cluster definition.
- [Obol Cluster Effectiveness API](https://apis.io/apis/obol/obol-cluster-effectiveness-api/) — The Cluster Effectiveness API from Obol — 1 operation(s) for cluster effectiveness.
- [Obol Cluster Lock API](https://apis.io/apis/obol/obol-cluster-lock-api/) — The Cluster Lock API from Obol — 22 operation(s) for cluster lock.
- [Obol Deposit Data API](https://apis.io/apis/obol/obol-deposit-data-api/) — The Deposit Data API from Obol — 4 operation(s) for deposit data.
- [Obol DV Exit API](https://apis.io/apis/obol/obol-dv-exit-api/) — The DV Exit API from Obol — 8 operation(s) for dv exit.
- [Obol DV Migrate API](https://apis.io/apis/obol/obol-dv-migrate-api/) — The DV Migrate API from Obol — 1 operation(s) for dv migrate.
- [Obol Fee Recipient API](https://apis.io/apis/obol/obol-fee-recipient-api/) — The Fee Recipient API from Obol — 4 operation(s) for fee recipient.
- [Obol Metrics API](https://apis.io/apis/obol/obol-metrics-api/) — The Metrics API from Obol — 1 operation(s) for metrics.
- [Obol OWR Information API](https://apis.io/apis/obol/obol-owr-information-api/) — The OWR Information API from Obol — 1 operation(s) for owr information.
- [Obol Positions API](https://apis.io/apis/obol/obol-positions-api/) — The Positions API from Obol — 2 operation(s) for positions.
- [Obol State API](https://apis.io/apis/obol/obol-state-api/) — The State API from Obol — 1 operation(s) for state.
- [Obol System API](https://apis.io/apis/obol/obol-system-api/) — System related endpoints.
- [Obol Techne Credentials API](https://apis.io/apis/obol/obol-techne-credentials-api/) — The Techne Credentials API from Obol — 4 operation(s) for techne credentials.
- [Obol Terms And Conditions API](https://apis.io/apis/obol/obol-terms-and-conditions-api/) — The Terms And Conditions API from Obol — 2 operation(s) for terms and conditions.
- [Obol Test API](https://apis.io/apis/obol/obol-test-api/) — The Test API from Obol — 2 operation(s) for test.
- [Obol Tvs API](https://apis.io/apis/obol/obol-tvs-api/) — The tvs API from Obol — 2 operation(s) for tvs.

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### MCP servers (1)

Model Context Protocol servers that expose the API to agents.

- [obol](https://apis.io/servers/obol/obol/)

#### Agentic access (1)

Which operations an agent can call, which act, and which need a human in the loop.

- [Obol Agentic Access](https://apis.io/agentic-access/obol/obol-agentic-access/)

#### Collections (17)

Postman and Open Collection request collections.

- [Obol Address API](https://apis.io/collections/obol/open-obol-address-api/)
- [Obol Address Cluster Definition API](https://apis.io/collections/obol/open-obol-cluster-definition-api/)
- [Obol Address Cluster Effectiveness API](https://apis.io/collections/obol/open-obol-cluster-effectiveness-api/)
- [Obol Address Cluster Lock API](https://apis.io/collections/obol/open-obol-cluster-lock-api/)
- [Obol Address Deposit Data API](https://apis.io/collections/obol/open-obol-deposit-data-api/)
- [Obol Address DV Exit API](https://apis.io/collections/obol/open-obol-dv-exit-api/)
- [Obol Address DV Migrate API](https://apis.io/collections/obol/open-obol-dv-migrate-api/)
- [Obol Address Fee Recipient API](https://apis.io/collections/obol/open-obol-fee-recipient-api/)
- [Obol Address Metrics API](https://apis.io/collections/obol/open-obol-metrics-api/)
- [Obol Address OWR Information API](https://apis.io/collections/obol/open-obol-owr-information-api/)
- [Obol Address Positions API](https://apis.io/collections/obol/open-obol-positions-api/)
- [Obol Address State API](https://apis.io/collections/obol/open-obol-state-api/)
- [Obol Address System API](https://apis.io/collections/obol/open-obol-system-api/)
- [Obol Address Techne Credentials API](https://apis.io/collections/obol/open-obol-techne-credentials-api/)
- [Obol Address Terms And Conditions API](https://apis.io/collections/obol/open-obol-terms-and-conditions-api/)
- [Obol Address Test API](https://apis.io/collections/obol/open-obol-test-api/)
- [Obol Address tvs API](https://apis.io/collections/obol/open-obol-tvs-api/)

#### Overlays (1)

OpenAPI overlays, including conversational phrasing for each operation.

- [Obol Openapi Overlay](https://apis.io/overlays/obol/obol-openapi-overlay/)

#### Security (3)

Authentication, trust centre, and vulnerability disclosure.

- [Obol Authentication](https://apis.io/security/obol/obol-authentication/)
- [Obol Domain Security](https://apis.io/security/obol/obol-domain-security/)
- [Obol Vulnerability Disclosure](https://apis.io/security/obol/obol-vulnerability-disclosure/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://obol.org/)
- [Documentation](https://docs.obol.org/)
- [Getting started](https://docs.obol.org/next/run-a-dv/start)
- [API reference](https://docs.obol.org/api)
- [Support](https://community.obol.org/)
- [Blog](https://blog.obol.org/)
- [Security](https://docs.obol.org/adv/security/overview)
- [Terms of service](https://obol.org/terms.pdf)
- [Privacy policy](https://obol.org/privacy-policy)
- [GitHub](https://github.com/ObolNetwork)
- [Status](https://status.obol.tech)

## API Evangelist rating

**Kin Score 45.0** — developing · rubric 0.25.0 · scored 2026-10-23

| Facet | Score |
|---|---|
| Discoverability | 73.2 |
| Contract quality | 47.2 |
| Contract governance | 4.5 |
| Operational transparency | 26.3 |
| Developer ergonomics | 80.4 |
| Access clarity | 21.1 |

**Agent readiness 20.2** — agent-aware

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | yes |
| Agentic Access | derived (partial credit) |
| Reversibility Documented | — |
| MCP Server | — |
| Auth Clarity | bearer (partial credit) |
| Idempotency | — |
| Error Semantics | derived (partial credit) |
| OpenAPI Examples | partial |
| Rate Limit Signal | — |
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
| Pagination Ratio | — |
| Operation Distinctiveness | — |

**Regulatory alignment 30.4** — Horizontal (data, software, accessibility, platform)

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/obol/](https://apis.io/providers/obol/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for Obol: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/obol/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
