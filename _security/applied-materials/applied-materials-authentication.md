---
api_key_in: []
api_specs:
- filename: applied-materials-openapi.yaml
  format: yaml
  label: Applied Materials API
  slug: applied-materials-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/applied-materials/refs/heads/main/openapi/applied-materials-openapi.yaml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Applied Materials Authentication
name_suffix: Authentication
oauth_flows: []
overview: Applied Materials secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Applied Materials
provider_slug: applied-materials
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/applied-materials-openapi.yaml
  type: http
slug: applied-materials-authentication
source_filename: applied-materials-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/applied-materials-openapi.yaml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/applied-materials-openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/applied-materials/refs/heads/main/authentication/applied-materials-authentication.yml
summary_line: http · 1 scheme
tags:
- Semiconductor
- Manufacturing
- Equipment
- Fab Operations
- Materials Engineering
- Fortune 500
---
