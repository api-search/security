---
api_key_in: []
api_specs:
- filename: zally-api.yml
  format: yaml
  label: Zally API
  slug: zally-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zally/refs/heads/main/openapi/zally-api.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Zally Authentication
name_suffix: Authentication
oauth_flows: []
overview: Zally secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Zally
provider_slug: zally
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/zally-api.yml
  type: http
slug: zally-authentication
source_filename: zally-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/zally-api.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/zally-api.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zally/refs/heads/main/authentication/zally-authentication.yml
summary_line: http · 1 scheme
tags:
- API Design
- API Linting
- API Quality
- Open Source
- OpenAPI
- Zalando
---
