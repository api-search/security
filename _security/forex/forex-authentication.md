---
api_key_in:
- query
api_specs:
- filename: forex-openapi.yml
  format: yaml
  label: Open Exchange Rates API
  slug: open-exchange-rates
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/forex/refs/heads/main/openapi/forex-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Forex Authentication
name_suffix: Authentication
oauth_flows: []
overview: Forex secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Forex
provider_slug: forex
scheme_count: 1
schemes:
- in: query
  name: appIdQuery
  parameter: app_id
  sources:
  - openapi/forex-openapi.yml
  type: apiKey
slug: forex-authentication
source_filename: forex-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/forex-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: appIdQuery\n  type: apiKey\n  in: query\n  parameter: app_id\n  sources:\n  - openapi/forex-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/forex/refs/heads/main/authentication/forex-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Currency
- Exchange Rates
- Financial Data
- Forex
- Trading
---
