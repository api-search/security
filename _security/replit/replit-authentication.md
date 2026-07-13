---
api_key_in: []
api_specs:
- filename: replit-openapi.yml
  format: yaml
  label: Replit
  slug: replit
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/replit/refs/heads/main/openapi/replit-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Replit Authentication
name_suffix: Authentication
oauth_flows: []
overview: Replit secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Replit
provider_slug: replit
scheme_count: 1
schemes:
- bearerFormat: API Token from https://replit.com/account#api-tokens
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/replit-openapi.yml
  type: http
slug: replit-authentication
source_filename: replit-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/replit-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: API Token from https://replit.com/account#api-tokens\n  sources:\n  - openapi/replit-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/replit/refs/heads/main/authentication/replit-authentication.yml
summary_line: http · 1 scheme
tags:
- Code
- Compiling
- Development Environment
- Programming Languages
- Version Control
---
