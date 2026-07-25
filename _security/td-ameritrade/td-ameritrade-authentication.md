---
api_key_in:
- header
api_specs:
- filename: td-ameritrade-instruments-api-openapi.yml
  format: yaml
  label: TD Ameritrade Instruments API
  slug: td-ameritrade-instruments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/td-ameritrade/refs/heads/main/openapi/td-ameritrade-instruments-api-openapi.yml
- filename: td-ameritrade-authentication-api-openapi.yml
  format: yaml
  label: TD Ameritrade Authentication API
  slug: td-ameritrade-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/td-ameritrade/refs/heads/main/openapi/td-ameritrade-authentication-api-openapi.yml
- filename: td-ameritrade-accounts-and-trading-api-openapi.yml
  format: yaml
  label: TD Ameritrade Accounts and Trading API
  slug: td-ameritrade-accounts-and-trading-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/td-ameritrade/refs/heads/main/openapi/td-ameritrade-accounts-and-trading-api-openapi.yml
- filename: td-ameritrade-authentication-api-openapi.yml
  format: yaml
  label: TD Ameritrade Authentication API
  slug: td-ameritrade-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/td-ameritrade/refs/heads/main/openapi/td-ameritrade-authentication-api-openapi.yml
- filename: td-ameritrade-instruments-api-openapi.yml
  format: yaml
  label: TD Ameritrade Instruments API
  slug: td-ameritrade-instruments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/td-ameritrade/refs/heads/main/openapi/td-ameritrade-instruments-api-openapi.yml
- filename: td-ameritrade-market-hours-api-openapi.yml
  format: yaml
  label: TD Ameritrade Market Hours API
  slug: td-ameritrade-market-hours-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/td-ameritrade/refs/heads/main/openapi/td-ameritrade-market-hours-api-openapi.yml
- filename: td-ameritrade-movers-api-openapi.yml
  format: yaml
  label: TD Ameritrade Movers API
  slug: td-ameritrade-movers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/td-ameritrade/refs/heads/main/openapi/td-ameritrade-movers-api-openapi.yml
- filename: td-ameritrade-option-chains-api-openapi.yml
  format: yaml
  label: TD Ameritrade Option Chains API
  slug: td-ameritrade-option-chains-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/td-ameritrade/refs/heads/main/openapi/td-ameritrade-option-chains-api-openapi.yml
- filename: td-ameritrade-price-history-api-openapi.yml
  format: yaml
  label: TD Ameritrade Price History API
  slug: td-ameritrade-price-history-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/td-ameritrade/refs/heads/main/openapi/td-ameritrade-price-history-api-openapi.yml
- filename: td-ameritrade-quotes-api-openapi.yml
  format: yaml
  label: TD Ameritrade Quotes API
  slug: td-ameritrade-quotes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/td-ameritrade/refs/heads/main/openapi/td-ameritrade-quotes-api-openapi.yml
- filename: td-ameritrade-transaction-history-api-openapi.yml
  format: yaml
  label: TD Ameritrade Transaction History API
  slug: td-ameritrade-transaction-history-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/td-ameritrade/refs/heads/main/openapi/td-ameritrade-transaction-history-api-openapi.yml
- filename: td-ameritrade-user-info-preferences-api-openapi.yml
  format: yaml
  label: TD Ameritrade User Info & Preferences API
  slug: td-ameritrade-user-info-preferences-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/td-ameritrade/refs/heads/main/openapi/td-ameritrade-user-info-preferences-api-openapi.yml
- filename: td-ameritrade-watchlist-api-openapi.yml
  format: yaml
  label: TD Ameritrade Watchlist API
  slug: td-ameritrade-watchlist-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/td-ameritrade/refs/heads/main/openapi/td-ameritrade-watchlist-api-openapi.yml
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
