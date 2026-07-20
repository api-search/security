---
api_key_in: []
api_specs:
- filename: arch-client-api-openapi.json
  format: json
  label: Arch Client API
  slug: arch-client-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arch/refs/heads/main/openapi/arch-client-api-openapi.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Arch Authentication
name_suffix: Authentication
oauth_flows: []
overview: Arch secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Arch
provider_slug: arch
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/arch-client-api-openapi.json
  type: http
slug: arch-authentication
source_filename: arch-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: derived\nsource: openapi/arch-client-api-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/arch-client-api-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/arch/refs/heads/main/authentication/arch-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Private Markets
- Alternative Investments
- Fintech
- Wealth Management
- Investment Administration
- Portfolio Management
- Documents
---
