---
api_key_in: []
api_specs:
- filename: wincl-openapi-original.json
  format: json
  label: Wincl API
  slug: wincl-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wincl/refs/heads/main/openapi/wincl-openapi-original.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Wincl Authentication
name_suffix: Authentication
oauth_flows: []
overview: WinCL secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: WinCL
provider_slug: wincl
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: Bearer 토큰 값
  scheme: bearer
  sources:
  - openapi/wincl-openapi-original.json
  type: http
slug: wincl-authentication
source_filename: wincl-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: derived\nsource: openapi/wincl-openapi-original.json\nsummary:\n  types:\n  - http\nschemes:\n- name: Bearer 토큰 값\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/wincl-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wincl/refs/heads/main/authentication/wincl-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Carbon Management
- Sustainability
- Greenhouse Gas
- Carbon Credits
- Carbon Offset
- ESG
- Climate
- Marketplace
- Payments
- Blockchain
- Hedera
---
