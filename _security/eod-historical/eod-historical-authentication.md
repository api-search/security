---
api_key_in:
- query
api_specs:
- filename: openapi.yaml
  format: yaml
  label: EOD Historical Data Financial API
  slug: financial-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/EodHistoricalData/EODHD-openapi/main/openapi.yaml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Eod Historical Authentication
name_suffix: Authentication
oauth_flows: []
overview: EOD Historical Data secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: EOD Historical Data
provider_slug: eod-historical
scheme_count: 1
schemes:
- description: EODHD API key (stored as a secret in ChatGPT).
  in: query
  name: EODHDQueryKey
  parameter: api_token
  sources:
  - openapi/openapi.yaml
  type: apiKey
slug: eod-historical-authentication
source_filename: eod-historical-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/openapi.yaml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: EODHDQueryKey\n  type: apiKey\n  in: query\n  parameter: api_token\n  description: EODHD API key (stored as a secret in ChatGPT).\n  sources:\n  - openapi/openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/eod-historical/refs/heads/main/authentication/eod-historical-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Fintech
- Market Data
- Stocks
- ETF
- Fundamentals
- Options
- Forex
- Crypto
- Macroeconomic
- Technical Indicators
- News
- Sentiment
- Historical Data
---
