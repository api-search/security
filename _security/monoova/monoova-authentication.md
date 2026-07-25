---
api_key_in: []
api_specs:
- filename: monoova-payments.yml
  format: yaml
  label: Monoova Payments API
  slug: monoova-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/monoova/refs/heads/main/openapi/monoova-payments.yml
- filename: monoova-payto.yml
  format: yaml
  label: Monoova PayTo API
  slug: monoova-payto-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/monoova/refs/heads/main/openapi/monoova-payto.yml
- filename: monoova-cc.yml
  format: yaml
  label: Monoova Card Payments API
  slug: monoova-card-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/monoova/refs/heads/main/openapi/monoova-cc.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Monoova Authentication
name_suffix: Authentication
oauth_flows: []
overview: Monoova secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Monoova
provider_slug: monoova
scheme_count: 2
schemes:
- bearerFormat: JWT
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/monoova-cc.yml
  - openapi/monoova-payto.yml
  type: http
- name: BasicAuth
  scheme: basic
  sources:
  - openapi/monoova-cc.yml
  - openapi/monoova-payments.yml
  - openapi/monoova-payto.yml
  type: http
slug: monoova-authentication
source_filename: monoova-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-24'\nmethod: derived\nsource: openapi/monoova-cc.yml, openapi/monoova-payments.yml, openapi/monoova-payto.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/monoova-cc.yml\n  - openapi/monoova-payto.yml\n- name: BasicAuth\n  type: http\n  scheme: basic\n  sources:\n  - openapi/monoova-cc.yml\n  - openapi/monoova-payments.yml\n  - openapi/monoova-payto.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/monoova/refs/heads/main/authentication/monoova-authentication.yml
summary_line: http · 2 schemes
tags:
- Payments
- Australia
- Real-Time Payments
- NPP
- PayTo
- PayID
- Account-to-Account
- BPAY
- Card Payments
- Money Movement
- Virtual Accounts
- Cross-Border
---
