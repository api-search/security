---
api_key_in: []
api_specs:
- filename: twentyci-twentyapi-oauth-openapi.json
  format: json
  label: TwentyAPI OAuth Token API
  slug: twentyapi-oauth-token-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/twentyci/refs/heads/main/openapi/twentyci-twentyapi-oauth-openapi.json
- filename: twentyci-twentyapi-openapi.json
  format: json
  label: TwentyAPI Properties API
  slug: twentyapi-properties-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/twentyci/refs/heads/main/openapi/twentyci-twentyapi-openapi.json
- filename: twentyci-twentyapi-openapi.json
  format: json
  label: TwentyAPI Agent Performance API
  slug: twentyapi-agent-performance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/twentyci/refs/heads/main/openapi/twentyci-twentyapi-openapi.json
- filename: twentyci-twentyapi-openapi.json
  format: json
  label: TwentyAPI Trigger Information API
  slug: twentyapi-trigger-information-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/twentyci/refs/heads/main/openapi/twentyci-twentyapi-openapi.json
- filename: twentyci-twentyapi-openapi.json
  format: json
  label: TwentyAPI Categories API
  slug: twentyapi-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/twentyci/refs/heads/main/openapi/twentyci-twentyapi-openapi.json
- filename: twentyci-twentyapi-openapi.json
  format: json
  label: TwentyAPI Address Match API
  slug: twentyapi-address-match-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/twentyci/refs/heads/main/openapi/twentyci-twentyapi-openapi.json
- filename: twentyci-twentyapi-openapi.json
  format: json
  label: TwentyAPI Schools API
  slug: twentyapi-schools-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/twentyci/refs/heads/main/openapi/twentyci-twentyapi-openapi.json
- filename: twentyci-twentyapi-openapi.json
  format: json
  label: TwentyAPI UK Housing Market Metrics API
  slug: twentyapi-uk-housing-market-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/twentyci/refs/heads/main/openapi/twentyci-twentyapi-openapi.json
- filename: twentyci-twentyapi-openapi.json
  format: json
  label: TwentyAPI This is Now API
  slug: twentyapi-this-is-now-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/twentyci/refs/heads/main/openapi/twentyci-twentyapi-openapi.json
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
