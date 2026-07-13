---
api_key_in: []
api_specs:
- filename: veli-openapi.yml
  format: yaml
  label: Veli API
  slug: veli
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/veli/refs/heads/main/openapi/veli-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Veli Authentication
name_suffix: Authentication
oauth_flows: []
overview: Veli secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Veli
provider_slug: veli
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: JWT Bearer token for API authentication
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/veli-openapi.yml
  type: http
slug: veli-authentication
source_filename: veli-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/veli-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: JWT Bearer token for API authentication\n  sources:\n  - openapi/veli-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/veli/refs/heads/main/authentication/veli-authentication.yml
summary_line: http · 1 scheme
tags:
- Crypto
- DeFi
- Finance
- Investment
- Portfolio Management
---
