---
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Wove Authentication
name_suffix: Authentication
oauth_flows: []
overview: Wove secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Wove
provider_slug: wove
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: OAuth 2.0 Bearer token obtained from /auth/token endpoint
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/wove-external-api-openapi-original.yml
  type: http
slug: wove-authentication
source_filename: wove-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: derived\nsource: openapi/wove-external-api-openapi-original.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: OAuth 2.0 Bearer token obtained from /auth/token endpoint\n  sources:\n  - openapi/wove-external-api-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wove/refs/heads/main/authentication/wove-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
---
