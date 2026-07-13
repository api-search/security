---
api_key_in: []
api_specs:
- filename: aptargroup-openapi.yaml
  format: yaml
  label: AptarGroup API
  slug: aptargroup-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aptargroup/refs/heads/main/openapi/aptargroup-openapi.yaml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Aptargroup Authentication
name_suffix: Authentication
oauth_flows: []
overview: AptarGroup secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: AptarGroup
provider_slug: aptargroup
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/aptargroup-openapi.yaml
  type: http
slug: aptargroup-authentication
source_filename: aptargroup-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/aptargroup-openapi.yaml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/aptargroup-openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aptargroup/refs/heads/main/authentication/aptargroup-authentication.yml
summary_line: http · 1 scheme
tags:
- Packaging
- Dispensing
- Manufacturing
- Sustainability
- Consumer Goods
- Fortune 1000
---
