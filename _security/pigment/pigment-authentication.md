---
api_key_in: []
api_specs:
- filename: pigment-external-api-openapi.json
  format: json
  label: Pigment External API
  slug: pigment-external-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pigment/refs/heads/main/openapi/pigment-external-api-openapi.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Pigment Authentication
name_suffix: Authentication
oauth_flows: []
overview: Pigment secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Pigment
provider_slug: pigment
scheme_count: 1
schemes:
- bearerFormat: ApiKey
  description: API Key Authorization header using the Bearer scheme.
  name: ApiKey
  scheme: bearer
  sources:
  - openapi/pigment-external-api-openapi.json
  type: http
slug: pigment-authentication
source_filename: pigment-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: derived\nsource: openapi/pigment-external-api-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: ApiKey\n  type: http\n  scheme: bearer\n  bearerFormat: ApiKey\n  description: API Key Authorization header using the Bearer scheme.\n  sources:\n  - openapi/pigment-external-api-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pigment/refs/heads/main/authentication/pigment-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Enterprise Software
- Business Planning
- Financial Planning
- FP&A
- Analytics
- EPM
- Data Integration
- MCP
- SCIM
---
