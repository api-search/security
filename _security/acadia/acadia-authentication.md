---
api_key_in: []
api_specs:
- filename: acadia-platform.yaml
  format: yaml
  label: Acadia Platform API
  slug: acadia-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/acadia/refs/heads/main/openapi/acadia-platform.yaml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Acadia Authentication
name_suffix: Authentication
oauth_flows: []
overview: Acadia secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Acadia
provider_slug: acadia
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: JWT Bearer token for API authentication
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/acadia-platform.yaml
  type: http
slug: acadia-authentication
source_filename: acadia-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/acadia-platform.yaml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: JWT Bearer token for API authentication\n  sources:\n  - openapi/acadia-platform.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/acadia/refs/heads/main/authentication/acadia-authentication.yml
summary_line: http · 1 scheme
tags:
- Connected Worker
- Knowledge Management
- Manufacturing
- Skills Management
- Training
- Workforce Development
---
