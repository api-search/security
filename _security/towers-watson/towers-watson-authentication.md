---
api_key_in: []
api_specs:
- filename: wtw-hr-portal-openapi.yml
  format: yaml
  label: WTW HR Portal
  slug: wtw-hr-portal
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/towers-watson/refs/heads/main/openapi/wtw-hr-portal-openapi.yml
- filename: wtw-benefits-administration-openapi.yml
  format: yaml
  label: WTW Benefits Administration
  slug: wtw-benefits-administration
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/towers-watson/refs/heads/main/openapi/wtw-benefits-administration-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Towers Watson Authentication
name_suffix: Authentication
oauth_flows: []
overview: Towers Watson secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Towers Watson
provider_slug: towers-watson
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/wtw-hr-portal-openapi.yml
  type: http
slug: towers-watson-authentication
source_filename: towers-watson-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/wtw-hr-portal-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/wtw-hr-portal-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/towers-watson/refs/heads/main/authentication/towers-watson-authentication.yml
summary_line: http · 1 scheme
tags:
- Human Resources
- Risk Management
- Benefits
- Consulting
- Actuarial
- Insurance Brokerage
- Human Capital
---
