# Artificial Labs

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

Artificial Labs is a London-based insurance technology company building algorithmic and digital underwriting software for the specialty and reinsurance market, with the Lloyd's of London subscription market as its home ground. Founded and headquartered in the City of London at 1-3 Frederick's Place, and led by co-founders and co-CEOs David King and Johnny Bridges under chairman Martin Reith, the company sells three products to carriers, syndicates, MGAs and wholesale brokers: Smart Underwriting (a configurable lead-and-follow digital underwriting platform with appetite modelling and accept/refer/decline submission triage), Smart Placement (a broker-side placement and distribution platform) and Contract Builder (MRCv3-compliant structured digital contract creation, which powers PPL's integrated Digital Contract Capability). Named customers and partners include Apollo, PPL, BMS Group, Lockton and McGill and Partners, and the firm is an alumnus of the Lloyd's Lab accelerator. Its API posture is partner-gated and matches the London Market pattern: Artificial talks publicly and often about APIs as the connective tissue between broker PAS, carrier systems and its own platform, and describes real quote-and-bind flows in which risk data is pushed to the Artificial platform via API and a written line and rate are returned via API, but it publishes no public self-serve developer portal, no downloadable OpenAPI or Swagger definition, no public Postman collection and no public API host. api.artificial.io and developer.artificial.io do not resolve in DNS. The product documentation site at docs.artificial.io returns HTTP 200 on its landing page only, which states plainly "To view the documentation, you must sign in"; every product and reference path 302-redirects to an Auth0 authorization-code login at auth.artificialos.com, and docs robots.txt is Disallow all. Its GitHub organization, github.com/artificial-labs, exists but has zero public repositories. Where Artificial is genuinely and demonstrably standards-forward is ACORD: it joined the ACORD Solutions Group Licensed Integrator Partner program in October 2023, builds Contract Builder and Smart Placement on a structured data model incorporating MRCv3, ACORD GRLC and the Lloyd's Core Data Record, validates contracts pre-submission against MRCv3 and ACORD standards, and consumes the ACORD Transcriber API for automated data extraction. That is the honest shape of this record: real, working, standards-aligned insurance APIs that are invisible from outside the contractual relationship.

**Areas:** Insurance · United Kingdom · Insurtech · Underwriting · Reinsurance · Specialty Insurance · London Market · Lloyd's of London · Brokerage · Policy Administration · ACORD · Algorithmic Underwriting

## Artificial Labs on APIs.io

Everything profiled for Artificial Labs is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/artificial-labs/](https://apis.io/providers/artificial-labs/)** — or go straight to one of the APIs or properties below.

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### MCP servers (1)

Model Context Protocol servers that expose the API to agents.

- [artificial-labs](https://apis.io/servers/artificial-labs/artificial-labs/)

#### Security (4)

Authentication, trust centre, and vulnerability disclosure.

- [Artificial Labs Authentication](https://apis.io/security/artificial-labs/artificial-labs-authentication/)
- [Artificial Labs Domain Security](https://apis.io/security/artificial-labs/artificial-labs-domain-security/)
- [Artificial Labs Trust Center](https://apis.io/security/artificial-labs/artificial-labs-trust-center/)
- [Artificial Labs Vulnerability Disclosure](https://apis.io/security/artificial-labs/artificial-labs-vulnerability-disclosure/)

#### OAuth scopes (1)

The permissions the API asks for.

- [Artificial Labs Scopes](https://apis.io/scopes/artificial-labs/artificial-labs-scopes/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://artificial.io/)
- [Documentation](https://docs.artificial.io/docs-site/)
- [Support](https://artificial.io/contact/)
- [Blog](https://artificial.io/company/blog/)
- [Security](https://artificial.io/security/)
- [Compliance](https://trust.artificial.io/)
- [Terms of service](https://artificial.io/website-terms/)
- [Privacy policy](https://artificial.io/privacy/)
- [GitHub](https://github.com/artificial-labs)

## API Evangelist rating

**Kin Score 28.6** — thin · rubric 0.25.0 · scored 2026-10-23

| Facet | Score |
|---|---|
| Discoverability | 58.3 |
| Contract quality | 0.0 |
| Contract governance | 18.2 |
| Operational transparency | 13.2 |
| Developer ergonomics | 28.6 |
| Access clarity | 43.4 |

**Agent readiness 27.3** — agent-aware

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | — |
| Agentic Access | — |
| Reversibility Documented | — |
| MCP Server | verified |
| Auth Clarity | served (partial credit) |
| Idempotency | — |
| Error Semantics | — |
| OpenAPI Examples | — |
| Rate Limit Signal | — |
| Event Surface Described | — |
| Agent Skills | — |
| Well Known Catalog | — |
| Consent Identity | — |
| Agent Card | — |
| Dry Run Mode | — |
| Delegated Identity | served (partial credit) |
| Protected Resource Metadata | verified |
| Dynamic Client Registration | yes |
| Agentic Commerce | — |
| Pagination Ratio | na |
| Operation Distinctiveness | na |

**Regulatory alignment 46.5** — Insurance

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/artificial-labs/](https://apis.io/providers/artificial-labs/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for Artificial Labs: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/artificial-labs/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
