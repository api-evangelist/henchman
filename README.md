# Henchman (henchman)

Henchman is a legal knowledge and contract-drafting AI platform that surfaces a firm's own past clauses and definitions from its document management system directly inside Microsoft Word, Outlook, and Copilot. It connects to legal DMS platforms (iManage, NetDocuments, SharePoint, OneDrive, Google Drive, OpenText eDocs), extracts and ranks clauses and definitions, and adds a secure multi-LLM AI clause assistant on top. Henchman was acquired by LexisNexis in 2024 and is being integrated into Lexis+ AI and Lexis Create+. Henchman is delivered primarily as add-ins and DMS connectors; it does not publish a public developer API.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/henchman/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/henchman/refs/heads/main/apis.yml)

## API Availability

Henchman is an add-in and integration product, not a developer platform. It has internal application API endpoints (under `*.henchman.io`, covering Dashboard, Auth, Add-in, and API surfaces, as referenced in its public bug bounty scope) that power the Word/Outlook add-ins and DMS connectors, but **no public, documented developer API or API reference is published** as of this writing. The "developer surface" is the set of supported document management system integrations and the Microsoft 365 add-ins. The OpenAPI document in this repository therefore carries an empty `paths` object with an honest description rather than fabricated endpoints.

## Tags

- Legal
- Legal Tech
- Contract Drafting
- Clause Search
- Knowledge Management
- AI

## Timestamps

- **Created:** 2026-06-21
- **Modified:** 2026-06-21

## APIs

### Henchman Clause and Definition Search

Searches a firm's extracted clauses and definitions across its connected contract database, with intelligent ranking by frequency, document type, and metadata, surfaced inside Microsoft Word and Outlook. This capability is exposed through Henchman's add-ins and an internal application API; no public developer API or API reference is published.

- **Human URL:** [https://henchman.io/artificial-intelligence](https://henchman.io/artificial-intelligence)

#### Tags

- Clause Search
- Definition Search
- Legal

#### Properties

- [Documentation](https://help.henchman.io/home)
- [OpenAPI](openapi/henchman-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/henchman.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/henchman.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Henchman Knowledge Base

Builds and maintains a searchable knowledge layer over a firm's precedent contracts by extracting clauses and definitions into a structured store (the base package plus an optional Dynamic Knowledge add-on and AI Clause Assistant add-on). Access is via the Henchman product, not a published developer API.

- **Human URL:** [https://henchman.io/integrations](https://henchman.io/integrations)

#### Tags

- Knowledge Management
- Contract Data
- Legal

#### Properties

- [Documentation](https://help.henchman.io/home)
- [OpenAPI](openapi/henchman-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/henchman.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/henchman.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Henchman Integrations

Connects Henchman to document management and storage systems - iManage Cloud and On-Prem, NetDocuments, SharePoint, Microsoft OneDrive, Google Drive, and OpenText eDocs - to extract precedent contracts, plus Microsoft Word, Outlook, and Copilot surfaces. Integrations are configured via service accounts and documented setup guides rather than a self-serve public API.

- **Human URL:** [https://henchman.io/integrations](https://henchman.io/integrations)

#### Tags

- Integrations
- DMS
- iManage
- NetDocuments

#### Properties

- [Documentation](https://help.henchman.io/home/imanage-cloud-integration)
- [OpenAPI](openapi/henchman-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/henchman.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/henchman.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [LinkedIn](https://www.linkedin.com/company/henchman-io)
- [Website](https://www.henchman.io)
- [Documentation](https://help.henchman.io/home)
- [Plans](plans/henchman-plans-pricing.yml)
- [Rate Limits](rate-limits/henchman-rate-limits.yml)
- [Fin Ops](finops/henchman-finops.yml)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
