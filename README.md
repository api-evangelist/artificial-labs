# Artificial Labs (artificial-labs)

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

Artificial Labs is a London-based insurance technology company building algorithmic and digital underwriting software for the specialty and reinsurance market, with the Lloyd's of London subscription market as its home ground. Founded and headquartered in the City of London and led by co-founders and co-CEOs David King and Johnny Bridges under chairman Martin Reith, it sells Smart Underwriting, Smart Placement and Contract Builder to carriers, syndicates, MGAs and wholesale brokers. Named customers and partners include Apollo, PPL, BMS Group, Lockton and McGill and Partners, and the firm is a Lloyd's Lab accelerator alumnus.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/artificial-labs/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/artificial-labs/refs/heads/main/apis.yml)

## Tags

- Insurance
- United Kingdom
- Insurtech
- Underwriting
- Reinsurance
- Specialty Insurance
- London Market
- Lloyd's of London
- Broker
- Policy Administration
- ACORD
- Algorithmic Underwriting

## Timestamps

- **Created:** 2026-07-25
- **Modified:** 2026-07-25

## APIs

**None listed — and that is the accurate finding.**

Artificial Labs runs real production APIs and talks about them openly, but none of that surface is public. There is no self-serve developer portal, no retrievable OpenAPI or Swagger definition, no public API host, no public Postman collection, no GraphQL endpoint and no event or webhook catalog.

- `docs.artificial.io` is the only documentation host. `https://docs.artificial.io/docs-site/` returns **HTTP 200**, but the page carries no reference material — it says verbatim *"To view the documentation, you must sign in."* Every product and reference path below it (`/smart-underwriting/`, `/smart-placement/`, `/contract-builder/`, `/docs-site/reference/glossary/`) returns **HTTP 302** to an Auth0 authorization-code login at `https://auth.artificialos.com/authorize`. `robots.txt` on that host is `Disallow: /`.
- `api.artificial.io`, `developer.artificial.io`, `developers.artificial.io`, `app.artificial.io` and `platform.artificial.io` have **no DNS records**. On the marketing site, `/developers`, `/api`, `/developer`, `/partners` and `/integrations` all return **HTTP 404**, and the 147-URL sitemap contains no developer page.
- `github.com/artificial-labs` exists but has **zero public repositories**.

This is the London Market pattern: the API work is genuine and standards-aligned, and it is entirely invisible outside a contractual relationship.

## ACORD posture

ACORD Solutions Group **Licensed Integrator Partner** (joined October 2023). Contract Builder and Smart Placement run on a structured data model incorporating **MRCv3**, **ACORD GRLC** and the **Lloyd's Core Data Record (CDR)**, with pre-submission validation built around MRCv3 and ACORD standards. Artificial also consumes the third-party **ACORD Transcriber API** for automated data extraction. No AL3, NGDS, IVANS or agency-download reference was found — consistent with a London Market specialty player rather than a US retail-agency one.

## Quote / bind / issue / FNOL

| Verb | Public API | Audience | Notes |
| --- | --- | --- | --- |
| Quote | No | Partner (broker PAS → syndicate) | Company blog describes risk data pushed to the Artificial platform via API against a syndicate's underwriting appetite. |
| Bind | No | Partner (broker PAS → syndicate) | Written line and rate calculated and returned via API to the broker and underwriter PAS. |
| Issue | No | Partner (broker) | Contract Builder generates MRCv3-compliant digital contracts; powers PPL's integrated Digital Contract Capability. |
| FNOL | No | — | No claims or FNOL product or API surface exists. |

## Auth model

OAuth 2.0 / OpenID Connect authorization code via Auth0 (UK tenant, `artificial.uk.auth0.com`). Discovery is public at [https://auth.artificialos.com/.well-known/openid-configuration](https://auth.artificialos.com/.well-known/openid-configuration) (HTTP 200) and advertises only standard OIDC scopes — `openid profile email`. No public API-key issuance, no client-credentials documentation, no published domain scopes. Partner API credentials are issued out of band.

## Artifacts harvested

The 2026-07-25 enrichment round re-ran contract discovery against every resolving host (including a certificate-transparency sweep of `*.artificial.io`) and confirmed the no-public-contract finding: `api.genesis.preview.artificial.io`, `genesis.preview.artificial.io` and `artificialos.preview.artificial.io` have DNS records but answer nothing, and `office.artificial.io` is an office-move microsite with no API. What it did find and save:

- `well-known/` — the Auth0 tenant publishes a full anonymous discovery surface: [`/.well-known/openid-configuration`](https://auth.artificialos.com/.well-known/openid-configuration) (200), [`/.well-known/oauth-authorization-server`](https://auth.artificialos.com/.well-known/oauth-authorization-server) (200, byte-identical) and `jwks.json` (200, two RS256 keys). No `security.txt`, `api-catalog`, `ai-plugin.json` or agent card anywhere.
- `authentication/` + `scopes/` — the full OAuth 2.0 / OIDC profile: authorization code with PKCE (S256), client credentials, device code, CIBA, RFC 8693 token exchange, `private_key_jwt`, DPoP (ES256), MFA. Only standard OIDC scopes are published; **no insurance-domain scopes exist publicly**.
- `security/` — a **Vanta trust center at [trust.artificial.io](https://trust.artificial.io/)** (found by hand; the page is client-rendered and exposes no anonymous JSON), plus **ISO 27001** and **Cyber Essentials Plus** certifications, HSTS-enforced TLS 1.3, AES-256 at rest and external penetration testing from the security page. No security.txt, no bug bounty; the only disclosure route is `privacy@artificial.io` in the Acceptable Use Policy.
- `conformance/` — twelve identity standards verified live; ACORD, ACORD GRLC, MRC v3 and the Lloyd's Core Data Record recorded as **claimed** (company-published, not externally testable).
- `lifecycle/` — no status page, no deprecation policy, no SLA. `artificial.statuspage.io` resolves but is a **squatted generic-word page** with placeholder components and 2023 spam, explicitly *not* recorded as this provider's status page.
- `packages/` — zero first-party SDKs on npm, PyPI or any other registry; the PyPI project `artificial` is unrelated.
- `llms/` — generated agent-readable summary of what is genuinely public.

## Links

- [Website](https://artificial.io/)
- [Documentation (sign-in required)](https://docs.artificial.io/docs-site/)
- [About](https://artificial.io/about/)
- [Blog](https://artificial.io/company/blog/)
- [Security](https://artificial.io/security/)
- [Contact](https://artificial.io/contact/)
- [GitHub](https://github.com/artificial-labs)
- [LinkedIn](https://www.linkedin.com/company/artificial-labs)

## Review

See [review.yml](review.yml) for the full API Evangelist reviewer finding, every probed URL with its HTTP status, and ACORD provenance.
