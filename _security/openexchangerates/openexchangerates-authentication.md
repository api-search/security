---
api_key_in:
- header
- query
api_specs:
- filename: openexchangerates-openapi.yml
  format: yaml
  label: Open Exchange Rates Latest Rates API
  slug: openexchangerates-latest-rates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openexchangerates/refs/heads/main/openapi/openexchangerates-openapi.yml
- filename: openexchangerates-openapi.yml
  format: yaml
  label: Open Exchange Rates Historical Rates API
  slug: openexchangerates-historical-rates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openexchangerates/refs/heads/main/openapi/openexchangerates-openapi.yml
- filename: openexchangerates-openapi.yml
  format: yaml
  label: Open Exchange Rates Time Series API
  slug: openexchangerates-time-series-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openexchangerates/refs/heads/main/openapi/openexchangerates-openapi.yml
- filename: openexchangerates-openapi.yml
  format: yaml
  label: Open Exchange Rates Convert API
  slug: openexchangerates-convert-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openexchangerates/refs/heads/main/openapi/openexchangerates-openapi.yml
- filename: openexchangerates-openapi.yml
  format: yaml
  label: Open Exchange Rates Currencies API
  slug: openexchangerates-currencies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openexchangerates/refs/heads/main/openapi/openexchangerates-openapi.yml
- filename: openexchangerates-openapi.yml
  format: yaml
  label: Open Exchange Rates OHLC API
  slug: openexchangerates-ohlc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openexchangerates/refs/heads/main/openapi/openexchangerates-openapi.yml
- filename: openexchangerates-openapi.yml
  format: yaml
  label: Open Exchange Rates Usage API
  slug: openexchangerates-usage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openexchangerates/refs/heads/main/openapi/openexchangerates-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Openexchangerates Authentication
name_suffix: Authentication
oauth_flows: []
overview: Open Exchange Rates secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Open Exchange Rates
provider_slug: openexchangerates
scheme_count: 2
schemes:
- description: Your unique App ID, passed as a query parameter.
  in: query
  name: appIdQuery
  parameter: app_id
  sources:
  - openapi/openexchangerates-openapi.yml
  type: apiKey
- description: 'Your unique App ID, passed as a header: Authorization: Token YOUR_APP_ID.'
  in: header
  name: appIdHeader
  parameter: Authorization
  sources:
  - openapi/openexchangerates-openapi.yml
  type: apiKey
slug: openexchangerates-authentication
source_filename: openexchangerates-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/openexchangerates-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  - query\nschemes:\n- name: appIdQuery\n  type: apiKey\n  in: query\n  parameter: app_id\n  description: Your unique App ID, passed as a query parameter.\n  sources:\n  - openapi/openexchangerates-openapi.yml\n- name: appIdHeader\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: 'Your unique App ID, passed as a header: Authorization: Token YOUR_APP_ID.'\n  sources:\n  - openapi/openexchangerates-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/openexchangerates/refs/heads/main/authentication/openexchangerates-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Foreign Exchange
- Currency
- Exchange Rates
- FX
- Currency Conversion
- Forex
- Financial Data
---
