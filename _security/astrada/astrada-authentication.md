---
api_key_in: []
api_specs:
- filename: astrada-openapi-original.json
  format: json
  label: Astrada API
  slug: astrada-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/astrada/refs/heads/main/openapi/astrada-openapi-original.json
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Astrada Authentication
name_suffix: Authentication
oauth_flows:
- client_credentials
overview: Astrada secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the client_credentials flow(s).
provider_name: Astrada
provider_slug: astrada
scheme_count: 1
schemes:
- documented_grant: client_credentials
  name: main-auth
  scopes: 34
  sources:
  - openapi/astrada-openapi-original.json
  - https://docs.astrada.co/reference/authentication
  spec_declared_flow: implicit
  token_endpoint: https://api.astrada.co/auth/realms/{accountId}/protocol/openid-connect/token
  type: oauth2
slug: astrada-authentication
source_filename: astrada-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: openapi/astrada-openapi-original.json\ndocs: https://docs.astrada.co/reference/authentication\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - client_credentials\n  bearer: true\nnotes: >-\n  Astrada uses OAuth 2.0. The documented grant is the client-credentials flow: POST\n  client_id/client_secret/grant_type=client_credentials to the Keycloak (OpenID Connect)\n  token endpoint, then send Authorization: Bearer <access_token>. Access tokens are\n  short-lived (expires_in ~300s). Client ID, Client Secret and Account ID are provisioned\n  by Astrada support. NOTE: the OpenAPI declares the scheme flow as 'implicit', but the\n  docs and token endpoint describe client_credentials.\nschemes:\n- name: main-auth\n  type: oauth2\n  documented_grant: client_credentials\n  spec_declared_flow: implicit\n  token_endpoint: https://api.astrada.co/auth/realms/{accountId}/protocol/openid-connect/token\n  scopes: 34\n  sources:\n  - openapi/astrada-openapi-original.json\n\
  \  - https://docs.astrada.co/reference/authentication\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/astrada/refs/heads/main/authentication/astrada-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Fintech
- Payments
- Card Data
- Transaction Data
- Reconciliation
- Expense Management
- Data Infrastructure
---
