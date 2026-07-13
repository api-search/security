---
api_key_in: []
api_specs:
- filename: starbucks-starbucks-api-openapi.yml
  format: yaml
  label: Starbucks API
  slug: starbucks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/starbucks/refs/heads/main/openapi/starbucks-starbucks-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Starbucks Authentication
name_suffix: Authentication
oauth_flows: []
overview: Starbucks secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Starbucks
provider_slug: starbucks
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/starbucks-starbucks-api-openapi.yml
  type: http
slug: starbucks-authentication
source_filename: starbucks-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/starbucks-starbucks-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/starbucks-starbucks-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/starbucks/refs/heads/main/authentication/starbucks-authentication.yml
summary_line: http · 1 scheme
tags:
- Coffee
- Food Service
- Loyalty
- Ordering
- Retail
- Fortune 500
---
