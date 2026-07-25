---
api_key_in:
- header
api_specs:
- filename: paymob-intentions-api-openapi.yml
  format: yaml
  label: Paymob Intentions API
  slug: paymob-intentions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paymob/refs/heads/main/openapi/paymob-intentions-api-openapi.yml
- filename: paymob-subscriptions-api-openapi.yml
  format: yaml
  label: Paymob Subscriptions API
  slug: paymob-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paymob/refs/heads/main/openapi/paymob-subscriptions-api-openapi.yml
- filename: paymob-card-tokens-api-openapi.yml
  format: yaml
  label: Paymob Card Tokens API
  slug: paymob-card-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paymob/refs/heads/main/openapi/paymob-card-tokens-api-openapi.yml
- filename: paymob-accounts-api-openapi.yml
  format: yaml
  label: Paymob Accounts API
  slug: paymob-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paymob/refs/heads/main/openapi/paymob-accounts-api-openapi.yml
- filename: paymob-authentication-api-openapi.yml
  format: yaml
  label: Paymob Authentication API
  slug: paymob-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paymob/refs/heads/main/openapi/paymob-authentication-api-openapi.yml
- filename: paymob-capture-api-openapi.yml
  format: yaml
  label: Paymob Capture API
  slug: paymob-capture-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paymob/refs/heads/main/openapi/paymob-capture-api-openapi.yml
- filename: paymob-checkout-api-openapi.yml
  format: yaml
  label: Paymob Checkout API
  slug: paymob-checkout-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paymob/refs/heads/main/openapi/paymob-checkout-api-openapi.yml
- filename: paymob-disbursement-api-openapi.yml
  format: yaml
  label: Paymob Disbursement API
  slug: paymob-disbursement-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paymob/refs/heads/main/openapi/paymob-disbursement-api-openapi.yml
- filename: paymob-orders-api-openapi.yml
  format: yaml
  label: Paymob Orders API
  slug: paymob-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paymob/refs/heads/main/openapi/paymob-orders-api-openapi.yml
- filename: paymob-payment-keys-api-openapi.yml
  format: yaml
  label: Paymob Payment Keys API
  slug: paymob-payment-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paymob/refs/heads/main/openapi/paymob-payment-keys-api-openapi.yml
- filename: paymob-payment-links-api-openapi.yml
  format: yaml
  label: Paymob Payment Links API
  slug: paymob-payment-links-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paymob/refs/heads/main/openapi/paymob-payment-links-api-openapi.yml
- filename: paymob-payments-api-openapi.yml
  format: yaml
  label: Paymob Payments API
  slug: paymob-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paymob/refs/heads/main/openapi/paymob-payments-api-openapi.yml
- filename: paymob-refund-api-openapi.yml
  format: yaml
  label: Paymob Refund API
  slug: paymob-refund-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paymob/refs/heads/main/openapi/paymob-refund-api-openapi.yml
- filename: paymob-saved-card-payments-api-openapi.yml
  format: yaml
  label: Paymob Saved Card Payments API
  slug: paymob-saved-card-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paymob/refs/heads/main/openapi/paymob-saved-card-payments-api-openapi.yml
- filename: paymob-subscription-plans-api-openapi.yml
  format: yaml
  label: Paymob Subscription Plans API
  slug: paymob-subscription-plans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paymob/refs/heads/main/openapi/paymob-subscription-plans-api-openapi.yml
- filename: paymob-topup-api-openapi.yml
  format: yaml
  label: Paymob Topup API
  slug: paymob-topup-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paymob/refs/heads/main/openapi/paymob-topup-api-openapi.yml
- filename: paymob-transactions-api-openapi.yml
  format: yaml
  label: Paymob Transactions API
  slug: paymob-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paymob/refs/heads/main/openapi/paymob-transactions-api-openapi.yml
- filename: paymob-void-api-openapi.yml
  format: yaml
  label: Paymob Void API
  slug: paymob-void-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paymob/refs/heads/main/openapi/paymob-void-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Paymob Authentication
name_suffix: Authentication
oauth_flows: []
overview: Paymob secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Paymob
provider_slug: paymob
scheme_count: 2
schemes:
- description: Bearer auth_token from /api/auth/tokens (60-minute TTL).
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/paymob-accept-api-openapi.yml
  - openapi/paymob-card-tokens-api-openapi.yml
  - openapi/paymob-payouts-api-openapi.yml
  - openapi/paymob-subscriptions-api-openapi.yml
  type: http
- description: 'Provide the merchant Secret Key as `Authorization: Token <secret_key>` for backend calls.'
  in: header
  name: SecretKey
  parameter: Authorization
  sources:
  - openapi/paymob-intentions-api-openapi.yml
  type: apiKey
slug: paymob-authentication
source_filename: paymob-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/paymob-accept-api-openapi.yml, openapi/paymob-card-tokens-api-openapi.yml, openapi/paymob-intentions-api-openapi.yml,\n  openapi/paymob-payouts-api-openapi.yml, openapi/paymob-subscriptions-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: Bearer auth_token from /api/auth/tokens (60-minute TTL).\n  sources:\n  - openapi/paymob-accept-api-openapi.yml\n  - openapi/paymob-card-tokens-api-openapi.yml\n  - openapi/paymob-payouts-api-openapi.yml\n  - openapi/paymob-subscriptions-api-openapi.yml\n- name: SecretKey\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: 'Provide the merchant Secret Key as `Authorization: Token <secret_key>` for backend\n    calls.'\n  sources:\n  - openapi/paymob-intentions-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/paymob/refs/heads/main/authentication/paymob-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Payments
- Payment Gateway
- Fintech
- MENA
- MENAP
- Egypt
- Saudi Arabia
- UAE
- Pakistan
- Oman
- Card Payments
- Mobile Wallets
- BNPL
- Payouts
- Subscriptions
---
