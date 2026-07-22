---
api_key_in:
- header
- query
api_specs:
- filename: quasar-rest-openapi-original.json
  format: json
  label: QuasarDB REST API
  slug: quasardb-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quasar/refs/heads/main/openapi/quasar-rest-openapi-original.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Quasar Authentication
name_suffix: Authentication
oauth_flows: []
overview: Quasar secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Quasar
provider_slug: quasar
scheme_count: 2
schemes:
- description: 'JWT bearer token obtained from POST /api/login (valid 12 hours); pass as ''Authorization: Bearer <token>''.'
  in: header
  name: Bearer
  parameter: Authorization
  sources:
  - openapi/quasar-rest-openapi-original.json
  type: apiKey
- description: The same JWT passed as a `token` query-string parameter for clients that cannot set headers.
  in: query
  name: UrlParam
  parameter: token
  sources:
  - openapi/quasar-rest-openapi-original.json
  type: apiKey
slug: quasar-authentication
source_filename: quasar-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: openapi/quasar-rest-openapi-original.json\ndocs: https://doc.quasar.ai/master/administration/security.html\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  - query\n  model: JWT bearer token (REST) over public/private key cluster credentials with server-side RBAC.\nschemes:\n- name: Bearer\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: \"JWT bearer token obtained from POST /api/login (valid 12 hours); pass as 'Authorization: Bearer <token>'.\"\n  sources:\n  - openapi/quasar-rest-openapi-original.json\n- name: UrlParam\n  type: apiKey\n  in: query\n  parameter: token\n  description: The same JWT passed as a `token` query-string parameter for clients that cannot set headers.\n  sources:\n  - openapi/quasar-rest-openapi-original.json\ncluster_auth:\n  method: public/private key\n  components: [username, user private key, cluster public key]\n  rbac_privileges: [select, insert, update, delete,\
  \ create, drop, grant, user_manage, system, set_transaction]\n  transport_encryption: Optional AES-GCM 256-bit full-stream encryption; TLS on the REST server (port 40443).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/quasar/refs/heads/main/authentication/quasar-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Company
- Time Series Database
- Database
- Analytics
- Infrastructure
- Real-Time Data
- Aerospace
- Finance
---
