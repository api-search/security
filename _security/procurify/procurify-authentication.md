---
api_key_in:
- cookie
api_specs:
- filename: openapi.json
  format: json
  label: Procurify API
  slug: procurify-api
  spec_type: OpenAPI
  url: https://developer.procurify.com/openapi.json
auth_types:
- apiKey
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Procurify Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Procurify secures its APIs with apiKey, http, and oauth2 across 4 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Procurify
provider_slug: procurify
scheme_count: 4
schemes:
- name: BasicAuthentication
  scheme: basic
  sources:
  - openapi/procurify-procurify-api-openapi.yml
  type: http
- bearerFormat: JWT
  name: M2MAuthentication
  scheme: bearer
  sources:
  - openapi/procurify-procurify-api-openapi.yml
  type: http
- flows:
  - authorizationUrl: https://<your-domain>.procurify.com/oauth/authorize
    flow: authorizationCode
    scopes: 0
    tokenUrl: https://<your-domain>.procurify.com/oauth/token
  name: RemoteAuthentication
  sources:
  - openapi/procurify-procurify-api-openapi.yml
  type: oauth2
- in: cookie
  name: cookieAuth
  parameter: sessionid
  sources:
  - openapi/procurify-procurify-api-openapi.yml
  type: apiKey
slug: procurify-authentication
source_filename: procurify-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/procurify-procurify-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  - oauth2\n  api_key_in:\n  - cookie\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: BasicAuthentication\n  type: http\n  scheme: basic\n  sources:\n  - openapi/procurify-procurify-api-openapi.yml\n- name: M2MAuthentication\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/procurify-procurify-api-openapi.yml\n- name: RemoteAuthentication\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://<your-domain>.procurify.com/oauth/authorize\n    tokenUrl: https://<your-domain>.procurify.com/oauth/token\n    scopes: 0\n  sources:\n  - openapi/procurify-procurify-api-openapi.yml\n- name: cookieAuth\n  type: apiKey\n  in: cookie\n  parameter: sessionid\n  sources:\n  - openapi/procurify-procurify-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/procurify/refs/heads/main/authentication/procurify-authentication.yml
summary_line: apiKey/http/oauth2 · 4 schemes
tags:
- Spend Management
- Procurement
- Purchase Orders
- Accounts Payable
- Vendor Management
- Budget Tracking
- Procure-to-Pay
- ERP Integration
---
