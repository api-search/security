---
api_key_in: []
api_specs:
- filename: finch-openapi.yml
  format: yaml
  label: Finch API
  slug: finch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/finch/refs/heads/main/openapi/finch-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Finch Authentication
name_suffix: Authentication
oauth_flows: []
overview: Finch secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Finch
provider_slug: finch
scheme_count: 1
schemes:
- bearerFormat: Finch access token
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/finch-openapi.yml
  type: http
slug: finch-authentication
source_filename: finch-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/finch-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: Finch access token\n  sources:\n  - openapi/finch-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/finch/refs/heads/main/authentication/finch-authentication.yml
summary_line: http · 1 scheme
tags:
- Employment
- HRIS
- Payroll
- Benefits
- HR
- Unified API
- Workforce
---
