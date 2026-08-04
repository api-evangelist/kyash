# Kyash

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

Kyash Inc. (株式会社Kyash) is a Tokyo-based fintech founded in 2015 that operates a consumer mobile wallet and Visa prepaid card in Japan — charging, peer-to-peer transfers, shared accounts, buy-now-pay-later, personal finance management, and contactless payment via Apple Pay, Google Pay, and Samsung Pay. Kyash is a registered Funds Transfer Service Provider (Kanto Local Finance Bureau No. 00082) and third-party Prepaid Payment Instrument Issuer (No. 00698), and is ISO/IEC 27001:2022, PCI DSS, and TRUSTe certified.

Its business-facing product is **Kyash Payout**, a mass payout service that sends funds to Japanese domestic bank accounts or Kyash wallets at a flat ¥50 per transfer, integrated either by Zengin/CSV file upload or by direct API integration (including a balance API). Kyash previously sold **Kyash Direct**, an API-based Visa card issuer processing platform launched in 2019.

## API posture

Kyash's API access is **sales-gated**. As of the 2026-07-19 enrichment pass there is no public developer portal, API reference, OpenAPI/AsyncAPI specification, SDK, CLI, Postman collection, sandbox, or `/.well-known/` discovery surface. `developers.kyash.co`, `docs.kyash.co`, `api.kyash.co`, `status.kyash.co`, and `trust.kyash.co` do not resolve. The Kyash GitHub organization publishes first-party general-purpose open source (a Zengin bank-format Go library, `async-retry`, `ghlint`, Android/iOS UI components) but no API client libraries.

## Artifacts

- `apis.yml` — provider index, Kyash Payout API entry, link properties
- `lifecycle/` — versioning/deprecation posture and status channels
- `llms/` — generated `llms.txt`
- `packages/` — first-party open source (no API clients)
- `security/` — domain-security probe, trust and compliance posture
- `well-known/` — `/.well-known/` probe (no documents published)

Backed by: partech — https://kyash.co/
