---
api_key_in: []
api_specs:
- filename: nordpool-market-data-openapi.yml
  format: yaml
  label: Nord Pool Day-Ahead Prices API
  slug: nordpool-day-ahead-prices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nordpool/refs/heads/main/openapi/nordpool-market-data-openapi.yml
- filename: nordpool-market-data-openapi.yml
  format: yaml
  label: Nord Pool Intraday Market Data API
  slug: nordpool-intraday-market-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nordpool/refs/heads/main/openapi/nordpool-market-data-openapi.yml
- filename: nordpool-market-data-openapi.yml
  format: yaml
  label: Nord Pool Power System Data API
  slug: nordpool-power-system-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nordpool/refs/heads/main/openapi/nordpool-market-data-openapi.yml
- filename: nordpool-data-portal-openapi.yml
  format: yaml
  label: Nord Pool Public Data Portal API
  slug: nordpool-public-data-portal-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nordpool/refs/heads/main/openapi/nordpool-data-portal-openapi.yml
- filename: nordpool-intraday-asyncapi.yml
  format: yaml
  label: Nord Pool Intraday Trading API
  slug: nordpool-intraday-trading-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/nordpool/refs/heads/main/asyncapi/nordpool-intraday-asyncapi.yml
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
