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
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

0G Labs builds **0G (Zero Gravity)**, a decentralized AI operating system: an EVM-compatible L1
(0G Chain, mainnet "Aristotle", chain ID 16661), a decentralized storage network addressed by
Merkle root hash (0G Storage), a data-availability layer for rollups (0G DA), and a TEE-attested
GPU marketplace for AI inference (0G Compute).

## API surface

| API | Base URL | Contract |
|---|---|---|
| 0G Compute Router | `https://router-api.0g.ai/v1` | [OpenAPI 3.0](openapi/0g-labs-router-openapi.yml) — 23 operations, 126 schemas |
| 0G Chain JSON-RPC | `https://evmrpc.0g.ai` | Ethereum JSON-RPC (EIP-1474) |
| 0G DA | gRPC | [Disperser](grpc/0g-labs-da-disperser.proto) · [Retriever](grpc/0g-labs-da-retriever.proto) · [Signer](grpc/0g-labs-da-signer.proto) |
| 0G Storage Indexer | `https://indexer-storage-turbo.0g.ai` | Go/TS SDKs + `0g-storage-client` CLI |

The Router is OpenAI- and Anthropic-wire-compatible: change `base_url` and `api_key` and an
existing OpenAI client works. `GET /v1/models`, `/v1/providers` and `/v1/service-types` answer
anonymously, so the live catalog, pricing and provider health can be read with no credential.

## Notable findings

- **The OpenAPI is not where you would look for it.** `router-api.0g.ai/openapi.json`,
  `docs.0g.ai/openapi.json` and `0g.ai/openapi.json` all return 404. The real 183KB spec is
  published on GitHub Pages at `https://0gfoundation.github.io/0g-router/openapi.yaml`, linked
  only from the Router authentication docs page.
- **The changelog lives inside the OpenAPI.** `docs.0g.ai/changelog` is a 404; release notes are
  a `## Changelog` section of `info.description`.
- **0G ships Agent Skills, not MCP.** 14 provider-authored `SKILL.md` files plus an `AGENTS.md`
  orchestration guide — harvested verbatim into [`skills/`](skills/_index.yml). No first-party
  MCP server exists.
- **The skills don't cover the Router.** All 14 target the wallet-signed Direct SDK path, not the
  gateway 0G's own docs call "recommended for most applications" — see
  [`mcp/0g-labs-tool-crosswalk.yml`](mcp/0g-labs-tool-crosswalk.yml).
- **`llms.txt` links 404.** Every entry in `docs.0g.ai/llms.txt` carries a `/docs/` path prefix
  that returns 404; the same page without it returns 200.
- **No operationIds.** None of the 23 operations declares one; proposals are recorded in
  [`overlays/`](overlays/0g-labs-router-overlay.yaml) rather than edited into the harvested spec.
- **No `/.well-known/` surface, no A2A agent card, no security.txt, no published certifications.**

Sources: <https://0g.ai> · <https://docs.0g.ai> · <https://0gfoundation.github.io/0g-router/> ·
<https://github.com/0gfoundation>

