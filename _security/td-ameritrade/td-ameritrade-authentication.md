---
api_key_in:
- header
api_specs:
- filename: apis
  format: yaml
  label: TD Ameritrade Accounts and Trading API
  slug: td-ameritrade-accounts-and-trading-api
  spec_type: OpenAPI
  url: https://developer.tdameritrade.com/account-access/apis
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Td Ameritrade Authentication
name_suffix: Authentication
oauth_flows: []
overview: TD Ameritrade secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: TD Ameritrade
provider_slug: td-ameritrade
scheme_count: 1
schemes:
- in: header
  name: Bearer
  parameter: Authorization
  sources:
  - openapi/openapi.yml
  type: apiKey
slug: td-ameritrade-authentication
source_filename: td-ameritrade-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: Bearer\n  type: apiKey\n  in: header\n  parameter: Authorization\n  sources:\n  - openapi/openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/td-ameritrade/refs/heads/main/authentication/td-ameritrade-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Brokerage
- Trading
- Finance
- Equities
- Options
- Market Data
- Streaming
---
