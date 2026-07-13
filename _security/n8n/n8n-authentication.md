---
api_key_in:
- header
api_specs:
- filename: n8n-openapi.yml
  format: yaml
  label: N8n
  slug: n8n
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/n8n/refs/heads/main/openapi/n8n-openapi.yml
- filename: n8n-openapi.yml
  format: yaml
  label: N8n REST API
  slug: n8n-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/n8n/refs/heads/main/openapi/n8n-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: N8N Authentication
name_suffix: Authentication
oauth_flows: []
overview: N8n secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: N8n
provider_slug: n8n
scheme_count: 2
schemes:
- in: header
  name: ApiKeyAuth
  parameter: X-N8N-API-KEY
  sources:
  - openapi/n8n-openapi.yml
  type: apiKey
- bearerFormat: JWT
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/n8n-openapi.yml
  type: http
slug: n8n-authentication
source_filename: n8n-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/n8n-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-N8N-API-KEY\n  sources:\n  - openapi/n8n-openapi.yml\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/n8n-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/n8n/refs/heads/main/authentication/n8n-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Agents
- Artificial Intelligence
- Integrations
---
