---
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Oracle Eloqua Authentication
name_suffix: Authentication
oauth_flows: []
overview: Oracle Eloqua secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Oracle Eloqua
provider_slug: oracle-eloqua
scheme_count: 2
schemes:
- bearerFormat: JWT
  description: 'OAuth 2.0 access token obtained from

    `https://login.eloqua.com/auth/oauth2/token`. Sent as

    `Authorization: Bearer {access_token}`.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/oracle-eloqua-openapi.yml
  type: http
- description: 'HTTP Basic Authentication with `client_id:client_secret`. Used at

    the token endpoint and as a legacy fallback.'
  name: basicAuth
  scheme: basic
  sources:
  - openapi/oracle-eloqua-openapi.yml
  type: http
slug: oracle-eloqua-authentication
source_filename: oracle-eloqua-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/oracle-eloqua-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: |-\n    OAuth 2.0 access token obtained from\n    `https://login.eloqua.com/auth/oauth2/token`. Sent as\n    `Authorization: Bearer {access_token}`.\n  sources:\n  - openapi/oracle-eloqua-openapi.yml\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: |-\n    HTTP Basic Authentication with `client_id:client_secret`. Used at\n    the token endpoint and as a legacy fallback.\n  sources:\n  - openapi/oracle-eloqua-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/oracle-eloqua/refs/heads/main/authentication/oracle-eloqua-authentication.yml
summary_line: http · 2 schemes
tags:
- Marketing Automation
- B2B Marketing
- Email Marketing
- Campaign Management
- Lead Management
- Oracle
---
