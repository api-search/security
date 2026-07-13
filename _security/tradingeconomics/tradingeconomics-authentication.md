---
api_key_in:
- header
- query
api_specs:
- filename: tradingeconomics-openapi.yml
  format: yaml
  label: Trading Economics Indicators API
  slug: tradingeconomics-indicators-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tradingeconomics/refs/heads/main/openapi/tradingeconomics-openapi.yml
- filename: tradingeconomics-openapi.yml
  format: yaml
  label: Trading Economics Economic Calendar API
  slug: tradingeconomics-economic-calendar-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tradingeconomics/refs/heads/main/openapi/tradingeconomics-openapi.yml
- filename: tradingeconomics-openapi.yml
  format: yaml
  label: Trading Economics Markets API
  slug: tradingeconomics-markets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tradingeconomics/refs/heads/main/openapi/tradingeconomics-openapi.yml
- filename: tradingeconomics-openapi.yml
  format: yaml
  label: Trading Economics Forecasts API
  slug: tradingeconomics-forecasts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tradingeconomics/refs/heads/main/openapi/tradingeconomics-openapi.yml
- filename: tradingeconomics-openapi.yml
  format: yaml
  label: Trading Economics Historical API
  slug: tradingeconomics-historical-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tradingeconomics/refs/heads/main/openapi/tradingeconomics-openapi.yml
- filename: tradingeconomics-openapi.yml
  format: yaml
  label: Trading Economics Financials API
  slug: tradingeconomics-financials-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tradingeconomics/refs/heads/main/openapi/tradingeconomics-openapi.yml
- filename: tradingeconomics-asyncapi.yml
  format: yaml
  label: Trading Economics Streaming API
  slug: tradingeconomics-streaming-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/tradingeconomics/refs/heads/main/asyncapi/tradingeconomics-asyncapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Tradingeconomics Authentication
name_suffix: Authentication
oauth_flows: []
overview: Trading Economics secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Trading Economics
provider_slug: tradingeconomics
scheme_count: 2
schemes:
- description: API client credentials in `key:secret` format passed as the `c` query parameter. Obtain a key by subscribing to a plan at developer.tradingeconomics.com.
  in: query
  name: clientKeyQuery
  parameter: c
  sources:
  - openapi/tradingeconomics-openapi.yml
  type: apiKey
- description: API client credentials passed in the Authorization header.
  in: header
  name: clientKeyHeader
  parameter: Authorization
  sources:
  - openapi/tradingeconomics-openapi.yml
  type: apiKey
slug: tradingeconomics-authentication
source_filename: tradingeconomics-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/tradingeconomics-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  - query\nschemes:\n- name: clientKeyQuery\n  type: apiKey\n  in: query\n  parameter: c\n  description: API client credentials in `key:secret` format passed as the `c` query parameter.\n    Obtain a key by subscribing to a plan at developer.tradingeconomics.com.\n  sources:\n  - openapi/tradingeconomics-openapi.yml\n- name: clientKeyHeader\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: API client credentials passed in the Authorization header.\n  sources:\n  - openapi/tradingeconomics-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tradingeconomics/refs/heads/main/authentication/tradingeconomics-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Economic Indicators
- Interest Rates
- Macroeconomics
- Financial Data
- Economic Calendar
- Forecasts
- Markets
---
