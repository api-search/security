---
api_key_in:
- header
api_specs:
- filename: S1a32n38
  format: yaml
  label: NOWPayments Mass Payouts API
  slug: nowpayments-mass-payouts-api
  spec_type: Postman
  url: https://documenter.getpostman.com/view/7907941/S1a32n38
- filename: now-payments-authentication-api-openapi.yml
  format: yaml
  label: NOWPayments Authentication API
  slug: now-payments-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/now-payments/refs/heads/main/openapi/now-payments-authentication-api-openapi.yml
- filename: now-payments-currencies-api-openapi.yml
  format: yaml
  label: NOWPayments Currencies API
  slug: now-payments-currencies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/now-payments/refs/heads/main/openapi/now-payments-currencies-api-openapi.yml
- filename: now-payments-estimates-api-openapi.yml
  format: yaml
  label: NOWPayments Estimates API
  slug: now-payments-estimates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/now-payments/refs/heads/main/openapi/now-payments-estimates-api-openapi.yml
- filename: now-payments-invoices-api-openapi.yml
  format: yaml
  label: NOWPayments Invoices API
  slug: now-payments-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/now-payments/refs/heads/main/openapi/now-payments-invoices-api-openapi.yml
- filename: now-payments-payments-api-openapi.yml
  format: yaml
  label: NOWPayments Payments API
  slug: now-payments-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/now-payments/refs/heads/main/openapi/now-payments-payments-api-openapi.yml
- filename: now-payments-payouts-api-openapi.yml
  format: yaml
  label: NOWPayments Payouts API
  slug: now-payments-payouts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/now-payments/refs/heads/main/openapi/now-payments-payouts-api-openapi.yml
- filename: now-payments-status-api-openapi.yml
  format: yaml
  label: NOWPayments Status API
  slug: now-payments-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/now-payments/refs/heads/main/openapi/now-payments-status-api-openapi.yml
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
