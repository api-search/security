---
api_key_in: []
api_specs:
- filename: ssc-geneva-fund-accounting-openapi.yml
  format: yaml
  label: SS&C Geneva Fund Accounting API
  slug: ssc-geneva-fund-accounting
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ssc-geneva/refs/heads/main/openapi/ssc-geneva-fund-accounting-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Ssc Geneva Authentication
name_suffix: Authentication
oauth_flows: []
overview: SS&C Geneva secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: SS&C Geneva
provider_slug: ssc-geneva
scheme_count: 2
schemes:
- bearerFormat: JWT
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/ssc-geneva-fund-accounting-openapi.yml
  type: http
- name: BasicAuth
  scheme: basic
  sources:
  - openapi/ssc-geneva-fund-accounting-openapi.yml
  type: http
slug: ssc-geneva-authentication
source_filename: ssc-geneva-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/ssc-geneva-fund-accounting-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/ssc-geneva-fund-accounting-openapi.yml\n- name: BasicAuth\n  type: http\n  scheme: basic\n  sources:\n  - openapi/ssc-geneva-fund-accounting-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ssc-geneva/refs/heads/main/authentication/ssc-geneva-authentication.yml
summary_line: http · 2 schemes
tags:
- Fund Accounting
- Asset Management
- Portfolio Management
- Financial Services
- Hedge Funds
- NAV Calculation
---
