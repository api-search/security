---
api_key_in:
- header
api_specs:
- filename: zenadmin-external-api.yml
  format: yaml
  label: ZenAdmin External API
  slug: zenadmin-external-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zenadmin/refs/heads/main/openapi/zenadmin-external-api.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: searched
name: Zenadmin Authentication
name_suffix: Authentication
oauth_flows: []
overview: ZenAdmin secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: ZenAdmin
provider_slug: zenadmin
scheme_count: 2
schemes:
- description: Per-key API key. Shown once at creation. Rate limit 60 req/min (burst 120).
  in: header
  name: ApiKeyHeader
  parameter: x-api-key
  sources:
  - openapi/zenadmin-external-api.yml
  type: apiKey
- description: 'The API key may alternatively be sent as: Authorization Bearer <api-key>.'
  name: ApiKeyBearer
  scheme: bearer
  sources:
  - openapi/zenadmin-external-api.yml
  type: http
slug: zenadmin-authentication
source_filename: zenadmin-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://docs.zenadmin.ai\ndocs: https://docs.zenadmin.ai\nnotes: >-\n  API-key authentication only; no OAuth2/OIDC. The key is created in the ZenAdmin\n  console and shown once. Send it as the x-api-key header (recommended) or as an\n  Authorization Bearer token. Per-key rate limit 60 req/min (burst 120).\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyHeader\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: Per-key API key. Shown once at creation. Rate limit 60 req/min (burst 120).\n  sources:\n  - openapi/zenadmin-external-api.yml\n- name: ApiKeyBearer\n  type: http\n  scheme: bearer\n  description: 'The API key may alternatively be sent as: Authorization Bearer <api-key>.'\n  sources:\n  - openapi/zenadmin-external-api.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zenadmin/refs/heads/main/authentication/zenadmin-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Company
- IT Management
- Device Management
- Mobile Device Management
- IT Asset Management
- SaaS Management
- Identity and Access Management
- IT Procurement
- Employee Lifecycle
- Webhooks
---
