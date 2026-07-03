# Stampli (stampli)

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
