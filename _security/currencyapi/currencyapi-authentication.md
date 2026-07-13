---
api_key_in:
- header
- query
api_specs:
- filename: currencyapi-openapi.yml
  format: yaml
  label: CurrencyAPI Latest Exchange Rates API
  slug: currencyapi-latest-exchange-rates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/currencyapi/refs/heads/main/openapi/currencyapi-openapi.yml
- filename: currencyapi-openapi.yml
  format: yaml
  label: CurrencyAPI Historical Exchange Rates API
  slug: currencyapi-historical-exchange-rates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/currencyapi/refs/heads/main/openapi/currencyapi-openapi.yml
- filename: currencyapi-openapi.yml
  format: yaml
  label: CurrencyAPI Range Exchange Rates API
  slug: currencyapi-range-exchange-rates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/currencyapi/refs/heads/main/openapi/currencyapi-openapi.yml
- filename: currencyapi-openapi.yml
  format: yaml
  label: CurrencyAPI Convert API
  slug: currencyapi-convert-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/currencyapi/refs/heads/main/openapi/currencyapi-openapi.yml
- filename: currencyapi-openapi.yml
  format: yaml
  label: CurrencyAPI Currencies API
  slug: currencyapi-currencies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/currencyapi/refs/heads/main/openapi/currencyapi-openapi.yml
- filename: currencyapi-openapi.yml
  format: yaml
  label: CurrencyAPI Status API
  slug: currencyapi-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/currencyapi/refs/heads/main/openapi/currencyapi-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Currencyapi Authentication
name_suffix: Authentication
oauth_flows: []
overview: CurrencyAPI secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: CurrencyAPI
provider_slug: currencyapi
scheme_count: 2
schemes:
- description: API key passed as an HTTP header (recommended).
  in: header
  name: apiKeyHeader
  parameter: apikey
  sources:
  - openapi/currencyapi-openapi.yml
  type: apiKey
- description: API key passed as a query parameter (may expose the key in access logs).
  in: query
  name: apiKeyQuery
  parameter: apikey
  sources:
  - openapi/currencyapi-openapi.yml
  type: apiKey
slug: currencyapi-authentication
source_filename: currencyapi-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/currencyapi-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  - query\nschemes:\n- name: apiKeyHeader\n  type: apiKey\n  in: header\n  parameter: apikey\n  description: API key passed as an HTTP header (recommended).\n  sources:\n  - openapi/currencyapi-openapi.yml\n- name: apiKeyQuery\n  type: apiKey\n  in: query\n  parameter: apikey\n  description: API key passed as a query parameter (may expose the key in access logs).\n  sources:\n  - openapi/currencyapi-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/currencyapi/refs/heads/main/authentication/currencyapi-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Foreign Exchange
- Currency
- Exchange Rates
- FX
- Currency Conversion
- Financial Data
---
