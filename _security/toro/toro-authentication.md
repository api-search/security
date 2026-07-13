---
api_key_in:
- header
api_specs:
- filename: toro-horizon360-openapi.yml
  format: yaml
  label: Toro Horizon360
  slug: horizon360
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toro/refs/heads/main/openapi/toro-horizon360-openapi.yml
- filename: toro-intellidash-openapi.yml
  format: yaml
  label: Toro IntelliDash
  slug: intellidash
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toro/refs/heads/main/openapi/toro-intellidash-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Toro Authentication
name_suffix: Authentication
oauth_flows: []
overview: Toro secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Toro
provider_slug: toro
scheme_count: 2
schemes:
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/toro-horizon360-openapi.yml
  type: http
- in: header
  name: apiKeyAuth
  parameter: X-API-Key
  sources:
  - openapi/toro-intellidash-openapi.yml
  type: apiKey
slug: toro-authentication
source_filename: toro-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/toro-horizon360-openapi.yml, openapi/toro-intellidash-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/toro-horizon360-openapi.yml\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  sources:\n  - openapi/toro-intellidash-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/toro/refs/heads/main/authentication/toro-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Landscaping
- Irrigation
- Golf
- Equipment
- Smart Connected Products
- Fleet Management
- Turf Management
- Fortune 1000
---
