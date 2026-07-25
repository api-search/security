---
api_key_in: []
api_specs:
- filename: api-fiddle-export-api-openapi.yml
  format: yaml
  label: API-Fiddle Export API
  slug: api-fiddle-export-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/api-fiddle/refs/heads/main/openapi/api-fiddle-export-api-openapi.yml
- filename: api-fiddle-projects-api-openapi.yml
  format: yaml
  label: API-Fiddle Projects API
  slug: api-fiddle-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/api-fiddle/refs/heads/main/openapi/api-fiddle-projects-api-openapi.yml
- filename: api-fiddle-sharing-api-openapi.yml
  format: yaml
  label: API-Fiddle Sharing API
  slug: api-fiddle-sharing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/api-fiddle/refs/heads/main/openapi/api-fiddle-sharing-api-openapi.yml
- filename: api-fiddle-specifications-api-openapi.yml
  format: yaml
  label: API-Fiddle Specifications API
  slug: api-fiddle-specifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/api-fiddle/refs/heads/main/openapi/api-fiddle-specifications-api-openapi.yml
- filename: api-fiddle-workspaces-api-openapi.yml
  format: yaml
  label: API-Fiddle Workspaces API
  slug: api-fiddle-workspaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/api-fiddle/refs/heads/main/openapi/api-fiddle-workspaces-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Api Fiddle Authentication
name_suffix: Authentication
oauth_flows: []
overview: API-Fiddle secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: API-Fiddle
provider_slug: api-fiddle
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/api-fiddle-api-fiddle-openapi.yml
  type: http
slug: api-fiddle-authentication
source_filename: api-fiddle-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/api-fiddle-api-fiddle-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/api-fiddle-api-fiddle-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/api-fiddle/refs/heads/main/authentication/api-fiddle-authentication.yml
summary_line: http · 1 scheme
tags:
- API Design
- OpenAPI
- Collaboration
- Documentation
- Platform
---
