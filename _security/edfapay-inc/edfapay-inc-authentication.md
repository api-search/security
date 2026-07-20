---
api_key_in:
- header
api_specs:
- filename: edfapay-inc-revamp.json
  format: json
  label: EdfaPay Management API
  slug: edfapay-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/edfapay-inc/refs/heads/main/openapi/edfapay-inc-revamp.json
- filename: edfapay-inc-payment-initiate.json
  format: json
  label: EdfaPay Payment Gateway API
  slug: edfapay-payment-gateway-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/edfapay-inc/refs/heads/main/openapi/edfapay-inc-payment-initiate.json
auth_types:
- apiKey
- signature
description: ''
kind: authentication
layout: security
method: searched
name: Edfapay Inc Authentication
name_suffix: Authentication
oauth_flows: []
overview: EdfaPay, Inc. secures its APIs with apiKey and signature across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: EdfaPay, Inc.
provider_slug: edfapay-inc
scheme_count: 2
schemes:
- description: API Key passed in the X-API-KEY request header for the management/dashboard API (revamp-api). Keys are scoped to a caller type (ADMIN, PARTNER, MERCHANT, USER).
  in: header
  name: apiKey
  parameter: X-API-KEY
  sources:
  - openapi/edfapay-inc-revamp.json
  type: apiKey
- credentials:
  - client_key
  - password
  description: The payment-gateway (Checkout / Server-to-Server) API authenticates each request with a per-request MD5 hash signature computed from the merchant credentials. Merchants receive a client_key and password on onboarding; the hash is MD5( reverse(payer_email) + password + reverse(first6+last4 of card number) ), uppercased. Webhook payloads carry the same hash for verification.
  in: body
  name: signature-hash
  parameter: hash
  sources:
  - https://docs.edfapay.com/docs/sandbox-environment
  - https://docs.edfapay.com/docs/production-environment-1
  type: signature
slug: edfapay-inc-authentication
source_filename: edfapay-inc-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: openapi/edfapay-inc-revamp.json + https://docs.edfapay.com/docs/sandbox-environment\ndocs: https://docs.edfapay.com/docs/sandbox-environment\nsummary:\n  types:\n  - apiKey\n  - signature\n  api_key_in:\n  - header\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: X-API-KEY\n  description: >-\n    API Key passed in the X-API-KEY request header for the management/dashboard\n    API (revamp-api). Keys are scoped to a caller type (ADMIN, PARTNER, MERCHANT,\n    USER).\n  sources:\n  - openapi/edfapay-inc-revamp.json\n- name: signature-hash\n  type: signature\n  in: body\n  parameter: hash\n  description: >-\n    The payment-gateway (Checkout / Server-to-Server) API authenticates each\n    request with a per-request MD5 hash signature computed from the merchant\n    credentials. Merchants receive a client_key and password on onboarding; the\n    hash is MD5( reverse(payer_email) + password + reverse(first6+last4\
  \ of card\n    number) ), uppercased. Webhook payloads carry the same hash for\n    verification.\n  credentials:\n  - client_key\n  - password\n  sources:\n  - https://docs.edfapay.com/docs/sandbox-environment\n  - https://docs.edfapay.com/docs/production-environment-1\nnotes: >-\n  Two distinct surfaces. (1) The management API (revamp-api.edfapay.com) uses an\n  X-API-KEY header. (2) The payment gateway (api.edfapay.com) uses signed\n  requests with a client_key/password-derived MD5 hash; there is no OAuth 2.0\n  flow published.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/edfapay-inc/refs/heads/main/authentication/edfapay-inc-authentication.yml
summary_line: apiKey/signature · 2 schemes
tags:
- Company
- Payments
- Payment Gateway
- Fintech
- SoftPOS
- Apple Pay
- Saudi Arabia
- Merchant Onboarding
---
