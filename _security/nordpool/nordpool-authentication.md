---
api_key_in: []
api_specs:
- filename: nordpool-intraday-asyncapi.yml
  format: yaml
  label: Nord Pool Intraday Trading API
  slug: nordpool-intraday-trading-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/nordpool/refs/heads/main/asyncapi/nordpool-intraday-asyncapi.yml
- filename: nordpool-auction-api-openapi.yml
  format: yaml
  label: Nord Pool Auction API
  slug: nordpool-auction-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nordpool/refs/heads/main/openapi/nordpool-auction-api-openapi.yml
- filename: nordpool-balancemarket-api-openapi.yml
  format: yaml
  label: Nord Pool BalanceMarket API
  slug: nordpool-balancemarket-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nordpool/refs/heads/main/openapi/nordpool-balancemarket-api-openapi.yml
- filename: nordpool-day-ahead-prices-api-openapi.yml
  format: yaml
  label: Nord Pool Day-Ahead Prices API
  slug: nordpool-day-ahead-prices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nordpool/refs/heads/main/openapi/nordpool-day-ahead-prices-api-openapi.yml
- filename: nordpool-exchangerate-api-openapi.yml
  format: yaml
  label: Nord Pool ExchangeRate API
  slug: nordpool-exchangerate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nordpool/refs/heads/main/openapi/nordpool-exchangerate-api-openapi.yml
- filename: nordpool-intraday-api-openapi.yml
  format: yaml
  label: Nord Pool Intraday API
  slug: nordpool-intraday-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nordpool/refs/heads/main/openapi/nordpool-intraday-api-openapi.yml
- filename: nordpool-powersystem-api-openapi.yml
  format: yaml
  label: Nord Pool PowerSystem API
  slug: nordpool-powersystem-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nordpool/refs/heads/main/openapi/nordpool-powersystem-api-openapi.yml
- filename: nordpool-pricecurves-api-openapi.yml
  format: yaml
  label: Nord Pool PriceCurves API
  slug: nordpool-pricecurves-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nordpool/refs/heads/main/openapi/nordpool-pricecurves-api-openapi.yml
- filename: nordpool-system-api-openapi.yml
  format: yaml
  label: Nord Pool System API
  slug: nordpool-system-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nordpool/refs/heads/main/openapi/nordpool-system-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Nordpool Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Nord Pool secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Nord Pool
provider_slug: nordpool
scheme_count: 1
schemes:
- description: Oauth2 Authentication
  flows:
  - authorizationUrl: https://sts.nordpoolgroup.com/connect/authorize
    flow: authorizationCode
    scopes: 1
    tokenUrl: https://sts.nordpoolgroup.com/connect/token
  name: oauth2
  sources:
  - openapi/nordpool-market-data-openapi.yml
  type: oauth2
slug: nordpool-authentication
source_filename: nordpool-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/nordpool-market-data-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://sts.nordpoolgroup.com/connect/authorize\n    tokenUrl: https://sts.nordpoolgroup.com/connect/token\n    scopes: 1\n  description: Oauth2 Authentication\n  sources:\n  - openapi/nordpool-market-data-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nordpool/refs/heads/main/authentication/nordpool-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Day-Ahead Prices
- Electricity
- Energy Markets
- Power Exchange
- Intraday Trading
- Market Data
- Europe
---
