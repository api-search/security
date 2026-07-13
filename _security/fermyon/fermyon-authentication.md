---
api_key_in:
- header
api_specs:
- filename: fermyon-openapi.yml
  format: yaml
  label: Fermyon Wasm Functions
  slug: fermyon
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fermyon/refs/heads/main/openapi/fermyon-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Fermyon Authentication
name_suffix: Authentication
oauth_flows: []
overview: Fermyon secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Fermyon
provider_slug: fermyon
scheme_count: 1
schemes:
- description: 'JWT Authorization header using the Bearer scheme. Example: "Authorization: Bearer {token}"'
  in: header
  name: Bearer
  parameter: Authorization
  sources:
  - openapi/fermyon-openapi.yml
  type: apiKey
slug: fermyon-authentication
source_filename: fermyon-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/fermyon-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: Bearer\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: 'JWT Authorization header using the Bearer scheme. Example: \"Authorization: Bearer\n    {token}\"'\n  sources:\n  - openapi/fermyon-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fermyon/refs/heads/main/authentication/fermyon-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Compute
- Functions
- WebAssembly
- Serverless
---
