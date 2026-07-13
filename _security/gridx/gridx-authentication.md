---
api_key_in: []
api_specs:
- filename: gridx-openapi.yml
  format: yaml
  label: GridX Rate Engine API
  slug: gridx-rate-engine-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gridx/refs/heads/main/openapi/gridx-openapi.yml
- filename: gridx-openapi.yml
  format: yaml
  label: GridX Bill Calculation API
  slug: gridx-bill-calculation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gridx/refs/heads/main/openapi/gridx-openapi.yml
- filename: gridx-openapi.yml
  format: yaml
  label: GridX Rate Analytics API
  slug: gridx-rate-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gridx/refs/heads/main/openapi/gridx-openapi.yml
- filename: gridx-openapi.yml
  format: yaml
  label: GridX OpenADR Programs API
  slug: gridx-openadr-programs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gridx/refs/heads/main/openapi/gridx-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Gridx Authentication
name_suffix: Authentication
oauth_flows: []
overview: GridX secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: GridX
provider_slug: gridx
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: JWT bearer token obtained from the /token endpoint (expires ~1 hour).
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/gridx-openapi.yml
  type: http
slug: gridx-authentication
source_filename: gridx-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/gridx-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: JWT bearer token obtained from the /token endpoint (expires ~1 hour).\n  sources:\n  - openapi/gridx-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gridx/refs/heads/main/authentication/gridx-authentication.yml
summary_line: http · 1 scheme
tags:
- Energy
- Utilities
- Rate Engine
- Billing
- Rate Analytics
---
