---
api_key_in:
- header
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Routefusion Authentication
name_suffix: Authentication
oauth_flows: []
overview: Routefusion secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Routefusion
provider_slug: routefusion
scheme_count: 1
schemes:
- description: A static API key presented as an HTTP bearer token on every GraphQL request. Tokens are issued by Routefusion on request (email customersuccess@routefusion.com); there is no self-service OAuth flow.
  format: 'Authorization: Bearer ${token}'
  header: Authorization
  in: header
  name: bearerAuth
  scheme: bearer
  token_contact: customersuccess@routefusion.com
  token_issuance: manual
  type: http
slug: routefusion-authentication
source_filename: routefusion-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://docs.routefusion.com/reference/authentication\ndocs: https://docs.routefusion.com/reference/authentication\nsummary:\n  types: [http]\n  scheme: bearer\n  api_key_in: [header]\n  oauth2_flows: []\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  in: header\n  header: Authorization\n  format: 'Authorization: Bearer ${token}'\n  description: A static API key presented as an HTTP bearer token on every GraphQL\n    request. Tokens are issued by Routefusion on request (email customersuccess@routefusion.com);\n    there is no self-service OAuth flow.\n  token_issuance: manual\n  token_contact: customersuccess@routefusion.com\nnotes:\n- The same bearer credential authenticates all GraphQL queries and mutations; some\n  admin actions (e.g. createUser) additionally require the caller's user to have the\n  admin role within their organization.\n- Separate sandbox and production tokens/endpoints exist (see sandbox/\
  \ and lifecycle/).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/routefusion/refs/heads/main/authentication/routefusion-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Fintech
- Payments
- Cross-Border Payments
- Global Payments
- FX
- Wallets
- GraphQL
- Stablecoin
---
