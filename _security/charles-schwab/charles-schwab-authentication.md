---
api_key_in: []
api_specs:
- filename: charles-schwab-trader-api-openapi.yml
  format: yaml
  label: Charles Schwab Trader API
  slug: trader-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/charles-schwab/refs/heads/main/openapi/charles-schwab-trader-api-openapi.yml
- filename: charles-schwab-market-data-api-openapi.yml
  format: yaml
  label: Charles Schwab Market Data API
  slug: market-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/charles-schwab/refs/heads/main/openapi/charles-schwab-market-data-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Charles Schwab Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Charles Schwab secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Charles Schwab
provider_slug: charles-schwab
scheme_count: 1
schemes:
- flows:
  - authorizationUrl: https://api.schwabapi.com/v1/oauth/authorize
    flow: authorizationCode
    scopes: 1
    tokenUrl: https://api.schwabapi.com/v1/oauth/token
  name: oauth2
  sources:
  - openapi/charles-schwab-market-data-api-openapi.yml
  - openapi/charles-schwab-trader-api-openapi.yml
  type: oauth2
slug: charles-schwab-authentication
source_filename: charles-schwab-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/charles-schwab-market-data-api-openapi.yml, openapi/charles-schwab-trader-api-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.schwabapi.com/v1/oauth/authorize\n    tokenUrl: https://api.schwabapi.com/v1/oauth/token\n    scopes: 1\n  sources:\n  - openapi/charles-schwab-market-data-api-openapi.yml\n  - openapi/charles-schwab-trader-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/charles-schwab/refs/heads/main/authentication/charles-schwab-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Accounts
- Banking
- Brokerage
- Financial Services
- Investing
- Market Data
- OAuth 2.0
- Orders
- Trading
- Fortune 500
---
