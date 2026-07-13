---
api_key_in: []
api_specs:
- filename: stackhawk-openapi.json
  format: json
  label: StackHawk API
  slug: stackhawk-api
  spec_type: OpenAPI
  url: https://download.stackhawk.com/openapi/stackhawk-openapi.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Stackhawk Authentication
name_suffix: Authentication
oauth_flows: []
overview: StackHawk secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: StackHawk
provider_slug: stackhawk
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: JWT token obtained via /api/v1/auth/login
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/stackhawk-openapi.yml
  type: http
slug: stackhawk-authentication
source_filename: stackhawk-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/stackhawk-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: JWT token obtained via /api/v1/auth/login\n  sources:\n  - openapi/stackhawk-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/stackhawk/refs/heads/main/authentication/stackhawk-authentication.yml
summary_line: http · 1 scheme
tags:
- API Security
- Application Security
- DAST
- Security Testing
- Vulnerability Management
---
