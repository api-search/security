---
api_key_in: []
api_specs:
- filename: td-ameritrade-holding-accounts-api-openapi.yml
  format: yaml
  label: TD Ameritrade Holding Accounts API
  slug: td-ameritrade-holding-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/td-ameritrade-holding/refs/heads/main/openapi/td-ameritrade-holding-accounts-api-openapi.yml
- filename: td-ameritrade-holding-instruments-api-openapi.yml
  format: yaml
  label: TD Ameritrade Holding Instruments API
  slug: td-ameritrade-holding-instruments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/td-ameritrade-holding/refs/heads/main/openapi/td-ameritrade-holding-instruments-api-openapi.yml
- filename: td-ameritrade-holding-market-data-api-openapi.yml
  format: yaml
  label: TD Ameritrade Holding Market Data API
  slug: td-ameritrade-holding-market-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/td-ameritrade-holding/refs/heads/main/openapi/td-ameritrade-holding-market-data-api-openapi.yml
- filename: td-ameritrade-holding-options-api-openapi.yml
  format: yaml
  label: TD Ameritrade Holding Options API
  slug: td-ameritrade-holding-options-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/td-ameritrade-holding/refs/heads/main/openapi/td-ameritrade-holding-options-api-openapi.yml
- filename: td-ameritrade-holding-orders-api-openapi.yml
  format: yaml
  label: TD Ameritrade Holding Orders API
  slug: td-ameritrade-holding-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/td-ameritrade-holding/refs/heads/main/openapi/td-ameritrade-holding-orders-api-openapi.yml
- filename: td-ameritrade-holding-saved-orders-api-openapi.yml
  format: yaml
  label: TD Ameritrade Holding Saved Orders API
  slug: td-ameritrade-holding-saved-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/td-ameritrade-holding/refs/heads/main/openapi/td-ameritrade-holding-saved-orders-api-openapi.yml
- filename: td-ameritrade-holding-transactions-api-openapi.yml
  format: yaml
  label: TD Ameritrade Holding Transactions API
  slug: td-ameritrade-holding-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/td-ameritrade-holding/refs/heads/main/openapi/td-ameritrade-holding-transactions-api-openapi.yml
- filename: td-ameritrade-holding-user-management-api-openapi.yml
  format: yaml
  label: TD Ameritrade Holding User Management API
  slug: td-ameritrade-holding-user-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/td-ameritrade-holding/refs/heads/main/openapi/td-ameritrade-holding-user-management-api-openapi.yml
- filename: td-ameritrade-holding-watchlists-api-openapi.yml
  format: yaml
  label: TD Ameritrade Holding Watchlists API
  slug: td-ameritrade-holding-watchlists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/td-ameritrade-holding/refs/heads/main/openapi/td-ameritrade-holding-watchlists-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Td Ameritrade Holding Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: TD Ameritrade Holding secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: TD Ameritrade Holding
provider_slug: td-ameritrade-holding
scheme_count: 1
schemes:
- description: TD Ameritrade uses OAuth 2.0 token-based authentication
  flows:
  - authorizationUrl: https://auth.tdameritrade.com/auth
    flow: authorizationCode
    scopes: 3
    tokenUrl: https://api.tdameritrade.com/v1/oauth2/token
  name: OAuth2
  sources:
  - openapi/td-ameritrade-accounts-trading-openapi.yml
  type: oauth2
slug: td-ameritrade-holding-authentication
source_filename: td-ameritrade-holding-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/td-ameritrade-accounts-trading-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.tdameritrade.com/auth\n    tokenUrl: https://api.tdameritrade.com/v1/oauth2/token\n    scopes: 3\n  description: TD Ameritrade uses OAuth 2.0 token-based authentication\n  sources:\n  - openapi/td-ameritrade-accounts-trading-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/td-ameritrade-holding/refs/heads/main/authentication/td-ameritrade-holding-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Finance
- Brokerage
- Trading
- Market Data
- Investment
- Charles Schwab
- Deprecated
- Fortune 1000
---
