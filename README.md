# 0G Labs

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

0G Labs builds 0G (Zero Gravity), a decentralized AI operating system (deAIOS) that packages four modular layers into one stack: 0G Chain, an EVM-compatible Layer 1 with sub-second finality (mainnet "Aristotle", chain ID 16661); 0G Storage, a decentralized storage network for large AI datasets addressed by Merkle root hash and reachable through an indexer service, Go/TypeScript SDKs and a CLI; 0G DA, a data-availability layer using erasure coding and KZG commitments that OP Stack, Arbitrum Nitro and AVS rollups can settle against; and the 0G Compute Network, a decentralized GPU marketplace where every inference provider runs inside a TEE and attests to the model it serves. The developer-facing API is the 0G Compute Router at router-api.0g.ai — an OpenAI- and Anthropic-compatible gateway in front of the whole provider network, with a published OpenAPI 3.0 covering chat completions, the Anthropic messages shape, image generation and edits (sync and async), audio transcription, video generation, model and provider catalogs, routing preview, account balance and usage, and API-key management. Authentication splits into billable `sk-` API keys for inference and scope-limited `mk-` management keys for account and key administration.

**Areas:** Artificial Intelligence · Inference · LLM · GPU Compute · Decentralized Compute · Blockchain · Web3 · EVM · Decentralized Storage · Data Availability · OpenAI-Compatible · Trusted Execution Environment

## 0G Labs on APIs.io

Everything profiled for 0G Labs is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/0g-labs/](https://apis.io/providers/0g-labs/)** — or go straight to one of the APIs or properties below.

### APIs (9)

- [0G Chain JSON-RPC](https://apis.io/apis/0g-labs/0g-chain-json-rpc/) — Ethereum-compatible JSON-RPC endpoint for the 0G Chain mainnet ("Aristotle", chain ID 16661), an AI-focused Layer 1 with sub-second finality. Standard EVM…
- [0G DA (Data Availability) gRPC](https://apis.io/apis/0g-labs/0g-da-data-availability-grpc/) — gRPC surface for the 0G data-availability layer. The Disperser service accepts blobs asynchronously (DisperseBlob), exposes polling for processing state…
- [0G Storage Indexer](https://apis.io/apis/0g-labs/0g-storage-indexer/) — Indexer service for the 0G Storage network. It locates the storage nodes holding a file's segments, brokers uploads and downloads addressed by Merkle root…
- [0G Labs Account API](https://apis.io/apis/0g-labs/0g-labs-account-api/) — The Account API from 0G Labs — 5 operation(s) for account.
- [0G Labs API Key API](https://apis.io/apis/0g-labs/0g-labs-api-key-api/) — The API Key API from 0G Labs — 2 operation(s) for api key.
- [0G Labs Inference API](https://apis.io/apis/0g-labs/0g-labs-inference-api/) — The Inference API from 0G Labs — 11 operation(s) for inference.
- [0G Labs Models API](https://apis.io/apis/0g-labs/0g-labs-models-api/) — The Models API from 0G Labs — 1 operation(s) for models.
- [0G Labs Provider API](https://apis.io/apis/0g-labs/0g-labs-provider-api/) — The Provider API from 0G Labs — 1 operation(s) for provider.
- [0G Labs Service Types API](https://apis.io/apis/0g-labs/0g-labs-service-types-api/) — The Service Types API from 0G Labs — 1 operation(s) for service types.

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### MCP servers (1)

Model Context Protocol servers that expose the API to agents.

- [0g-router](https://apis.io/servers/0g-labs/0g-router/)

#### Collections (6)

Postman and Open Collection request collections.

- [0G Router Account API](https://apis.io/collections/0g-labs/open-0g-labs-account-api/)
- [0G Router API Key API](https://apis.io/collections/0g-labs/open-0g-labs-api-key-api/)
- [0G Router Inference API](https://apis.io/collections/0g-labs/open-0g-labs-inference-api/)
- [0G Router Models API](https://apis.io/collections/0g-labs/open-0g-labs-models-api/)
- [0G Router Provider API](https://apis.io/collections/0g-labs/open-0g-labs-provider-api/)
- [0G Router Service Types API](https://apis.io/collections/0g-labs/open-0g-labs-service-types-api/)

#### Overlays (1)

OpenAPI overlays, including conversational phrasing for each operation.

- [0G Labs Router Overlay](https://apis.io/overlays/0g-labs/0g-labs-router-overlay/)

#### Security (2)

Authentication, trust centre, and vulnerability disclosure.

- [0G Labs Authentication](https://apis.io/security/0g-labs/0g-labs-authentication/)
- [0G Labs Domain Security](https://apis.io/security/0g-labs/0g-labs-domain-security/)

#### Rate limits (1)

Published request limits.

- [0G Labs Rate Limits](https://apis.io/rate-limits/0g-labs/0g-labs-rate-limits/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://0g.ai)
- [Documentation](https://docs.0g.ai)
- [Getting started](https://docs.0g.ai/developer-hub/getting-started)
- [API reference](https://0gfoundation.github.io/0g-router/)
- [Sign up](https://pc.0g.ai)
- [Support](https://discord.gg/0glabs)
- [Blog](https://0g.ai/blog)
- [Terms of service](https://0g.ai/terms-of-service)
- [Privacy policy](https://0g.ai/privacy-policy)
- [GitHub](https://github.com/0gfoundation)
- [Status](https://status.0g.ai)

## API Evangelist rating

**Kin Score 48.8** — developing · rubric 0.24.0 · scored 2026-10-17

| Facet | Score |
|---|---|
| Discoverability | 64.3 |
| Contract quality | 47.6 |
| Contract governance | 4.5 |
| Operational transparency | 42.1 |
| Developer ergonomics | 85.7 |
| Access clarity | 34.2 |

**Agent readiness 30.6** — agent-ready

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | yes |
| Agentic Access | — |
| Reversibility Documented | — |
| MCP Server | — |
| Auth Clarity | bearer (partial credit) |
| Idempotency | documented (partial credit) |
| Error Semantics | verified |
| OpenAPI Examples | — |
| Rate Limit Signal | documented (partial credit) |
| Event Surface Described | — |
| Agent Skills | yes |
| Well Known Catalog | — |
| Consent Identity | — |
| Agent Card | — |
| Dry Run Mode | — |
| Delegated Identity | — |
| Protected Resource Metadata | — |
| Dynamic Client Registration | — |
| Agentic Commerce | — |

**Regulatory alignment 22.7** — Horizontal (data, software, accessibility, platform)

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/0g-labs/](https://apis.io/providers/0g-labs/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for 0G Labs: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/0g-labs/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
