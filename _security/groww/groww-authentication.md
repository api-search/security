---
api_key_in:
- header
api_specs:
- filename: groww-authentication-api-openapi.yml
  format: yaml
  label: Groww Authentication API
  slug: groww-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/groww/refs/heads/main/openapi/groww-authentication-api-openapi.yml
- filename: groww-historical-data-api-openapi.yml
  format: yaml
  label: Groww Historical Data API
  slug: groww-historical-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/groww/refs/heads/main/openapi/groww-historical-data-api-openapi.yml
- filename: groww-live-data-api-openapi.yml
  format: yaml
  label: Groww Live Data API
  slug: groww-live-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/groww/refs/heads/main/openapi/groww-live-data-api-openapi.yml
- filename: groww-margin-api-openapi.yml
  format: yaml
  label: Groww Margin API
  slug: groww-margin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/groww/refs/heads/main/openapi/groww-margin-api-openapi.yml
- filename: groww-orders-api-openapi.yml
  format: yaml
  label: Groww Orders API
  slug: groww-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/groww/refs/heads/main/openapi/groww-orders-api-openapi.yml
- filename: groww-portfolio-api-openapi.yml
  format: yaml
  label: Groww Portfolio API
  slug: groww-portfolio-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/groww/refs/heads/main/openapi/groww-portfolio-api-openapi.yml
auth_types:
- apiKey
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Groww Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Groww secures its APIs with apiKey, http, and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Groww
provider_slug: groww
scheme_count: 3
schemes:
- description: 'Daily access token (or API key on the token endpoint) sent as `Authorization: Bearer {ACCESS_TOKEN}`.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/groww-trade-api-openapi.yml
  type: http
- description: API version header, currently `1.0`.
  in: header
  name: apiVersion
  parameter: X-API-VERSION
  sources:
  - openapi/groww-trade-api-openapi.yml
  type: apiKey
- description: OAuth2 authorization-code flow advertised at https://api.groww.in/.well-known/oauth-authorization-server
  flows:
  - authorizationUrl: https://groww.in/oauth/authorize
    flow: authorizationCode
    scopes: 0
    tokenUrl: https://api.groww.in/oauth2/v1/token
  name: oauth2
  sources:
  - openapi/groww-trade-api-openapi.yml
  type: oauth2
slug: groww-authentication
source_filename: groww-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: derived\nsource: openapi/groww-trade-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'Daily access token (or API key on the token endpoint) sent as `Authorization:\n    Bearer {ACCESS_TOKEN}`.'\n  sources:\n  - openapi/groww-trade-api-openapi.yml\n- name: apiVersion\n  type: apiKey\n  in: header\n  parameter: X-API-VERSION\n  description: API version header, currently `1.0`.\n  sources:\n  - openapi/groww-trade-api-openapi.yml\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://groww.in/oauth/authorize\n    tokenUrl: https://api.groww.in/oauth2/v1/token\n    scopes: 0\n  description: OAuth2 authorization-code flow advertised at https://api.groww.in/.well-known/oauth-authorization-server\n  sources:\n  - openapi/groww-trade-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/groww/refs/heads/main/authentication/groww-authentication.yml
summary_line: apiKey/http/oauth2 · 3 schemes
tags:
- Company
- Fintech
- Trading
- Investing
- Stock Broking
- Market Data
- Algorithmic Trading
- India
---
