---
api_key_in:
- header
- query
api_specs:
- filename: openapi.yml
  format: yaml
  label: Free Currency API
  slug: freecurrencyapi
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freecurrencyapi/refs/heads/main/openapi/openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Freecurrencyapi Authentication
name_suffix: Authentication
oauth_flows: []
overview: Free Currency API secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Free Currency API
provider_slug: freecurrencyapi
scheme_count: 2
schemes:
- description: 'API key passed as a query parameter. Note: this may expose your API key in access logs. Using the header method is recommended.'
  in: query
  name: ApiKeyQuery
  parameter: apikey
  sources:
  - openapi/openapi.yml
  type: apiKey
- description: API key passed as an HTTP header (recommended method).
  in: header
  name: ApiKeyHeader
  parameter: apikey
  sources:
  - openapi/openapi.yml
  type: apiKey
slug: freecurrencyapi-authentication
source_filename: freecurrencyapi-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  - query\nschemes:\n- name: ApiKeyQuery\n  type: apiKey\n  in: query\n  parameter: apikey\n  description: 'API key passed as a query parameter. Note: this may expose your API key in access\n    logs. Using the header method is recommended.'\n  sources:\n  - openapi/openapi.yml\n- name: ApiKeyHeader\n  type: apiKey\n  in: header\n  parameter: apikey\n  description: API key passed as an HTTP header (recommended method).\n  sources:\n  - openapi/openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/freecurrencyapi/refs/heads/main/authentication/freecurrencyapi-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Currency
- Exchange Rates
- Finance
- Historical Data
- Free
---
