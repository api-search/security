---
api_key_in: []
api_specs:
- filename: twentyci-address-match-api-openapi.yml
  format: yaml
  label: TwentyCi Address Match API
  slug: twentyci-address-match-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/twentyci/refs/heads/main/openapi/twentyci-address-match-api-openapi.yml
- filename: twentyci-agent-performance-api-openapi.yml
  format: yaml
  label: TwentyCi Agent Performance API
  slug: twentyci-agent-performance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/twentyci/refs/heads/main/openapi/twentyci-agent-performance-api-openapi.yml
- filename: twentyci-authorisation-api-openapi.yml
  format: yaml
  label: TwentyCi Authorisation API
  slug: twentyci-authorisation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/twentyci/refs/heads/main/openapi/twentyci-authorisation-api-openapi.yml
- filename: twentyci-categories-api-openapi.yml
  format: yaml
  label: TwentyCi Categories API
  slug: twentyci-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/twentyci/refs/heads/main/openapi/twentyci-categories-api-openapi.yml
- filename: twentyci-properties-api-openapi.yml
  format: yaml
  label: TwentyCi Properties API
  slug: twentyci-properties-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/twentyci/refs/heads/main/openapi/twentyci-properties-api-openapi.yml
- filename: twentyci-schools-api-openapi.yml
  format: yaml
  label: TwentyCi Schools API
  slug: twentyci-schools-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/twentyci/refs/heads/main/openapi/twentyci-schools-api-openapi.yml
- filename: twentyci-this-is-now-retail-propensity-to-buy-goods-api-openapi.yml
  format: yaml
  label: TwentyCi This is Now | Retail Propensity To Buy Goods API
  slug: twentyci-this-is-now-retail-propensity-to-buy-goods-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/twentyci/refs/heads/main/openapi/twentyci-this-is-now-retail-propensity-to-buy-goods-api-openapi.yml
- filename: twentyci-trigger-information-api-openapi.yml
  format: yaml
  label: TwentyCi Trigger Information API
  slug: twentyci-trigger-information-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/twentyci/refs/heads/main/openapi/twentyci-trigger-information-api-openapi.yml
- filename: twentyci-uk-housing-market-metrics-api-openapi.yml
  format: yaml
  label: TwentyCi UK Housing Market Metrics API
  slug: twentyci-uk-housing-market-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/twentyci/refs/heads/main/openapi/twentyci-uk-housing-market-metrics-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Twentyci Authentication
name_suffix: Authentication
oauth_flows:
- password
overview: TwentyCi secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the password flow(s).
provider_name: TwentyCi
provider_slug: twentyci
scheme_count: 1
schemes:
- description: 'OAuth 2.0 bearer token. TwentyCi''s documentation labels the scheme "OAuth2" with flow "Implicit" but describes a resource-owner password-credentials exchange: POST /oauth/token with client_id, client_secret, username, password, grant_type=password and scope=* returns {token_type: Bearer, expires_in, access_token, refresh_token}. The token is then sent as "Authorization: Bearer <token-key>". Modell'
  flows:
  - flow: password
    scopes: 1
    tokenUrl: https://api.twentyci.co.uk/oauth/token
  name: twentyapiOAuth
  sources:
  - openapi/twentyci-twentyapi-openapi.json
  type: oauth2
slug: twentyci-authentication
source_filename: twentyci-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-26'\nmethod: derived\nsource: openapi/twentyci-twentyapi-openapi.json\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - password\nschemes:\n- name: twentyapiOAuth\n  type: oauth2\n  flows:\n  - flow: password\n    tokenUrl: https://api.twentyci.co.uk/oauth/token\n    scopes: 1\n  description: 'OAuth 2.0 bearer token. TwentyCi''s documentation labels the scheme \"OAuth2\"\n    with flow \"Implicit\" but describes a resource-owner password-credentials exchange: POST\n    /oauth/token with client_id, client_secret, username, password, grant_type=password and\n    scope=* returns {token_type: Bearer, expires_in, access_token, refresh_token}. The token\n    is then sent as \"Authorization: Bearer <token-key>\". Modell'\n  sources:\n  - openapi/twentyci-twentyapi-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/twentyci/refs/heads/main/authentication/twentyci-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Real-Estate
- United Kingdom
- PropTech
- Property Data
- Valuation
- AVM
- Rentals
- Address Data
- Conveyancing
- Homemover Data
- Agent Performance
- Data as a Service
---
