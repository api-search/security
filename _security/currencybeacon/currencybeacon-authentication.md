---
api_key_in:
- query
api_specs:
- filename: currencybeacon-openapi.yml
  format: yaml
  label: CurrencyBeacon API
  slug: currencybeacon-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/currencybeacon/refs/heads/main/openapi/currencybeacon-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Currencybeacon Authentication
name_suffix: Authentication
oauth_flows: []
overview: CurrencyBeacon secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: CurrencyBeacon
provider_slug: currencybeacon
scheme_count: 2
schemes:
- description: API key passed as a query parameter.
  in: query
  name: ApiKeyQuery
  parameter: api_key
  sources:
  - openapi/currencybeacon-openapi.yml
  type: apiKey
- description: API key passed as a Bearer token in the Authorization header.
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/currencybeacon-openapi.yml
  type: http
slug: currencybeacon-authentication
source_filename: currencybeacon-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/currencybeacon-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - query\nschemes:\n- name: ApiKeyQuery\n  type: apiKey\n  in: query\n  parameter: api_key\n  description: API key passed as a query parameter.\n  sources:\n  - openapi/currencybeacon-openapi.yml\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: API key passed as a Bearer token in the Authorization header.\n  sources:\n  - openapi/currencybeacon-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/currencybeacon/refs/heads/main/authentication/currencybeacon-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Currency
- Exchange Rates
- Forex
- Cryptocurrency
- Financial Data
- Historical Rates
- Currency Conversion
---
