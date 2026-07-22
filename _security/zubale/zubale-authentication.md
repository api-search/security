---
api_key_in: []
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Zubale Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Zubale secures its APIs with http and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Zubale
provider_slug: zubale
scheme_count: 3
schemes:
- bearerFormat: JWT
  description: 'OAuth2 client-credentials access token from POST /oauth2/token, sent as Authorization: Bearer <token>.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/zubale-openapi.yml
  type: http
- description: HTTP Basic (client_id:client_secret) used only against POST /oauth2/token.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/zubale-openapi.yml
  type: http
- flows:
  - flow: clientCredentials
    scopes: 0
    tokenUrl: https://api.zubale.com/oauth2/token
  name: oauth2
  sources:
  - openapi/zubale-openapi.yml
  type: oauth2
slug: zubale-authentication
source_filename: zubale-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: derived\nsource: openapi/zubale-openapi.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: 'OAuth2 client-credentials access token from POST /oauth2/token, sent as Authorization:\n    Bearer <token>.'\n  sources:\n  - openapi/zubale-openapi.yml\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic (client_id:client_secret) used only against POST /oauth2/token.\n  sources:\n  - openapi/zubale-openapi.yml\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.zubale.com/oauth2/token\n    scopes: 0\n  sources:\n  - openapi/zubale-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zubale/refs/heads/main/authentication/zubale-authentication.yml
summary_line: http/oauth2 · 3 schemes
tags:
- Company
- Ecommerce
---
