---
api_key_in: []
api_specs:
- filename: squillo-platform-openapi.yml
  format: yaml
  label: Squillo Platform API
  slug: squillo-platform
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/squillo/refs/heads/main/openapi/squillo-platform-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Squillo Authentication
name_suffix: Authentication
oauth_flows: []
overview: Squillo secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Squillo
provider_slug: squillo
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/squillo-platform-openapi.yml
  type: http
slug: squillo-authentication
source_filename: squillo-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/squillo-platform-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/squillo-platform-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/squillo/refs/heads/main/authentication/squillo-authentication.yml
summary_line: http · 1 scheme
tags:
- Integration Platform
- Automation
- Workflow
- No-Code
- IT Process Automation
- Software As A Utility
---
