---
api_key_in:
- header
api_specs:
- filename: un-comtrade-bulk-download-api-openapi.yml
  format: yaml
  label: UN Comtrade Bulk Download API
  slug: un-comtrade-bulk-download-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/un-comtrade/refs/heads/main/openapi/un-comtrade-bulk-download-api-openapi.yml
- filename: un-comtrade-data-availability-api-openapi.yml
  format: yaml
  label: UN Comtrade Data Availability API
  slug: un-comtrade-data-availability-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/un-comtrade/refs/heads/main/openapi/un-comtrade-data-availability-api-openapi.yml
- filename: un-comtrade-final-trade-data-api-openapi.yml
  format: yaml
  label: UN Comtrade Final Trade Data API
  slug: un-comtrade-final-trade-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/un-comtrade/refs/heads/main/openapi/un-comtrade-final-trade-data-api-openapi.yml
- filename: un-comtrade-public-preview-api-openapi.yml
  format: yaml
  label: UN Comtrade Public Preview API
  slug: un-comtrade-public-preview-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/un-comtrade/refs/heads/main/openapi/un-comtrade-public-preview-api-openapi.yml
- filename: un-comtrade-reference-data-api-openapi.yml
  format: yaml
  label: UN Comtrade Reference Data API
  slug: un-comtrade-reference-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/un-comtrade/refs/heads/main/openapi/un-comtrade-reference-data-api-openapi.yml
- filename: un-comtrade-tariffline-data-api-openapi.yml
  format: yaml
  label: UN Comtrade Tariffline Data API
  slug: un-comtrade-tariffline-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/un-comtrade/refs/heads/main/openapi/un-comtrade-tariffline-data-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Un Comtrade Authentication
name_suffix: Authentication
oauth_flows: []
overview: UN Comtrade secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: UN Comtrade
provider_slug: un-comtrade
scheme_count: 1
schemes:
- description: API subscription key obtained after registering a free B2C account at https://comtradeplus.un.org/ and subscribing to the relevant API product.
  in: header
  name: ApiKeyHeader
  parameter: Ocp-Apim-Subscription-Key
  sources:
  - openapi/openapi.yml
  type: apiKey
slug: un-comtrade-authentication
source_filename: un-comtrade-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyHeader\n  type: apiKey\n  in: header\n  parameter: Ocp-Apim-Subscription-Key\n  description: API subscription key obtained after registering a free B2C account at https://comtradeplus.un.org/\n    and subscribing to the relevant API product.\n  sources:\n  - openapi/openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/un-comtrade/refs/heads/main/authentication/un-comtrade-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Trade
- International Trade
- Import
- Export
- Statistics
- United Nations
- Economics
- Commodities
- Bilateral Trade
- HS Codes
- SITC
---
