---
api_key_in: []
api_specs:
- filename: turso-platform-api-openapi.yml
  format: yaml
  label: Turso Platform API
  slug: platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/turso/refs/heads/main/openapi/turso-platform-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Turso Authentication
name_suffix: Authentication
oauth_flows: []
overview: Turso secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Turso
provider_slug: turso
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/turso-platform-api-openapi.yml
  type: http
slug: turso-authentication
source_filename: turso-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/turso-platform-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/turso-platform-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/turso/refs/heads/main/authentication/turso-authentication.yml
summary_line: http · 1 scheme
tags:
- Database
- Edge Computing
- SQLite
- Developer Tools
- Multi-tenant
- AI Agents
---
