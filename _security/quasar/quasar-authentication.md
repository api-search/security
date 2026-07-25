---
api_key_in:
- header
- query
api_specs:
- filename: quasar-cluster-api-openapi.yml
  format: yaml
  label: Quasar cluster API
  slug: quasar-cluster-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quasar/refs/heads/main/openapi/quasar-cluster-api-openapi.yml
- filename: quasar-login-api-openapi.yml
  format: yaml
  label: Quasar Login API
  slug: quasar-login-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quasar/refs/heads/main/openapi/quasar-login-api-openapi.yml
- filename: quasar-max-in-buffer-size-api-openapi.yml
  format: yaml
  label: Quasar max-in-buffer-size API
  slug: quasar-max-in-buffer-size-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quasar/refs/heads/main/openapi/quasar-max-in-buffer-size-api-openapi.yml
- filename: quasar-option-api-openapi.yml
  format: yaml
  label: Quasar option API
  slug: quasar-option-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quasar/refs/heads/main/openapi/quasar-option-api-openapi.yml
- filename: quasar-parallelism-api-openapi.yml
  format: yaml
  label: Quasar parallelism API
  slug: quasar-parallelism-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quasar/refs/heads/main/openapi/quasar-parallelism-api-openapi.yml
- filename: quasar-prometheus-api-openapi.yml
  format: yaml
  label: Quasar Prometheus API
  slug: quasar-prometheus-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quasar/refs/heads/main/openapi/quasar-prometheus-api-openapi.yml
- filename: quasar-query-api-openapi.yml
  format: yaml
  label: Quasar query API
  slug: quasar-query-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quasar/refs/heads/main/openapi/quasar-query-api-openapi.yml
- filename: quasar-status-api-openapi.yml
  format: yaml
  label: Quasar Status API
  slug: quasar-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quasar/refs/heads/main/openapi/quasar-status-api-openapi.yml
- filename: quasar-tables-api-openapi.yml
  format: yaml
  label: Quasar Tables API
  slug: quasar-tables-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quasar/refs/heads/main/openapi/quasar-tables-api-openapi.yml
- filename: quasar-tags-api-openapi.yml
  format: yaml
  label: Quasar tags API
  slug: quasar-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quasar/refs/heads/main/openapi/quasar-tags-api-openapi.yml
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
