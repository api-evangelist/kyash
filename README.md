# Kyash

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
