---
api_key_in: []
api_specs:
- filename: opay-cashier-api-openapi.yml
  format: yaml
  label: OPay Cashier API
  slug: opay-cashier-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opay/refs/heads/main/openapi/opay-cashier-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Opay Authentication
name_suffix: Authentication
oauth_flows: []
overview: OPay secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: OPay
provider_slug: opay
scheme_count: 1
schemes:
- description: Bearer token = merchant public key (used for cashier/create).
  name: PublicKeyAuth
  scheme: bearer
  sources:
  - openapi/opay-cashier-api-openapi.yml
  type: http
slug: opay-authentication
source_filename: opay-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/opay-cashier-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: PublicKeyAuth\n  type: http\n  scheme: bearer\n  description: Bearer token = merchant public key (used for cashier/create).\n  sources:\n  - openapi/opay-cashier-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/opay/refs/heads/main/authentication/opay-authentication.yml
summary_line: http · 1 scheme
tags:
- Payments
- Mobile Money
- Fintech
- Super App
- Nigeria
- Africa
- Wallet
- Savings
- BNPL
- Bank Transfer
- Card Payments
- USSD
- Agent Banking
- POS
- Bill Payments
- Airtime
- Cashier
- Checkout
- Merchant Acquiring
---
