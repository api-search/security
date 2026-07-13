---
api_key_in: []
api_specs:
- filename: highline-fi-openapi.yml
  format: yaml
  label: Highline Pay by Paycheck API
  slug: pay-by-paycheck-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/highline-fi/refs/heads/main/openapi/highline-fi-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Highline Fi Authentication
name_suffix: Authentication
oauth_flows: []
overview: Highline secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Highline
provider_slug: highline-fi
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/highline-fi-openapi.yml
  type: http
slug: highline-fi-authentication
source_filename: highline-fi-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/highline-fi-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/highline-fi-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/highline-fi/refs/heads/main/authentication/highline-fi-authentication.yml
summary_line: http · 1 scheme
tags:
- Embedded Finance
- Payroll
- Payments
- ACH
- Bill Pay
- Lending
- Direct Deposit
- API-First
- Webhooks
- Pay by Paycheck
---
