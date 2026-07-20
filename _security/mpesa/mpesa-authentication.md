---
api_key_in: []
api_specs:
- filename: mpesa-openapi.yml
  format: yaml
  label: M-Pesa Authorization API
  slug: mpesa-authorization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mpesa/refs/heads/main/openapi/mpesa-openapi.yml
- filename: mpesa-openapi.yml
  format: yaml
  label: M-Pesa Express (STK Push) API
  slug: mpesa-express-stk-push-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mpesa/refs/heads/main/openapi/mpesa-openapi.yml
- filename: mpesa-openapi.yml
  format: yaml
  label: M-Pesa Customer To Business (C2B) API
  slug: mpesa-c2b-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mpesa/refs/heads/main/openapi/mpesa-openapi.yml
- filename: mpesa-openapi.yml
  format: yaml
  label: M-Pesa Business To Customer (B2C) API
  slug: mpesa-b2c-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mpesa/refs/heads/main/openapi/mpesa-openapi.yml
- filename: mpesa-openapi.yml
  format: yaml
  label: M-Pesa Business To Business (B2B) API
  slug: mpesa-b2b-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mpesa/refs/heads/main/openapi/mpesa-openapi.yml
- filename: mpesa-openapi.yml
  format: yaml
  label: M-Pesa B2B Express Checkout (USSD Push) API
  slug: mpesa-b2b-express-checkout-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mpesa/refs/heads/main/openapi/mpesa-openapi.yml
- filename: mpesa-openapi.yml
  format: yaml
  label: M-Pesa Transaction Status API
  slug: mpesa-transaction-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mpesa/refs/heads/main/openapi/mpesa-openapi.yml
- filename: mpesa-openapi.yml
  format: yaml
  label: M-Pesa Account Balance API
  slug: mpesa-account-balance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mpesa/refs/heads/main/openapi/mpesa-openapi.yml
- filename: mpesa-openapi.yml
  format: yaml
  label: M-Pesa Reversal API
  slug: mpesa-reversal-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mpesa/refs/heads/main/openapi/mpesa-openapi.yml
- filename: mpesa-openapi.yml
  format: yaml
  label: M-Pesa Dynamic QR Code API
  slug: mpesa-dynamic-qr-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mpesa/refs/heads/main/openapi/mpesa-openapi.yml
- filename: mpesa-openapi.yml
  format: yaml
  label: M-Pesa Tax Remittance API
  slug: mpesa-tax-remittance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mpesa/refs/heads/main/openapi/mpesa-openapi.yml
- filename: mpesa-openapi.yml
  format: yaml
  label: M-Pesa Bill Manager API
  slug: mpesa-bill-manager-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mpesa/refs/heads/main/openapi/mpesa-openapi.yml
- filename: mpesa-openapi.yml
  format: yaml
  label: M-Pesa Ratiba (Standing Order) API
  slug: mpesa-ratiba-standing-order-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mpesa/refs/heads/main/openapi/mpesa-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Mpesa Authentication
name_suffix: Authentication
oauth_flows: []
overview: M-Pesa (Safaricom Daraja) secures its APIs with http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: M-Pesa (Safaricom Daraja)
provider_slug: mpesa
scheme_count: 3
schemes:
- description: Consumer key/secret Basic auth used only against /oauth/v1/generate to obtain a token.
  name: basic_auth
  scheme: basic
  sources:
  - openapi/mpesa-openapi.yml
  type: http
- bearerFormat: OAuth access token
  description: Short-lived OAuth access token presented on all M-Pesa product endpoints.
  name: bearer_token
  scheme: bearer
  sources:
  - openapi/mpesa-openapi.yml
  type: http
- description: Region-specific application-layer credential. Initiator password RSA-encrypted with the M-Pesa public certificate, sent in the SecurityCredential request field on privileged B2C/B2B/Reversal/Balance/Status operations.
  in: body
  name: security_credential
  sources:
  - openapi/mpesa-openapi.yml
  type: apiKey
slug: mpesa-authentication
source_filename: mpesa-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: derived\nsource: openapi/mpesa-openapi.yml\nsummary:\n  types:\n  - http\nnotes: >-\n  Two-step auth. (1) Mint an OAuth access token: GET /oauth/v1/generate?grant_type=client_credentials\n  authenticated with HTTP Basic (consumer key as username, consumer secret as password). The\n  response access_token (valid ~3599s) is then presented as a Bearer token on every other Daraja\n  call. (2) Privileged funds-movement operations (B2C, B2B, Reversal, Account Balance,\n  Transaction Status, Tax Remittance) additionally require a SecurityCredential field: the API\n  initiator's password encrypted with Safaricom's M-Pesa public X.509 certificate (RSA), plus\n  STK Push requires a Base64 Password = Base64(Shortcode + Passkey + Timestamp).\nschemes:\n- name: basic_auth\n  type: http\n  scheme: basic\n  description: Consumer key/secret Basic auth used only against /oauth/v1/generate to obtain a token.\n  sources:\n  - openapi/mpesa-openapi.yml\n- name:\
  \ bearer_token\n  type: http\n  scheme: bearer\n  bearerFormat: OAuth access token\n  description: Short-lived OAuth access token presented on all M-Pesa product endpoints.\n  sources:\n  - openapi/mpesa-openapi.yml\n- name: security_credential\n  type: apiKey\n  in: body\n  description: >-\n    Region-specific application-layer credential. Initiator password RSA-encrypted with the\n    M-Pesa public certificate, sent in the SecurityCredential request field on privileged\n    B2C/B2B/Reversal/Balance/Status operations.\n  sources:\n  - openapi/mpesa-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mpesa/refs/heads/main/authentication/mpesa-authentication.yml
summary_line: http · 3 schemes
tags:
- Mobile Money
- Payments
- Fintech
- Kenya
- Africa
- M-Pesa
---
