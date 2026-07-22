---
api_key_in:
- header
api_specs:
- filename: vivenu-openapi-original.json
  format: json
  label: vivenu API
  slug: vivenu-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vivenu/refs/heads/main/openapi/vivenu-openapi-original.json
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Vivenu Authentication
name_suffix: Authentication
oauth_flows: []
overview: vivenu secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: vivenu
provider_slug: vivenu
scheme_count: 2
schemes:
- bearerFormat: JWT
  name: jwt
  scheme: bearer
  sources:
  - openapi/vivenu-openapi-original.json
  type: http
- in: header
  name: apikey
  parameter: Authorization
  sources:
  - openapi/vivenu-openapi-original.json
  type: apiKey
slug: vivenu-authentication
source_filename: vivenu-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: derived\nsource: openapi/vivenu-openapi-original.json\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: jwt\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/vivenu-openapi-original.json\n- name: apikey\n  type: apiKey\n  in: header\n  parameter: Authorization\n  sources:\n  - openapi/vivenu-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vivenu/refs/heads/main/authentication/vivenu-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Company
- Event Ticketing
- Ticketing
- Events
- Payments
- Live Entertainment
- Webhooks
- API-first
---
