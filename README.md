# Stampli (stampli)

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

Stampli is an AI-driven accounts payable (AP) and procure-to-pay automation platform. It automates invoice capture and coding, approval workflows, vendor management, payments, and corporate cards, while staying aligned to a customer's ERP as the system of record.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/stampli/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/stampli/refs/heads/main/apis.yml)

## API Access Model — No Public Developer API

**Stampli does not offer a public, self-serve developer API.** This catalog entry is an honest, sourced stub documenting that fact.

What Stampli refers to as its "API" is **not** a developer-facing product. It is a set of **pre-built, in-house integrations** that Stampli builds, operates, and maintains itself:

- **API integration (cloud-to-cloud):** Managed connectors that auto-sync master data between Stampli and cloud ERPs such as NetSuite, Sage Intacct, and QuickBooks Online.
- **Bridge integration (cloud-to-on-premises):** An executable application that moves data between on-premises ERP applications (e.g., SAP S/4HANA, Sage 100) and Stampli.
- **File integration:** Templated file-based sync for ERPs where no API or Bridge connector exists.

Stampli explicitly states its integrations are "built in-house" by its own engineering team rather than relying on third-party connectors or developers. There is:

- **No developer portal.** `developer.stampli.com` does not resolve.
- **No published API reference, OpenAPI/Swagger document, or endpoint list** on Stampli's own properties.
- **No self-service authentication, API keys, or sandbox** documented publicly.
- **No documented webhooks, REST, GraphQL, or WebSocket surface** available to third parties.

Access to any programmatic data flow is **gated behind a sales and onboarding relationship**; Stampli configures the ERP sync on the customer's behalf. Third-party API tracker sites list speculative "OpenAPI/webhook/auth" capability flags for Stampli, but none are corroborated by a public Stampli developer resource, so they are not treated as confirmed here.

### Logical data objects (integration-only, not an open API)

Even though there is no public API, Stampli's managed integrations move a well-understood set of AP/procure-to-pay objects between the ERP and Stampli. These are documented here as **modeled, not confirmed** endpoints, because Stampli exposes no public reference for them:

- Invoices (capture, coding, custom fields)
- Vendors / vendor master data
- Purchase Orders (2- and 3-way matching, line items)
- GL Accounts and coding/dimension fields
- Locations / Entities (master lists)
- Approvals / approval workflows
- Payments and corporate cards

## Tags

- Accounts Payable
- AP Automation
- Procure-to-Pay
- Invoice Management
- Vendor Management
- ERP Integration
- FinTech
- No Public API
- Gated API

## Timestamps

- **Created:** 2026-07-03
- **Modified:** 2026-07-03

## Pricing

Stampli does not publish list pricing. Cost is quote-based and varies by invoice volume, number of users, and modules selected; buyers must contact Stampli sales for a quote. Implementation/onboarding is a separate cost. See [https://www.stampli.com/pricing/](https://www.stampli.com/pricing/).

## Common Properties

- [Website](https://www.stampli.com)
- [LinkedIn](https://www.linkedin.com/company/stampli)
- [Integrations](https://www.stampli.com/stampli-integrations/)
- [Documentation (ERP integration overview)](https://www.stampli.com/accounting-systems-erps/)
- [Pricing](https://www.stampli.com/pricing/)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com

## Sources

- Stampli Integrations — https://www.stampli.com/stampli-integrations/ (integrations built in-house; API/Bridge/File models; no developer API or portal mentioned)
- Stampli ERP integrations (70+ systems) — https://www.stampli.com/accounting-systems-erps/ (pre-built cloud-to-cloud API and Bridge integrations, managed by Stampli)
- Stampli Pricing — https://www.stampli.com/pricing/ (quote-based, contact sales)
- Stampli on LinkedIn — https://www.linkedin.com/company/stampli
- `developer.stampli.com` — does not resolve (no developer portal), verified 2026-07-03
