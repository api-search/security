---
api_key_in: []
api_specs:
- filename: rtx-eagle-api-openapi.yml
  format: yaml
  label: RTX EAGLE API
  slug: eagle-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rtx/refs/heads/main/openapi/rtx-eagle-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Rtx Authentication
name_suffix: Authentication
oauth_flows: []
overview: RTX secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: RTX
provider_slug: rtx
scheme_count: 1
schemes:
- name: bearerAuth
  scheme: bearer
  sources:
  - openapi/rtx-eagle-api-openapi.yml
  type: http
slug: rtx-authentication
source_filename: rtx-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/rtx-eagle-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/rtx-eagle-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rtx/refs/heads/main/authentication/rtx-authentication.yml
summary_line: http · 1 scheme
tags:
- Defense
- Aerospace
- Government
- Logistics
- Intelligence
- Military
---
