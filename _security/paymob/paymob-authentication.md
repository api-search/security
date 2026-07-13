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
- filename: paymob-accept-api-openapi.yml
  format: yaml
  label: Paymob Accept API
  slug: paymob-accept-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paymob/refs/heads/main/openapi/paymob-accept-api-openapi.yml
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
- filename: paymob-payouts-api-openapi.yml
  format: yaml
  label: Paymob Payouts (Send) API
  slug: paymob-payouts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paymob/refs/heads/main/openapi/paymob-payouts-api-openapi.yml
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
