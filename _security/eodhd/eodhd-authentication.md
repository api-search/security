---
api_key_in:
- query
api_specs:
- filename: eodhd-eod-historical-data-openapi.yml
  format: yaml
  label: EODHD End-Of-Day Historical Data API
  slug: eod-historical-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eodhd/refs/heads/main/openapi/eodhd-eod-historical-data-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Eodhd Authentication
name_suffix: Authentication
oauth_flows: []
overview: EODHD secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: EODHD
provider_slug: eodhd
scheme_count: 1
schemes:
- in: query
  name: apiToken
  parameter: api_token
  sources:
  - openapi/eodhd-eod-historical-data-openapi.yml
  type: apiKey
slug: eodhd-authentication
source_filename: eodhd-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/eodhd-eod-historical-data-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: apiToken\n  type: apiKey\n  in: query\n  parameter: api_token\n  sources:\n  - openapi/eodhd-eod-historical-data-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/eodhd/refs/heads/main/authentication/eodhd-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Financial
- Market Data
- Stock Options
- Stocks
---
