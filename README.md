# AlgoSeek (algoseek)

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

AlgoSeek, LLC is a New York-based financial market data vendor (spun off from a trading fund) selling historical intraday US market data - equities, ETFs, equity options with Greeks and IV, futures, futures options, and reference data (security masters, adjustment factors, IPOs, index components) - plus real-time feeds. Delivery is data-platform-first rather than API-first, through S3 flat-file buckets, the ArdaDB managed ClickHouse cloud database queried via the open-source algoseek-connector Python library, ultra-low-latency real-time feeds via colocated MultiCast/TCP, and a REST Metadata Services API with a public OpenAPI/Swagger surface. Sales-led commercially, with a customer console at console.algoseek.com.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/algoseek/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/algoseek/refs/heads/main/apis.yml)

## Tags

- Financial
- Market Data
- Stocks
- Options
- Futures
- Tick Data
- Reference Data
- Real-Time
- Trading

## Timestamps

- **Created:** 2026-07-21
- **Modified:** 2026-07-21

## APIs

### AlgoSeek Metadata Services API

FastAPI-based REST API (metadata-api v1.2) describing AlgoSeek's dataset catalog - data groups, datasets, pricing records, database objects and tables, cloud storage buckets, documentation, vendors, and sample data. Publishes a live Swagger UI and OpenAPI 3.0.2 document with 148 paths (56 public, 90 internal); endpoints require HTTP Bearer authentication obtained via `/api/v1/login/access_token/`. This is the metadata backend used by the algoseek-connector Python library.

- **Human URL:** [https://metadata-services.algoseek.com/docs](https://metadata-services.algoseek.com/docs)
- **Base URL:** `https://metadata-services.algoseek.com/api/v1`

#### Tags

- Metadata
- Datasets
- Reference Data
- Discovery

#### Properties

- [Documentation](https://metadata-services.algoseek.com/docs)
- [OpenAPI](openapi/algoseek-metadata-services-openapi.json) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)

### AlgoSeek ArdaDB Query Service

Managed ClickHouse-based columnar cloud database (AWS us-east-1) pre-loaded with two petabytes of AlgoSeek historical and near-real-time market data, queried with full SQL. Programmatic access is documented through the open-source algoseek-connector Python library (SQL-like method-chaining queries, pandas DataFrames, streaming results) using ArdaDB credentials; no public HTTP base URL is documented.

- **Human URL:** [https://algoseek.com/ardadb](https://algoseek.com/ardadb)

#### Tags

- Database
- SQL
- ClickHouse
- Historical Data

#### Properties

- [Documentation](https://algoseek.com/ardadb)
- [Documentation](https://algoseek-connector.readthedocs.io/)

## Common Properties

- [Website](https://algoseek.com/)
- [Portal](https://console.algoseek.com/)
- [Documentation](https://algoseek-connector.readthedocs.io/)
- [GitHub Organization](https://github.com/algoseekgit)
- [LinkedIn](https://www.linkedin.com/company/algoseek)
- [Blog](https://algoseek.com/blog)
- [Plans](https://algoseek.com/financial-data/packages)
- [Sign Up](https://console.algoseek.com/auth/register)
- [Support](https://algoseek.com/contact-us)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
