---
api_key_in: []
api_specs:
- filename: aloft-openapi-original.json
  format: json
  label: Aloft API V1
  slug: aloft-api-v1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aloft/refs/heads/main/openapi/aloft-openapi-original.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Aloft Authentication
name_suffix: Authentication
oauth_flows: []
overview: Aloft secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Aloft
provider_slug: aloft
scheme_count: 1
schemes:
- name: Aloft Token
  scheme: bearer
  sources:
  - openapi/aloft-openapi-original.json
  type: http
slug: aloft-authentication
source_filename: aloft-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: openapi/aloft-openapi-original.json\ndocs: https://www.aloft.ai/developer/\nsummary:\n  types:\n  - http\n  http_scheme: bearer\n  credential: Aloft Token\n  header: Authorization\n  note: >-\n    Aloft issues a per-integration API key (Aloft Token) provided on request; it\n    is sent as an http bearer credential in the Authorization header. Requests\n    are scoped to an account_id.\nschemes:\n- name: Aloft Token\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/aloft-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aloft/refs/heads/main/authentication/aloft-authentication.yml
summary_line: http · 1 scheme
tags:
- Drones
- Airspace
- UTM
- LAANC
- Aviation
- Fleet Management
- Geospatial
- Public Safety
---
