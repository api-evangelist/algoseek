---
name: Browse data groups, pricing, and documentation
description: 'Walk the AlgoSeek catalog hierarchy: data groups, their pricing records, and dataset documentation'
api: openapi/algoseek-datagroup-api-openapi.yml
operations:
- get_data_groups_public_api_v1_public_data_group__get
- get_data_group_public_api_v1_public_data_group__data_group_id___get
- get_data_group_pricings_public_api_v1_public_data_group_pricing__get
- get_documentations_public_api_v1_public_documentation__get
generated: '2026-07-22'
method: generated
---

After authenticating (see the authenticate-and-list-datasets skill), walk the catalog hierarchy.

1. **List data groups** — `GET /api/v1/public/data_group/` (`get_data_groups_public_api_v1_public_data_group__get`). A data group (e.g. US Equity Market Data) bundles datasets; each group carries `status_id`, `region_id`, and `pricing_id`.
2. **Fetch a group** — `GET /api/v1/public/data_group/{data_group_id}/` (`get_data_group_public_api_v1_public_data_group__data_group_id___get`).
3. **Resolve pricing records** — `GET /api/v1/public/data_group_pricing/` (`get_data_group_pricings_public_api_v1_public_data_group_pricing__get`) and match `pricing_id`. Pricing is catalog metadata; actual purchase is sales-led (https://algoseek.com/financial-data/packages).
4. **Fetch documentation entries** — `GET /api/v1/public/documentation/` (`get_documentations_public_api_v1_public_documentation__get`); each record points at S3-hosted dataset documentation and maps to datasets via the dataset `documentation_id`.

Lookup tables (`data_class`, `data_type`, `data_format`, `time_granularity`, `region`, `status`) each have matching `/api/v1/public/<resource>/` list + get operations to decode the id fields — see data-model/algoseek-data-model.yml for the full entity graph.
