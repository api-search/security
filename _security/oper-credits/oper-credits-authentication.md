---
api_key_in: []
api_specs:
- filename: oper-credits-api-openapi.json
  format: json
  label: Oper Mortgage API
  slug: oper-mortgage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oper-credits/refs/heads/main/openapi/oper-credits-api-openapi.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Oper Credits Authentication
name_suffix: Authentication
oauth_flows: []
overview: Oper Credits secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Oper Credits
provider_slug: oper-credits
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: jwtAuth
  scheme: bearer
  sources:
  - openapi/oper-credits-api-openapi.json
  - openapi/oper-credits-metrics-openapi.json
  - openapi/oper-credits-resources-openapi.json
  type: http
slug: oper-credits-authentication
source_filename: oper-credits-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: derived\nsource: openapi/oper-credits-api-openapi.json, openapi/oper-credits-metrics-openapi.json, openapi/oper-credits-resources-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: jwtAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/oper-credits-api-openapi.json\n  - openapi/oper-credits-metrics-openapi.json\n  - openapi/oper-credits-resources-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/oper-credits/refs/heads/main/authentication/oper-credits-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Mortgages
- Lending
- Credit
- Fintech
- Banking
- Loan Origination
- Real Estate
- Financial Services
---
