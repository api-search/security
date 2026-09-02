---
api_key_in: []
api_specs:
- filename: turso-auth-api-openapi.yml
  format: yaml
  label: Turso Auth API
  slug: turso-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/turso/refs/heads/main/openapi/turso-auth-api-openapi.yml
- filename: turso-locations-api-openapi.yml
  format: yaml
  label: Turso Locations API
  slug: turso-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/turso/refs/heads/main/openapi/turso-locations-api-openapi.yml
- filename: turso-organizations-api-openapi.yml
  format: yaml
  label: Turso Organizations API
  slug: turso-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/turso/refs/heads/main/openapi/turso-organizations-api-openapi.yml
- filename: turso-user-api-openapi.yml
  format: yaml
  label: Turso User API
  slug: turso-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/turso/refs/heads/main/openapi/turso-user-api-openapi.yml
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
- Multi-Tenant
- AI Agents
---
