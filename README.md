# Enterprise Mobility (enterprise-mobility)

Enterprise Mobility is the Clayton, Missouri parent of Enterprise Rent-A-Car, National Car Rental and Alamo Rent a Car, and the largest car rental provider in the world — 90,000+ team members, 9,500+ rental branches across more than 90 countries and territories, a global fleet of over 2.4 million vehicles and $39 billion in 2025 fiscal-year revenue. Beyond leisure and corporate car rental it operates fleet management, flexible vehicle hire, carsharing, vanpooling, truck rental, car sales, vehicle subscription and the ARMS / Entegral replacement-rental technology used by insurers, collision repairers and dealerships. In the United States travel distribution chain it is a ground-transportation supplier whose inventory reaches buyers through GDS and OTA intermediaries, corporate travel programs and its own direct brand sites, rather than through any published public booking API. Its API posture is partner-gated and honestly so: EHI runs a real API Marketplace at developer.ehi.com with public marketing overviews for three business lines — Rental, Replacement Rental and Commute — but the API catalog, API specs, guides and release notes all sit behind Azure AD B2C sign-in and the portal states access is for "an Enterprise employee or trusted Partner" who should "contact your account manager ... to request access". No OpenAPI, no base URL and no endpoint is published publicly; probes of /openapi.json, /swagger.json, /api-docs and /.well-known/ return AEM soft-404 HTML or 404. The published API License Agreement grants only a "limited, revocable, non-transferable, non-sublicensable, non-exclusive" right, restricts use to the licensee's internal purpose, states the licensee has no ownership rights in Renter Information, and on termination requires the licensee to "delete or return any copies of the APIs and Enterprise Content" — public docs shell, gated specs, no exit path.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/enterprise-mobility/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/enterprise-mobility/refs/heads/main/apis.yml)

## Tags

- Travel
- United States
- Car Rental
- Ground Transportation
- Mobility
- Corporate Travel
- Distribution
- Fleet Management
- Insurance Replacement Rental
- Booking

## Timestamps

- **Created:** 2026-07-28
- **Modified:** 2026-07-28

## APIs

### EHI Rental APIs

The Rental business line of the EHI API Marketplace, covering Enterprise Rent-A-Car's network of neighborhood and airport branches. The public overview page describes the capabilities as vehicle rental beyond traditional car rental and directs prospective consumers to register as an Enterprise employee or trusted Partner to shop the API catalog. No API names, base URL, endpoints, authentication scheme or specification are published outside the Azure AD B2C sign-in.

- **Human URL:** [https://developer.ehi.com/apis-overview/rental.html](https://developer.ehi.com/apis-overview/rental.html)
- **Base URL:** none published

#### Tags

- Car Rental
- Reservations
- Travel

#### Properties

- [Documentation](https://developer.ehi.com/apis-overview/rental.html)
- [Portal](https://developer.ehi.com/)
- [Website](https://www.enterprise.com/en/home.html)
- [Terms of Service](https://developer.ehi.com/general/terms-of-use.html)

### EHI Replacement Rental APIs

The Replacement Rental business line of the EHI API Marketplace, exposing the ARMS (Automated Rental Management System) and Entegral platforms to insurance providers, collision repair shops, dealership partners and fleet maintenance companies. The public overview page segments the capability set into three groups — Communication, Lifecycle and Data — and closes with "Note: Contact your account manager for more information and to request access." No specification, base URL or endpoint is published publicly.

- **Human URL:** [https://developer.ehi.com/apis-overview/replacement-rental.html](https://developer.ehi.com/apis-overview/replacement-rental.html)
- **Base URL:** none published

#### Tags

- Replacement Rental
- Insurance
- Collision Repair
- Claims

#### Properties

- [Documentation](https://developer.ehi.com/apis-overview/replacement-rental.html)
- [Portal](https://developer.ehi.com/)
- [Website](https://www.entegral.com/)
- [Terms of Service](https://developer.ehi.com/general/terms-of-use.html)

### EHI Commute APIs

The Commute business line of the EHI API Marketplace, covering Commute with Enterprise vanpooling and rideshare-to-work programs sold to employers. The public overview page describes the capability as APIs that "manage the process and create better experiences for your riders". No API names, base URL, endpoints or specification are published outside the gated catalog.

- **Human URL:** [https://developer.ehi.com/apis-overview/commute.html](https://developer.ehi.com/apis-overview/commute.html)
- **Base URL:** none published

#### Tags

- Vanpool
- Rideshare
- Commute
- Corporate Travel

#### Properties

- [Documentation](https://developer.ehi.com/apis-overview/commute.html)
- [Portal](https://developer.ehi.com/)
- [Terms of Service](https://developer.ehi.com/general/terms-of-use.html)

## Common Properties

- [Website](https://www.enterprisemobility.com/)
- [Portal](https://developer.ehi.com/)
- [Documentation](https://developer.ehi.com/dashboard/get-started.html)
- [Terms of Service](https://developer.ehi.com/general/terms-of-use.html)
- [Privacy Policy](https://developer.ehi.com/general/privacy-policy.html)
- [Contact](https://developer.ehi.com/general/contact-us.html)
- [LinkedIn](https://www.linkedin.com/company/enterprise-mobility)

## Switching Cost

Recorded in full in [review.yml](review.yml).

- **Interface shape:** `proprietary-undocumented` — no spec, base URL, endpoint or auth scheme is public. The one real open-standard signal is CIECA BMS on the Entegral/ARMS collision-claims side, asserted by CIECA rather than published by Enterprise. No OpenTravel conformance claim anywhere.
- **Second source:** `alternatives-with-migration` — Sixt publishes a genuinely public developer portal; Hertz, Avis Budget and Europcar publish none that resolves; aggregators (CarTrawler, Amadeus Cars, Sabre Cars, Travelport) substitute for the supplier relationship. For insurers on ARMS/Entegral the picture is closer to few-alternatives.
- **Exit path:** `no-export-published` — and worse than absent. Section 15 of the API License Agreement requires the licensee to "delete or return any copies of the APIs and Enterprise Content" on termination, and Section 1 denies the licensee any ownership rights in Renter Information.
- **Identifier portability:** nothing published. No IATA/ARC, ACRISS/SIPP, airport or GDS vendor codes are named in Enterprise's own material; assume vendor-internal opaque ARMS/Entegral identifiers behind the gate.
- **Contractual lock-in:** API License Agreement v1.0, effective 18 October 2022 — a "limited, revocable, non-transferable, non-sublicensable, non-exclusive" grant, internal use only unless Enterprise authorizes otherwise, redistribution "strictly forbidden", no uptime guarantee, quotas set at Enterprise's discretion, 30 days' written notice to leave versus termination by Enterprise "for any reason or no reason ... without notice".
- **Distribution model:** `gds-intermediated` — a supplier, not a distributor. No public booking, shopping or rate API.
- **NDC posture:** not applicable (car rental, not an airline).
- **Access gate:** `partner-only` — Azure AD B2C registration is self-serve, but the catalog requires being "an Enterprise employee or trusted Partner", an account manager's approval, click-acceptance of the API License Agreement binding your employer, and an annual third-party security audit obligation on request.
