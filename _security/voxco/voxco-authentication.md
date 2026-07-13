---
api_key_in: []
api_specs:
- filename: coder
  format: yaml
  label: Voxco Survey API
  slug: voxco-survey-api
  spec_type: OpenAPI
  url: https://webservices.goascribe.com/coder
- filename: coder
  format: yaml
  label: Voxco Ascribe Coder API
  slug: voxco-ascribe-coder-api
  spec_type: OpenAPI
  url: https://webservices.goascribe.com/coder
- filename: cxi
  format: yaml
  label: Voxco Ascribe CX Inspector API
  slug: voxco-ascribe-cxi-api
  spec_type: OpenAPI
  url: https://webservices.goascribe.com/cxi
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Voxco Authentication
name_suffix: Authentication
oauth_flows: []
overview: Voxco secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Voxco
provider_slug: voxco
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: 'Please enter a valid bearer token.


    It should be in the format "bearer eyJhbGciOiJSU..."


    It will be added to the "Authentication" HTTP header'
  name: Bearer
  scheme: Bearer
  sources:
  - openapi/voxco-ascribe-coder-api-openapi.json
  type: http
slug: voxco-authentication
source_filename: voxco-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/voxco-ascribe-coder-api-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: Bearer\n  type: http\n  scheme: Bearer\n  bearerFormat: JWT\n  description: |-\n    Please enter a valid bearer token.\n\n    It should be in the format \"bearer eyJhbGciOiJSU...\"\n\n    It will be added to the \"Authentication\" HTTP header\n  sources:\n  - openapi/voxco-ascribe-coder-api-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/voxco/refs/heads/main/authentication/voxco-authentication.yml
summary_line: http · 1 scheme
tags:
- Survey Software
- Market Research
- CATI
- Omnichannel
- Text Analytics
- Data Collection
- Panel Management
---
