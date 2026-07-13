---
api_key_in:
- header
api_specs:
- filename: ampersand-api-openapi-original.yml
  format: yaml
  label: Ampersand API
  slug: ampersand-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ampersand/refs/heads/main/openapi/ampersand-api-openapi-original.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Ampersand Authentication
name_suffix: Authentication
oauth_flows: []
overview: Ampersand secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Ampersand
provider_slug: ampersand
scheme_count: 2
schemes:
- in: header
  name: APIKeyHeader
  parameter: X-Api-Key
  sources:
  - openapi/ampersand-api-openapi-original.yml
  type: apiKey
- bearerFormat: JWT
  name: Bearer
  scheme: bearer
  sources:
  - openapi/ampersand-api-openapi-original.yml
  type: http
slug: ampersand-authentication
source_filename: ampersand-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/ampersand-api-openapi-original.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: APIKeyHeader\n  type: apiKey\n  in: header\n  parameter: X-Api-Key\n  sources:\n  - openapi/ampersand-api-openapi-original.yml\n- name: Bearer\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/ampersand-api-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ampersand/refs/heads/main/authentication/ampersand-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Developer Tools
- Integrations
- Platform
- SaaS
- OAuth
- Data Sync
- Webhooks
---
