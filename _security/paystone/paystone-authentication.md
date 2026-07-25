---
api_key_in: []
api_specs:
- filename: paystone-datacandy-openapi.yml
  format: yaml
  label: Paystone DataCandy API
  slug: paystone-datacandy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paystone/refs/heads/main/openapi/paystone-datacandy-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Paystone Authentication
name_suffix: Authentication
oauth_flows: []
overview: Paystone secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Paystone
provider_slug: paystone
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: Enter your JWT token (without the "Bearer" prefix).
  name: JWT
  scheme: bearer
  sources:
  - openapi/paystone-datacandy-openapi.yml
  type: http
slug: paystone-authentication
source_filename: paystone-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-24'\nmethod: derived\nsource: openapi/paystone-datacandy-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: JWT\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: Enter your JWT token (without the \"Bearer\" prefix).\n  sources:\n  - openapi/paystone-datacandy-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/paystone/refs/heads/main/authentication/paystone-authentication.yml
summary_line: http · 1 scheme
tags:
- Payments
- Canada
- Payment Processing
- Acquiring
- Gift Cards
- Loyalty
- Subscriptions
- Billing
- Merchant Services
---
