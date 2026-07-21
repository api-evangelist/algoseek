# AlgoSeek (algoseek)

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
