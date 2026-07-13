---
api_key_in: []
api_specs:
- filename: contentsquare-openapi.yml
  format: yaml
  label: Contentsquare Data Export API
  slug: data-export-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/contentsquare/refs/heads/main/openapi/contentsquare-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Contentsquare Authentication
name_suffix: Authentication
oauth_flows: []
overview: Contentsquare secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Contentsquare
provider_slug: contentsquare
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/contentsquare-openapi.yml
  type: http
slug: contentsquare-authentication
source_filename: contentsquare-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/contentsquare-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/contentsquare-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/contentsquare/refs/heads/main/authentication/contentsquare-authentication.yml
summary_line: http · 1 scheme
tags:
- Digital Experience Analytics
- Product Analytics
- Session Replay
- Heatmaps
- Customer Experience
- Conversion Optimization
- User Behavior
---
