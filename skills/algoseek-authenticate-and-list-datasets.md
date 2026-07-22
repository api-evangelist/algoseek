---
name: Authenticate and list AlgoSeek datasets
description: Obtain a bearer token from the Metadata Services API and enumerate the public dataset catalog
api: openapi/algoseek-dataset-api-openapi.yml
operations:
- apps_access_token_api_v1_login_access_token__post
- get_datasets_public_api_v1_public_dataset__get
- get_dataset_public_api_v1_public_dataset__dataset_id___get
- get_dataset_by_text_id_public_api_v1_public_dataset_text_id__text_id___get
generated: '2026-07-22'
method: generated
---

Use the AlgoSeek Metadata Services API (base `https://metadata-services.algoseek.com/api/v1`) to browse the dataset catalog.

1. **Authenticate** — `POST /api/v1/login/access_token/` (operation `apps_access_token_api_v1_login_access_token__post`) with a JSON `AppsTokenQuery` body containing your AlgoSeek credentials. The `Token` response carries the bearer token. There is no OAuth flow and no self-serve API key: credentials come from your AlgoSeek account (sales-led onboarding via https://console.algoseek.com/).
2. **Send the token** on every call as `Authorization: Bearer <token>` (securityScheme `HTTPBearer`).
3. **List datasets** — `GET /api/v1/public/dataset/` (`get_datasets_public_api_v1_public_dataset__get`). There is no pagination; the collection returns in full.
4. **Fetch one dataset** — by numeric id `GET /api/v1/public/dataset/{dataset_id}/` (`get_dataset_public_api_v1_public_dataset__dataset_id___get`) or by stable text id `GET /api/v1/public/dataset/text_id/{text_id}/` (`get_dataset_by_text_id_public_api_v1_public_dataset_text_id__text_id___get`). Dataset `text_id` values match the slugs on https://algoseek.com/data-sets/details/ pages (e.g. `eq_taq_1min`).

Errors: the contract declares only `422` (`HTTPValidationError` with a `detail[]` list); auth failures are undeclared in the spec. No idempotency keys and no documented rate limits — see conventions/algoseek-conventions.yml.
