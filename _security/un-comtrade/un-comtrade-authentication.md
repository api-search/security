---
api_key_in:
- header
api_specs:
- filename: openapi.yaml
  format: yaml
  label: UN Comtrade Data API
  slug: un-comtrade-data-api
  spec_type: OpenAPI
  url: https://comtradedeveloper.un.org/
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
