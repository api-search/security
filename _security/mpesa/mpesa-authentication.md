---
api_key_in: []
api_specs:
- filename: mpesa-account-balance-api-openapi.yml
  format: yaml
  label: M-Pesa (Safaricom Daraja) Account Balance API
  slug: mpesa-account-balance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mpesa/refs/heads/main/openapi/mpesa-account-balance-api-openapi.yml
- filename: mpesa-authorization-api-openapi.yml
  format: yaml
  label: M-Pesa (Safaricom Daraja) Authorization API
  slug: mpesa-authorization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mpesa/refs/heads/main/openapi/mpesa-authorization-api-openapi.yml
- filename: mpesa-b2b-api-openapi.yml
  format: yaml
  label: M-Pesa (Safaricom Daraja) B2B API
  slug: mpesa-b2b-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mpesa/refs/heads/main/openapi/mpesa-b2b-api-openapi.yml
- filename: mpesa-b2c-api-openapi.yml
  format: yaml
  label: M-Pesa (Safaricom Daraja) B2C API
  slug: mpesa-b2c-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mpesa/refs/heads/main/openapi/mpesa-b2c-api-openapi.yml
- filename: mpesa-c2b-api-openapi.yml
  format: yaml
  label: M-Pesa (Safaricom Daraja) C2B API
  slug: mpesa-c2b-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mpesa/refs/heads/main/openapi/mpesa-c2b-api-openapi.yml
- filename: mpesa-dynamic-qr-api-openapi.yml
  format: yaml
  label: M-Pesa (Safaricom Daraja) Dynamic QR API
  slug: mpesa-dynamic-qr-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mpesa/refs/heads/main/openapi/mpesa-dynamic-qr-api-openapi.yml
- filename: mpesa-m-pesa-express-api-openapi.yml
  format: yaml
  label: M-Pesa (Safaricom Daraja) M-Pesa Express API
  slug: mpesa-m-pesa-express-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mpesa/refs/heads/main/openapi/mpesa-m-pesa-express-api-openapi.yml
- filename: mpesa-reversal-api-openapi.yml
  format: yaml
  label: M-Pesa (Safaricom Daraja) Reversal API
  slug: mpesa-reversal-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mpesa/refs/heads/main/openapi/mpesa-reversal-api-openapi.yml
- filename: mpesa-standing-order-api-openapi.yml
  format: yaml
  label: M-Pesa (Safaricom Daraja) Standing Order API
  slug: mpesa-standing-order-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mpesa/refs/heads/main/openapi/mpesa-standing-order-api-openapi.yml
- filename: mpesa-tax-remittance-api-openapi.yml
  format: yaml
  label: M-Pesa (Safaricom Daraja) Tax Remittance API
  slug: mpesa-tax-remittance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mpesa/refs/heads/main/openapi/mpesa-tax-remittance-api-openapi.yml
- filename: mpesa-transaction-status-api-openapi.yml
  format: yaml
  label: M-Pesa (Safaricom Daraja) Transaction Status API
  slug: mpesa-transaction-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mpesa/refs/heads/main/openapi/mpesa-transaction-status-api-openapi.yml
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
- M-PESA
---
