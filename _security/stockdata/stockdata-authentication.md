---
api_key_in:
- query
api_specs:
- filename: stockdata-openapi.yml
  format: yaml
  label: StockData API
  slug: stockdata
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stockdata/refs/heads/main/openapi/stockdata-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Stockdata Authentication
name_suffix: Authentication
oauth_flows: []
overview: StockData secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: StockData
provider_slug: stockdata
scheme_count: 1
schemes:
- description: API token obtained from the StockData dashboard.
  in: query
  name: ApiToken
  parameter: api_token
  sources:
  - openapi/stockdata-openapi.yml
  type: apiKey
slug: stockdata-authentication
source_filename: stockdata-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/stockdata-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: ApiToken\n  type: apiKey\n  in: query\n  parameter: api_token\n  description: API token obtained from the StockData dashboard.\n  sources:\n  - openapi/stockdata-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/stockdata/refs/heads/main/authentication/stockdata-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Finance
- Financial Data
- Stock Market
- Market Data
- News
- Sentiment Analysis
---
