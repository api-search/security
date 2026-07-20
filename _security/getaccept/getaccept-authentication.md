---
api_key_in: []
api_specs:
- filename: getaccept-openapi-original.json
  format: json
  label: GetAccept API
  slug: getaccept-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/getaccept/refs/heads/main/openapi/getaccept-openapi-original.json
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Getaccept Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: GetAccept secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: GetAccept
provider_slug: getaccept
scheme_count: 2
schemes:
- description: For testing purpose, use client_id **api** and client_secret **app**
  flows:
  - authorizationUrl: https://app.getaccept.com/oauth2/authorize
    flow: authorizationCode
    scopes: 1
    tokenUrl: https://app.getaccept.com/oauth2/token
  name: Oauth2
  sources:
  - openapi/getaccept-openapi-original.json
  type: oauth2
- bearerFormat: JWT
  description: Enter your bearer token
  name: Token
  scheme: bearer
  sources:
  - openapi/getaccept-openapi-original.json
  type: http
slug: getaccept-authentication
source_filename: getaccept-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: derived\nsource: openapi/getaccept-openapi-original.json\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: Oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://app.getaccept.com/oauth2/authorize\n    tokenUrl: https://app.getaccept.com/oauth2/token\n    scopes: 1\n  description: For testing purpose, use client_id **api** and client_secret **app**\n  sources:\n  - openapi/getaccept-openapi-original.json\n- name: Token\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: Enter your bearer token\n  sources:\n  - openapi/getaccept-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/getaccept/refs/heads/main/authentication/getaccept-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Company
- Cloud
- Sales Enablement
- Electronic Signature
- E-Signature
- Digital Sales Room
- Document Management
- Contract Management
- Proposals
- SaaS
---
