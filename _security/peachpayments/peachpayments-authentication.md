---
api_key_in: []
api_specs:
- filename: peachpayments-authentication-api-openapi.yml
  format: yaml
  label: Peach Payments Authentication API
  slug: peachpayments-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/peachpayments/refs/heads/main/openapi/peachpayments-authentication-api-openapi.yml
- filename: peachpayments-checkout-api-openapi.yml
  format: yaml
  label: Peach Payments Checkout API
  slug: peachpayments-checkout-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/peachpayments/refs/heads/main/openapi/peachpayments-checkout-api-openapi.yml
- filename: peachpayments-payment-links-api-openapi.yml
  format: yaml
  label: Peach Payments Payment Links API
  slug: peachpayments-payment-links-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/peachpayments/refs/heads/main/openapi/peachpayments-payment-links-api-openapi.yml
- filename: peachpayments-payments-api-openapi.yml
  format: yaml
  label: Peach Payments Payments API
  slug: peachpayments-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/peachpayments/refs/heads/main/openapi/peachpayments-payments-api-openapi.yml
- filename: peachpayments-payouts-api-openapi.yml
  format: yaml
  label: Peach Payments Payouts API
  slug: peachpayments-payouts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/peachpayments/refs/heads/main/openapi/peachpayments-payouts-api-openapi.yml
- filename: peachpayments-reconciliation-api-openapi.yml
  format: yaml
  label: Peach Payments Reconciliation API
  slug: peachpayments-reconciliation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/peachpayments/refs/heads/main/openapi/peachpayments-reconciliation-api-openapi.yml
auth_types:
- http
- inline-credentials
description: ''
kind: authentication
layout: security
method: searched
name: Peachpayments Authentication
name_suffix: Authentication
oauth_flows: []
overview: Peach Payments secures its APIs with http and inline-credentials across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Peach Payments
provider_slug: peachpayments
scheme_count: 3
schemes:
- bearerFormat: JWT
  name: oauth_bearer
  notes: 'Checkout, Payment Links, Payouts, and Reconciliation use OAuth 2.0 client-credentials. POST clientId + clientSecret + merchantId to {peach-auth-service}/api/oauth/token (sandbox-dashboard.peachpayments.com for sandbox, dashboard.peachpayments.com for live) to obtain a short-lived access_token, then send Authorization: Bearer {access_token}. An entityId scopes the merchant channel, currencies, and payment methods.'
  scheme: bearer
  sources:
  - openapi/peachpayments-openapi.yml
  type: http
- in: body
  name: payments_inline_auth
  notes: The server-to-server Payments API does not use the OAuth Bearer flow; it accepts an inline authentication object of userId, password, and entityId in the request body.
  scheme: inline-credentials
  sources:
  - openapi/peachpayments-openapi.yml
  type: apiKey
- name: checkout_signature
  notes: Legacy/Hosted Checkout V1 additionally supports HMAC SHA-256 request signing using a shared secret token from the Peach Payments Dashboard.
  scheme: hmac-sha256
  sources:
  - https://developer.peachpayments.com/docs/checkout-authentication
  type: hmac
slug: peachpayments-authentication
source_filename: peachpayments-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: searched\nsource: openapi/peachpayments-openapi.yml\ndocs: https://developer.peachpayments.com/docs/checkout-embedded-authentication\nsummary:\n  types:\n  - http\n  - inline-credentials\nschemes:\n- name: oauth_bearer\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/peachpayments-openapi.yml\n  notes: >-\n    Checkout, Payment Links, Payouts, and Reconciliation use OAuth 2.0\n    client-credentials. POST clientId + clientSecret + merchantId to\n    {peach-auth-service}/api/oauth/token (sandbox-dashboard.peachpayments.com\n    for sandbox, dashboard.peachpayments.com for live) to obtain a\n    short-lived access_token, then send Authorization: Bearer {access_token}.\n    An entityId scopes the merchant channel, currencies, and payment methods.\n- name: payments_inline_auth\n  type: apiKey\n  in: body\n  scheme: inline-credentials\n  sources:\n  - openapi/peachpayments-openapi.yml\n  notes: >-\n    The server-to-server\
  \ Payments API does not use the OAuth Bearer flow;\n    it accepts an inline authentication object of userId, password, and\n    entityId in the request body.\n- name: checkout_signature\n  type: hmac\n  scheme: hmac-sha256\n  sources:\n  - https://developer.peachpayments.com/docs/checkout-authentication\n  notes: >-\n    Legacy/Hosted Checkout V1 additionally supports HMAC SHA-256 request\n    signing using a shared secret token from the Peach Payments Dashboard.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/peachpayments/refs/heads/main/authentication/peachpayments-authentication.yml
summary_line: http/inline-credentials · 3 schemes
tags:
- Payments
- Fintech
- Africa
- Payment Gateway
- Checkout
- Payouts
---
