---
api_key_in:
- header
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Clumio Authentication
name_suffix: Authentication
oauth_flows: []
overview: Clumio secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Clumio
provider_slug: clumio
scheme_count: 1
schemes:
- bearer_format: JWT
  header: Authorization
  in: header
  name: bearerAuth
  scheme: bearer
  sources:
  - https://help.clumio.com/docs/api-tokens
  type: http
  value_format: Bearer <token>
slug: clumio-authentication
source_filename: clumio-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://help.clumio.com/docs/api-tokens\ndocs: https://help.clumio.com/docs/api-tokens\nsummary:\n  types: [http]\n  http_scheme: bearer\n  bearer_format: JWT\n  api_key_in: [header]\n  oauth2_flows: []\n  note: >-\n    Clumio authenticates every REST API request with a long-lived, signed JSON Web Token (JWT)\n    passed as a bearer token in the Authorization header. There is no OAuth2 authorization-server\n    flow; tokens are minted from the Clumio UI (Account Settings > API Tokens) and remain valid\n    until manually refreshed or deleted. Clumio recommends refreshing tokens every three months.\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearer_format: JWT\n  in: header\n  header: Authorization\n  value_format: 'Bearer <token>'\n  sources: [https://help.clumio.com/docs/api-tokens]\ntoken_types:\n- name: Personal Token\n  purpose: Development and testing. Inherits the same permissions and access as the\
  \ associated user.\n- name: Service Token\n  purpose: Production automation and third-party integrations. Not tied to an interactive user.\nexample: |\n  curl -X GET https://us-west-2.api.clumio.com/users \\\n    -H 'Authorization: Bearer ${BEARER_TOKEN}'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/clumio/refs/heads/main/authentication/clumio-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Data
- Backup
- Data Protection
- Disaster Recovery
- Cloud
- Storage
- Security
- Compliance
---
