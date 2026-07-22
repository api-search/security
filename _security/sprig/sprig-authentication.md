---
api_key_in:
- header
api_specs:
- filename: sprig-api-openapi-original.json
  format: json
  label: Sprig API
  slug: sprig-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sprig/refs/heads/main/openapi/sprig-api-openapi-original.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Sprig Authentication
name_suffix: Authentication
oauth_flows: []
overview: Sprig secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Sprig
provider_slug: sprig
scheme_count: 1
schemes:
- description: Use `API-Key YOUR_API_KEY` for v2 endpoints or `Bearer YOUR_API_KEY` for export endpoints.
  in: header
  name: apiKeyAuth
  parameter: Authorization
  sources:
  - openapi/sprig-api-openapi-original.json
  type: apiKey
slug: sprig-authentication
source_filename: sprig-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: derived\nsource: openapi/sprig-api-openapi-original.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Use `API-Key YOUR_API_KEY` for v2 endpoints or `Bearer YOUR_API_KEY` for export\n    endpoints.\n  sources:\n  - openapi/sprig-api-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sprig/refs/heads/main/authentication/sprig-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Product Research
- Surveys
- User Insights
- Customer Experience
- Analytics
- Product Analytics
- AI
- SaaS
---
