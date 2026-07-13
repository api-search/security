---
api_key_in: []
api_specs:
- filename: aol-openapi.yml
  format: yaml
  label: Yahoo Developer Network (formerly AOL Developer)
  slug: yahoo-developer-network-formerly-aol-developer
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aol/refs/heads/main/openapi/aol-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Aol Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: AOL secures its APIs with http and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: AOL
provider_slug: aol
scheme_count: 3
schemes:
- description: HTTP Basic authentication with base64-encoded `client_id:client_secret`
  name: basicAuth
  scheme: basic
  sources:
  - openapi/aol-openapi.yml
  type: http
- bearerFormat: JWT
  description: OAuth 2.0 Bearer access token
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/aol-openapi.yml
  type: http
- flows:
  - authorizationUrl: https://api.login.yahoo.com/oauth2/request_auth
    flow: authorizationCode
    scopes: 3
    tokenUrl: https://api.login.yahoo.com/oauth2/get_token
  name: oauth2
  sources:
  - openapi/aol-openapi.yml
  type: oauth2
slug: aol-authentication
source_filename: aol-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/aol-openapi.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic authentication with base64-encoded `client_id:client_secret`\n  sources:\n  - openapi/aol-openapi.yml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: OAuth 2.0 Bearer access token\n  sources:\n  - openapi/aol-openapi.yml\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.login.yahoo.com/oauth2/request_auth\n    tokenUrl: https://api.login.yahoo.com/oauth2/get_token\n    scopes: 3\n  sources:\n  - openapi/aol-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aol/refs/heads/main/authentication/aol-authentication.yml
summary_line: http/oauth2 · 3 schemes
tags:
- Advertising
- Digital Media
- Entertainment
- News
- Fortune 1000
---
