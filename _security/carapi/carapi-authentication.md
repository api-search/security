---
api_key_in: []
api_specs:
- filename: carapi-openapi.yml
  format: yaml
  label: CarAPI
  slug: carapi
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/carapi/refs/heads/main/openapi/carapi-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Carapi Authentication
name_suffix: Authentication
oauth_flows: []
overview: CarAPI secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: CarAPI
provider_slug: carapi
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: JWT bearer token obtained from /api/auth/login.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/carapi-openapi.yml
  type: http
slug: carapi-authentication
source_filename: carapi-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/carapi-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: JWT bearer token obtained from /api/auth/login.\n  sources:\n  - openapi/carapi-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/carapi/refs/heads/main/authentication/carapi-authentication.yml
summary_line: http · 1 scheme
tags:
- Automobiles
- Vehicles
---
