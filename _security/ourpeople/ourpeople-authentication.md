---
api_key_in: []
api_specs:
- filename: ourpeople-openapi.yml
  format: yaml
  label: OurPeople API
  slug: ourpeople-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ourpeople/refs/heads/main/openapi/ourpeople-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Ourpeople Authentication
name_suffix: Authentication
oauth_flows: []
overview: OurPeople secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: OurPeople
provider_slug: ourpeople
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/ourpeople-openapi.yml
  type: http
slug: ourpeople-authentication
source_filename: ourpeople-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/ourpeople-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/ourpeople-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ourpeople/refs/heads/main/authentication/ourpeople-authentication.yml
summary_line: http · 1 scheme
tags:
- Communications
- Workforce
- Frontline
---
