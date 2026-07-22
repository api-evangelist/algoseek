---
name: Resolve where a dataset lives (S3 and ArdaDB)
description: Map an AlgoSeek dataset to its S3 cloud-storage buckets, CSV layout, and ArdaDB database
  table with SQL columns
api: openapi/algoseek-cloudstorage-api-openapi.yml
operations:
- get_cloud_storages_public_api_v1_public_cloud_storage__get
- get_csv_columns_public_api_v1_public_csv_column__get
- get_database_tables_public_api_v1_public_database_table__get
- get_sql_columns_public_api_v1_public_sql_column__get
generated: '2026-07-22'
method: generated
---

AlgoSeek datasets are delivered from S3 flat-file buckets and mirrored into the ArdaDB (ClickHouse) cloud database. After authenticating, resolve a dataset's physical delivery surfaces:

1. **S3 delivery** — `GET /api/v1/public/cloud_storage/` (`get_cloud_storages_public_api_v1_public_cloud_storage__get`); each CloudStorage record `belongs_to` a dataset via `dataset_id` and describes the bucket layout.
2. **CSV layout** — `GET /api/v1/public/csv_column/` (`get_csv_columns_public_api_v1_public_csv_column__get`); CSVColumn rows (via `cloud_storage_id`) give the ordered flat-file column schema.
3. **ArdaDB table** — `GET /api/v1/public/database_table/` (`get_database_tables_public_api_v1_public_database_table__get`); DatabaseTable records (via `dataset_id`) name the ClickHouse table backing the dataset. Tables are also addressable by name: `/api/v1/public/database_table/table_name/{table_name}/`.
4. **SQL columns** — `GET /api/v1/public/sql_column/` (`get_sql_columns_public_api_v1_public_sql_column__get`); SQLColumn rows (via `table_id`) give the typed ArdaDB column schema.

To actually query ArdaDB, use the algoseek-connector Python library (`pip install algoseek-connector`) with ArdaDB credentials — the REST API serves catalog metadata only.
