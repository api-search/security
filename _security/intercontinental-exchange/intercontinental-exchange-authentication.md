---
api_key_in:
- header
api_specs:
- filename: intercontinental-exchange-instruments-api-openapi.yml
  format: yaml
  label: ICE Consolidated Feed API
  slug: consolidated-feed-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/intercontinental-exchange/refs/heads/main/openapi/intercontinental-exchange-instruments-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Intercontinental Exchange Authentication
name_suffix: Authentication
oauth_flows: []
overview: Intercontinental Exchange secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Intercontinental Exchange
provider_slug: intercontinental-exchange
scheme_count: 2
schemes:
- in: header
  name: apiKey
  parameter: Authorization
  sources:
  - openapi/intercontinental-exchange-instruments-api-openapi.yml
  - openapi/intercontinental-exchange-market-data-api-openapi.yml
  - openapi/intercontinental-exchange-reference-data-api-openapi.yml
  type: apiKey
- name: bearerAuth
  scheme: bearer
  sources:
  - openapi/intercontinental-exchange-instruments-api-openapi.yml
  - openapi/intercontinental-exchange-market-data-api-openapi.yml
  - openapi/intercontinental-exchange-reference-data-api-openapi.yml
  type: http
slug: intercontinental-exchange-authentication
source_filename: intercontinental-exchange-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-22'\nmethod: derived\nsource: openapi/intercontinental-exchange-instruments-api-openapi.yml, openapi/intercontinental-exchange-market-data-api-openapi.yml,\n  openapi/intercontinental-exchange-reference-data-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: Authorization\n  sources:\n  - openapi/intercontinental-exchange-instruments-api-openapi.yml\n  - openapi/intercontinental-exchange-market-data-api-openapi.yml\n  - openapi/intercontinental-exchange-reference-data-api-openapi.yml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/intercontinental-exchange-instruments-api-openapi.yml\n  - openapi/intercontinental-exchange-market-data-api-openapi.yml\n  - openapi/intercontinental-exchange-reference-data-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/intercontinental-exchange/refs/heads/main/authentication/intercontinental-exchange-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Commodities
- Financial Exchanges
- Market Data
- NYSE
- Trading
- Fortune 1000
---
