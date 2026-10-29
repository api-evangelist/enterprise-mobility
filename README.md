# Enterprise Mobility

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

Enterprise Mobility is the Clayton, Missouri parent of Enterprise Rent-A-Car, National Car Rental and Alamo Rent a Car, and the largest car rental provider in the world — 90,000+ team members, 9,500+ rental branches across more than 90 countries and territories, a global fleet of over 2.4 million vehicles and $39 billion in 2025 fiscal-year revenue. Beyond leisure and corporate car rental it operates fleet management, flexible vehicle hire, carsharing, vanpooling, truck rental, car sales, vehicle subscription and the ARMS / Entegral replacement-rental technology used by insurers, collision repairers and dealerships. In the United States travel distribution chain it is a ground-transportation supplier whose inventory reaches buyers through GDS and OTA intermediaries, corporate travel programs and its own direct brand sites, rather than through any published public booking API. Its API posture is partner-gated and honestly so: EHI runs a real API Marketplace at developer.ehi.com with public marketing overviews for three business lines — Rental, Replacement Rental and Commute — but the API catalog, API specs, guides and release notes all sit behind Azure AD B2C sign-in and the portal states access is for "an Enterprise employee or trusted Partner" who should "contact your account manager ... to request access". No OpenAPI is published for those business lines; probes of /openapi.json, /swagger.json, /api-docs and /.well-known/ return AEM soft-404 HTML or 404. What is public is the plumbing around the gate: the production API gateway at api.ehi.com is a live Kong Gateway behind Imperva, the marketplace's own experience API publishes three POST endpoints in the portal's anonymous page source, the Azure AD B2C tenant serves two readable OpenID Connect discovery documents, and the sign-in link enumerates fourteen OAuth scopes covering catalog search, client-application registration and authorization requests. The published API License Agreement grants only a "limited, revocable, non-transferable, non-sublicensable, non-exclusive" right, restricts use to the licensee's internal purpose, states the licensee has no ownership rights in Renter Information, and on termination requires the licensee to "delete or return any copies of the APIs and Enterprise Content" — public docs shell, gated specs, no exit path.

**Areas:** Travel · United States · Car Rental · Ground Transportation · Mobility · Corporate Travel · Distribution · Fleet Management · Insurance Replacement Rental · Booking

## Enterprise Mobility on APIs.io

Everything profiled for Enterprise Mobility is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/enterprise-mobility/](https://apis.io/providers/enterprise-mobility/)** — or go straight to one of the APIs or properties below.

### APIs (4)

- [EHI Rental APIs](https://apis.io/apis/enterprise-mobility/ehi-rental-apis/) — The Rental business line of the EHI API Marketplace, covering Enterprise Rent-A-Car's network of neighborhood and airport branches. The public overview page…
- [EHI Replacement Rental APIs](https://apis.io/apis/enterprise-mobility/ehi-replacement-rental-apis/) — The Replacement Rental business line of the EHI API Marketplace, exposing the ARMS (Automated Rental Management System) and Entegral platforms to insurance…
- [EHI Commute APIs](https://apis.io/apis/enterprise-mobility/ehi-commute-apis/) — The Commute business line of the EHI API Marketplace, covering Commute with Enterprise vanpooling and rideshare-to-work programs sold to employers. The…
- [EHI API Marketplace Experience API](https://apis.io/apis/enterprise-mobility/ehi-marketplace-experience-api/) — The backend-for-frontend that powers the EHI API Marketplace itself, and the only Enterprise Mobility API surface with endpoints published anonymously.…

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### Security (3)

Authentication, trust centre, and vulnerability disclosure.

- [Enterprise Mobility Authentication](https://apis.io/security/enterprise-mobility/enterprise-mobility-authentication/)
- [Enterprise Mobility Domain Security](https://apis.io/security/enterprise-mobility/enterprise-mobility-domain-security/)
- [Enterprise Mobility Vulnerability Disclosure](https://apis.io/security/enterprise-mobility/enterprise-mobility-vulnerability-disclosure/)

#### OAuth scopes (1)

The permissions the API asks for.

- [Enterprise Mobility Scopes](https://apis.io/scopes/enterprise-mobility/enterprise-mobility-scopes/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://www.enterprisemobility.com/)
- [Documentation](https://developer.ehi.com/apis-overview.html)
- [Support](https://developer.ehi.com/general/contact-us.html)
- [Blog](https://www.enterprisemobility.com/en/news-stories.html)
- [Terms of service](https://developer.ehi.com/general/terms-of-use.html)
- [Privacy policy](https://developer.ehi.com/general/privacy-policy.html)

## API Evangelist rating

**Kin Score 24.1** — emerging · rubric 0.24.0 · scored 2026-10-17

| Facet | Score |
|---|---|
| Discoverability | 62.5 |
| Contract quality | 0.0 |
| Contract governance | 18.2 |
| Operational transparency | 0.0 |
| Developer ergonomics | 38.1 |
| Access clarity | 21.1 |

**Agent readiness 5.4** — agent-aware

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | — |
| Agentic Access | — |
| Reversibility Documented | — |
| MCP Server | — |
| Auth Clarity | bearer (partial credit) |
| Idempotency | — |
| Error Semantics | documented (partial credit) |
| OpenAPI Examples | — |
| Rate Limit Signal | — |
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

**Regulatory alignment 42.1** — Insurance

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/enterprise-mobility/](https://apis.io/providers/enterprise-mobility/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for Enterprise Mobility: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/enterprise-mobility/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
