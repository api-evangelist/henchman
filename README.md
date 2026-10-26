# Henchman (henchman)

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
