---
api_key_in:
- header
api_specs:
- filename: firstrade-account-api-openapi.yml
  format: yaml
  label: Firstrade Account API
  slug: firstrade-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/firstrade/refs/heads/main/openapi/firstrade-account-api-openapi.yml
- filename: firstrade-authentication-api-openapi.yml
  format: yaml
  label: Firstrade Authentication API
  slug: firstrade-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/firstrade/refs/heads/main/openapi/firstrade-authentication-api-openapi.yml
- filename: firstrade-market-data-api-openapi.yml
  format: yaml
  label: Firstrade Market Data API
  slug: firstrade-market-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/firstrade/refs/heads/main/openapi/firstrade-market-data-api-openapi.yml
- filename: firstrade-orders-api-openapi.yml
  format: yaml
  label: Firstrade Orders API
  slug: firstrade-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/firstrade/refs/heads/main/openapi/firstrade-orders-api-openapi.yml
- filename: firstrade-watchlist-api-openapi.yml
  format: yaml
  label: Firstrade Watchlist API
  slug: firstrade-watchlist-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/firstrade/refs/heads/main/openapi/firstrade-watchlist-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Firstrade Authentication
name_suffix: Authentication
oauth_flows: []
overview: Firstrade secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Firstrade
provider_slug: firstrade
scheme_count: 1
schemes:
- description: 'Session token obtained after login. The ftat header must be accompanied by a sid header (session ID) and the static access-token header (value: 833w3XuIFycv18ybi).'
  in: header
  name: sessionAuth
  parameter: ftat
  sources:
  - openapi/openapi.yml
  type: apiKey
slug: firstrade-authentication
source_filename: firstrade-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: sessionAuth\n  type: apiKey\n  in: header\n  parameter: ftat\n  description: 'Session token obtained after login. The ftat header must be accompanied by a\n    sid header (session ID) and the static access-token header (value: 833w3XuIFycv18ybi).'\n  sources:\n  - openapi/openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/firstrade/refs/heads/main/authentication/firstrade-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Brokerage
- Commission-Free Trading
- Stocks
- ETFs
- Options
- Mutual Funds
- Fixed Income
- Retirement
- IRA
- Investing
- Finance
- Open Banking
---
