---
api_key_in:
- header
api_specs:
- filename: openapi.yml
  format: yaml
  label: NOWPayments Payment API
  slug: nowpayments-payment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/now-payments/refs/heads/main/openapi/openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Now Payments Authentication
name_suffix: Authentication
oauth_flows: []
overview: NOWPayments secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: NOWPayments
provider_slug: now-payments
scheme_count: 2
schemes:
- description: NOWPayments API key obtained from your merchant dashboard
  in: header
  name: ApiKeyAuth
  parameter: x-api-key
  sources:
  - openapi/openapi.yml
  type: apiKey
- bearerFormat: JWT
  description: JWT token obtained from the /auth endpoint (required for mass payout operations)
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/openapi.yml
  type: http
slug: now-payments-authentication
source_filename: now-payments-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: NOWPayments API key obtained from your merchant dashboard\n  sources:\n  - openapi/openapi.yml\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: JWT token obtained from the /auth endpoint (required for mass payout operations)\n  sources:\n  - openapi/openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/now-payments/refs/heads/main/authentication/now-payments-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Crypto Payments
- Cryptocurrency
- Payment Gateway
- Invoicing
- Subscriptions
- Mass Payouts
- Bitcoin
- Ethereum
---
