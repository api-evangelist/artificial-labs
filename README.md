# Artificial Labs (artificial-labs)

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
