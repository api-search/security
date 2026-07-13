---
api_key_in: []
api_specs:
- filename: ukg-ready-openapi.yml
  format: yaml
  label: UKG Ready REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ukg-ready/refs/heads/main/openapi/ukg-ready-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Ukg Ready Authentication
name_suffix: Authentication
oauth_flows: []
overview: UKG Ready secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: UKG Ready
provider_slug: ukg-ready
scheme_count: 1
schemes:
- description: OAuth 2.0 bearer access token issued via /authentication/access_token.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/ukg-ready-openapi.yml
  type: http
slug: ukg-ready-authentication
source_filename: ukg-ready-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/ukg-ready-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: OAuth 2.0 bearer access token issued via /authentication/access_token.\n  sources:\n  - openapi/ukg-ready-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ukg-ready/refs/heads/main/authentication/ukg-ready-authentication.yml
summary_line: http · 1 scheme
tags:
- HCM
- Human Capital Management
- Payroll
- Workforce Management
- Time and Attendance
- HR
- Benefits
---
