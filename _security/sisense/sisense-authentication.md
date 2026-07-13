---
api_key_in: []
api_specs:
- filename: sisense-rest-api-openapi.yml
  format: yaml
  label: Sisense REST API v1
  slug: rest-api-v1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sisense/refs/heads/main/openapi/sisense-rest-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Sisense Authentication
name_suffix: Authentication
oauth_flows: []
overview: Sisense secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Sisense
provider_slug: sisense
scheme_count: 1
schemes:
- description: Bearer token obtained from POST /api/v1/authentication/login
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/sisense-rest-api-openapi.yml
  type: http
slug: sisense-authentication
source_filename: sisense-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/sisense-rest-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Bearer token obtained from POST /api/v1/authentication/login\n  sources:\n  - openapi/sisense-rest-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sisense/refs/heads/main/authentication/sisense-authentication.yml
summary_line: http · 1 scheme
tags:
- Analytics
- Business Intelligence
- Dashboards
- Data Models
- Embedded Analytics
---
