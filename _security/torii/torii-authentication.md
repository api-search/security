---
api_key_in: []
api_specs:
- filename: torii-torii-openapi.yml
  format: yaml
  label: Torii SaaS Management API
  slug: torii
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/torii/refs/heads/main/openapi/torii-torii-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Torii Authentication
name_suffix: Authentication
oauth_flows: []
overview: Torii secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Torii
provider_slug: torii
scheme_count: 1
schemes:
- description: 'API key authentication. Generate an API key from Settings > API Access in Torii. Use the Authorization header: Bearer {API_KEY}.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/torii-torii-openapi.yml
  type: http
slug: torii-authentication
source_filename: torii-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/torii-torii-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'API key authentication. Generate an API key from Settings > API Access in Torii.\n    Use the Authorization header: Bearer {API_KEY}.'\n  sources:\n  - openapi/torii-torii-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/torii/refs/heads/main/authentication/torii-authentication.yml
summary_line: http · 1 scheme
tags:
- Apps
- Compliance
- Cost Optimization
- Governance
- IT Management
- SaaS Management
---
