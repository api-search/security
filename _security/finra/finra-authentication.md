---
api_key_in: []
api_specs:
- filename: finra-openapi.yml
  format: yaml
  label: FINRA Query API
  slug: query-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/finra/refs/heads/main/openapi/finra-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Finra Authentication
name_suffix: Authentication
oauth_flows: []
overview: FINRA secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: FINRA
provider_slug: finra
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/finra-openapi.yml
  type: http
slug: finra-authentication
source_filename: finra-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/finra-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/finra-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/finra/refs/heads/main/authentication/finra-authentication.yml
summary_line: http · 1 scheme
tags:
- Compliance
- Financial
- Regulations
- Securities
- Market Data
---
