# AlgoSeek

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

**Areas:** Finance · Market Data · Stocks · Options · Futures · Tick Data · Reference Data · Real-Time · Trading

## AlgoSeek on APIs.io

Everything profiled for AlgoSeek is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/algoseek/](https://apis.io/providers/algoseek/)** — or go straight to one of the APIs or properties below.

### APIs (34)

- [AlgoSeek ArdaDB Query Service](https://apis.io/apis/algoseek/algoseek-ardadb-query-service/) — Managed ClickHouse-based columnar cloud database (AWS us-east-1) pre-loaded with two petabytes of AlgoSeek historical and near-real-time market data,…
- [AlgoSeek AWSAccount API](https://apis.io/apis/algoseek/algoseek-awsaccount-api/) — The AWSAccount API from AlgoSeek — 3 operation(s) for awsaccount.
- [AlgoSeek AWSResourceType API](https://apis.io/apis/algoseek/algoseek-awsresourcetype-api/) — The AWSResourceType API from AlgoSeek — 3 operation(s) for awsresourcetype.
- [AlgoSeek BucketGroup API](https://apis.io/apis/algoseek/algoseek-bucketgroup-api/) — The BucketGroup API from AlgoSeek — 7 operation(s) for bucketgroup.
- [AlgoSeek BucketMonitoring API](https://apis.io/apis/algoseek/algoseek-bucketmonitoring-api/) — The BucketMonitoring API from AlgoSeek — 2 operation(s) for bucketmonitoring.
- [AlgoSeek BucketSource API](https://apis.io/apis/algoseek/algoseek-bucketsource-api/) — The BucketSource API from AlgoSeek — 3 operation(s) for bucketsource.
- [AlgoSeek BucketUpdate API](https://apis.io/apis/algoseek/algoseek-bucketupdate-api/) — The BucketUpdate API from AlgoSeek — 4 operation(s) for bucketupdate.
- [AlgoSeek CSVColumn API](https://apis.io/apis/algoseek/algoseek-csvcolumn-api/) — The CSVColumn API from AlgoSeek — 4 operation(s) for csvcolumn.
- [AlgoSeek DatabaseObject API](https://apis.io/apis/algoseek/algoseek-databaseobject-api/) — The DatabaseObject API from AlgoSeek — 7 operation(s) for databaseobject.
- [AlgoSeek DatabaseTable API](https://apis.io/apis/algoseek/algoseek-databasetable-api/) — The DatabaseTable API from AlgoSeek — 7 operation(s) for databasetable.
- [AlgoSeek DataClass API](https://apis.io/apis/algoseek/algoseek-dataclass-api/) — The DataClass API from AlgoSeek — 5 operation(s) for dataclass.
- [AlgoSeek DataFormat API](https://apis.io/apis/algoseek/algoseek-dataformat-api/) — The DataFormat API from AlgoSeek — 5 operation(s) for dataformat.
- [AlgoSeek DataGroup API](https://apis.io/apis/algoseek/algoseek-datagroup-api/) — The DataGroup API from AlgoSeek — 5 operation(s) for datagroup.
- [AlgoSeek DataGroupPricing API](https://apis.io/apis/algoseek/algoseek-datagrouppricing-api/) — The DataGroupPricing API from AlgoSeek — 4 operation(s) for datagrouppricing.
- [AlgoSeek Dataset API](https://apis.io/apis/algoseek/algoseek-dataset-api/) — The Dataset API from AlgoSeek — 10 operation(s) for dataset.
- [AlgoSeek DatasetChange API](https://apis.io/apis/algoseek/algoseek-datasetchange-api/) — The DatasetChange API from AlgoSeek — 2 operation(s) for datasetchange.
- [AlgoSeek DataType API](https://apis.io/apis/algoseek/algoseek-datatype-api/) — The DataType API from AlgoSeek — 5 operation(s) for datatype.
- [AlgoSeek DBObjectType API](https://apis.io/apis/algoseek/algoseek-dbobjecttype-api/) — The DBObjectType API from AlgoSeek — 5 operation(s) for dbobjecttype.
- [AlgoSeek DeliveryMethod API](https://apis.io/apis/algoseek/algoseek-deliverymethod-api/) — The DeliveryMethod API from AlgoSeek — 5 operation(s) for deliverymethod.
- [AlgoSeek Documentation API](https://apis.io/apis/algoseek/algoseek-documentation-api/) — The Documentation API from AlgoSeek — 5 operation(s) for documentation.
- [AlgoSeek Identity API](https://apis.io/apis/algoseek/algoseek-identity-api/) — The Identity API from AlgoSeek — 2 operation(s) for identity.
- [AlgoSeek Login API](https://apis.io/apis/algoseek/algoseek-login-api/) — The Login API from AlgoSeek — 1 operation(s) for login.
- [AlgoSeek Person API](https://apis.io/apis/algoseek/algoseek-person-api/) — The Person API from AlgoSeek — 4 operation(s) for person.
- [AlgoSeek Region API](https://apis.io/apis/algoseek/algoseek-region-api/) — The Region API from AlgoSeek — 5 operation(s) for region.
- [AlgoSeek S3Object API](https://apis.io/apis/algoseek/algoseek-s3object-api/) — The S3Object API from AlgoSeek — 5 operation(s) for s3object.
- [AlgoSeek SQLColumn API](https://apis.io/apis/algoseek/algoseek-sqlcolumn-api/) — The SQLColumn API from AlgoSeek — 4 operation(s) for sqlcolumn.
- [AlgoSeek Status API](https://apis.io/apis/algoseek/algoseek-status-api/) — The Status API from AlgoSeek — 5 operation(s) for status.
- [AlgoSeek StorageType API](https://apis.io/apis/algoseek/algoseek-storagetype-api/) — The StorageType API from AlgoSeek — 5 operation(s) for storagetype.
- [AlgoSeek TimeGranularity API](https://apis.io/apis/algoseek/algoseek-timegranularity-api/) — The TimeGranularity API from AlgoSeek — 5 operation(s) for timegranularity.
- [AlgoSeek TTLPeriodType API](https://apis.io/apis/algoseek/algoseek-ttlperiodtype-api/) — The TTLPeriodType API from AlgoSeek — 5 operation(s) for ttlperiodtype.
- [AlgoSeek Vendor API](https://apis.io/apis/algoseek/algoseek-vendor-api/) — The Vendor API from AlgoSeek — 4 operation(s) for vendor.
- [AlgoSeek Cloud Storage API](https://apis.io/apis/algoseek/algoseek-cloud-storage-api/) — The Cloud Storage API from AlgoSeek — 6 operation(s) for cloud storage.
- [AlgoSeek Health Check API](https://apis.io/apis/algoseek/algoseek-health-check-api/) — The Health Check API from AlgoSeek — 1 operation(s) for health check.
- [AlgoSeek Sample Data API](https://apis.io/apis/algoseek/algoseek-sample-data-api/) — The Sample Data API from AlgoSeek — 5 operation(s) for sample data.

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### MCP servers (1)

Model Context Protocol servers that expose the API to agents.

- [algoseek-metadata-services](https://apis.io/servers/algoseek/algoseek-metadata-services/)

#### Collections (33)

Postman and Open Collection request collections.

- [metadata-api AWSAccount API](https://apis.io/collections/algoseek/open-algoseek-awsaccount-api/)
- [metadata-api AWSAccount AWSResourceType API](https://apis.io/collections/algoseek/open-algoseek-awsresourcetype-api/)
- [metadata-api AWSAccount BucketGroup API](https://apis.io/collections/algoseek/open-algoseek-bucketgroup-api/)
- [metadata-api AWSAccount BucketMonitoring API](https://apis.io/collections/algoseek/open-algoseek-bucketmonitoring-api/)
- [metadata-api AWSAccount BucketSource API](https://apis.io/collections/algoseek/open-algoseek-bucketsource-api/)
- [metadata-api AWSAccount BucketUpdate API](https://apis.io/collections/algoseek/open-algoseek-bucketupdate-api/)
- [metadata-api AWSAccount CloudStorage API](https://apis.io/collections/algoseek/open-algoseek-cloudstorage-api/)
- [metadata-api AWSAccount CSVColumn API](https://apis.io/collections/algoseek/open-algoseek-csvcolumn-api/)
- [metadata-api AWSAccount DatabaseObject API](https://apis.io/collections/algoseek/open-algoseek-databaseobject-api/)
- [metadata-api AWSAccount DatabaseTable API](https://apis.io/collections/algoseek/open-algoseek-databasetable-api/)
- [metadata-api AWSAccount DataClass API](https://apis.io/collections/algoseek/open-algoseek-dataclass-api/)
- [metadata-api AWSAccount DataFormat API](https://apis.io/collections/algoseek/open-algoseek-dataformat-api/)
- [metadata-api AWSAccount DataGroup API](https://apis.io/collections/algoseek/open-algoseek-datagroup-api/)
- [metadata-api AWSAccount DataGroupPricing API](https://apis.io/collections/algoseek/open-algoseek-datagrouppricing-api/)
- [metadata-api AWSAccount Dataset API](https://apis.io/collections/algoseek/open-algoseek-dataset-api/)
- [metadata-api AWSAccount DatasetChange API](https://apis.io/collections/algoseek/open-algoseek-datasetchange-api/)
- [metadata-api AWSAccount DataType API](https://apis.io/collections/algoseek/open-algoseek-datatype-api/)
- [metadata-api AWSAccount DBObjectType API](https://apis.io/collections/algoseek/open-algoseek-dbobjecttype-api/)
- [metadata-api AWSAccount DeliveryMethod API](https://apis.io/collections/algoseek/open-algoseek-deliverymethod-api/)
- [metadata-api AWSAccount Documentation API](https://apis.io/collections/algoseek/open-algoseek-documentation-api/)
- [metadata-api AWSAccount Healthcheck API](https://apis.io/collections/algoseek/open-algoseek-healthcheck-api/)
- [metadata-api AWSAccount Identity API](https://apis.io/collections/algoseek/open-algoseek-identity-api/)
- [metadata-api AWSAccount Login API](https://apis.io/collections/algoseek/open-algoseek-login-api/)
- [metadata-api AWSAccount Person API](https://apis.io/collections/algoseek/open-algoseek-person-api/)
- [metadata-api AWSAccount Region API](https://apis.io/collections/algoseek/open-algoseek-region-api/)
- …and 8 more published on APIs.io

#### Overlays (33)

OpenAPI overlays, including conversational phrasing for each operation.

- [Algoseek Awsaccount Api Overlay](https://apis.io/overlays/algoseek/algoseek-awsaccount-api-overlay/)
- [Algoseek Awsresourcetype Api Overlay](https://apis.io/overlays/algoseek/algoseek-awsresourcetype-api-overlay/)
- [Algoseek Bucketgroup Api Overlay](https://apis.io/overlays/algoseek/algoseek-bucketgroup-api-overlay/)
- [Algoseek Bucketmonitoring Api Overlay](https://apis.io/overlays/algoseek/algoseek-bucketmonitoring-api-overlay/)
- [Algoseek Bucketsource Api Overlay](https://apis.io/overlays/algoseek/algoseek-bucketsource-api-overlay/)
- [Algoseek Bucketupdate Api Overlay](https://apis.io/overlays/algoseek/algoseek-bucketupdate-api-overlay/)
- [Algoseek Cloudstorage Api Overlay](https://apis.io/overlays/algoseek/algoseek-cloudstorage-api-overlay/)
- [Algoseek Csvcolumn Api Overlay](https://apis.io/overlays/algoseek/algoseek-csvcolumn-api-overlay/)
- [Algoseek Databaseobject Api Overlay](https://apis.io/overlays/algoseek/algoseek-databaseobject-api-overlay/)
- [Algoseek Databasetable Api Overlay](https://apis.io/overlays/algoseek/algoseek-databasetable-api-overlay/)
- [Algoseek Dataclass Api Overlay](https://apis.io/overlays/algoseek/algoseek-dataclass-api-overlay/)
- [Algoseek Dataformat Api Overlay](https://apis.io/overlays/algoseek/algoseek-dataformat-api-overlay/)
- [Algoseek Datagroup Api Overlay](https://apis.io/overlays/algoseek/algoseek-datagroup-api-overlay/)
- [Algoseek Datagrouppricing Api Overlay](https://apis.io/overlays/algoseek/algoseek-datagrouppricing-api-overlay/)
- [Algoseek Dataset Api Overlay](https://apis.io/overlays/algoseek/algoseek-dataset-api-overlay/)
- [Algoseek Datasetchange Api Overlay](https://apis.io/overlays/algoseek/algoseek-datasetchange-api-overlay/)
- [Algoseek Datatype Api Overlay](https://apis.io/overlays/algoseek/algoseek-datatype-api-overlay/)
- [Algoseek Dbobjecttype Api Overlay](https://apis.io/overlays/algoseek/algoseek-dbobjecttype-api-overlay/)
- [Algoseek Deliverymethod Api Overlay](https://apis.io/overlays/algoseek/algoseek-deliverymethod-api-overlay/)
- [Algoseek Documentation Api Overlay](https://apis.io/overlays/algoseek/algoseek-documentation-api-overlay/)
- [Algoseek Healthcheck Api Overlay](https://apis.io/overlays/algoseek/algoseek-healthcheck-api-overlay/)
- [Algoseek Identity Api Overlay](https://apis.io/overlays/algoseek/algoseek-identity-api-overlay/)
- [Algoseek Login Api Overlay](https://apis.io/overlays/algoseek/algoseek-login-api-overlay/)
- [Algoseek Person Api Overlay](https://apis.io/overlays/algoseek/algoseek-person-api-overlay/)
- [Algoseek Region Api Overlay](https://apis.io/overlays/algoseek/algoseek-region-api-overlay/)
- …and 8 more published on APIs.io

#### Security (2)

Authentication, trust centre, and vulnerability disclosure.

- [Algoseek Authentication](https://apis.io/security/algoseek/algoseek-authentication/)
- [Algoseek Domain Security](https://apis.io/security/algoseek/algoseek-domain-security/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://algoseek.com/)
- [Documentation](https://algoseek-connector.readthedocs.io/)
- [Getting started](https://algoseek-connector.readthedocs.io/en/latest/algoseek_connector/tutorials.html)
- [API reference](https://metadata-services.algoseek.com/docs)
- [Sign up](https://console.algoseek.com/auth/register)
- [Support](https://algoseek.com/contact-us)
- [Changelog](https://github.com/algoseekgit/algoseek-connector/blob/master/CHANGELOG.md)
- [Blog](https://algoseek.com/blog/)
- [Terms of service](https://algoseek.com/terms-of-use)
- [Privacy policy](https://algoseek.com/privacy-cookies)
- [GitHub](https://github.com/algoseekgit)

## API Evangelist rating

**Kin Score 39.3** — developing · rubric 0.25.0 · scored 2026-10-23

| Facet | Score |
|---|---|
| Discoverability | 73.2 |
| Contract quality | 47.6 |
| Contract governance | 4.5 |
| Operational transparency | 18.4 |
| Developer ergonomics | 66.1 |
| Access clarity | 21.1 |

**Agent readiness 20.9** — agent-aware

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | yes |
| Agentic Access | — |
| Reversibility Documented | — |
| MCP Server | — |
| Auth Clarity | bearer (partial credit) |
| Idempotency | — |
| Error Semantics | verified |
| OpenAPI Examples | — |
| Rate Limit Signal | — |
| Event Surface Described | — |
| Agent Skills | derived (partial credit) |
| Well Known Catalog | — |
| Consent Identity | — |
| Agent Card | — |
| Dry Run Mode | — |
| Delegated Identity | — |
| Protected Resource Metadata | — |
| Dynamic Client Registration | — |
| Agentic Commerce | — |
| Pagination Ratio | — |
| Operation Distinctiveness | — |

**Regulatory alignment 23.1** — Securities & Market Data

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/algoseek/](https://apis.io/providers/algoseek/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for AlgoSeek: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/algoseek/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
