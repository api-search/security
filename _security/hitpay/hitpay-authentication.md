---
api_key_in: []
api_specs:
- filename: hitpay-openapi.yml
  format: yaml
  label: HitPay Payment Requests API
  slug: hitpay-payment-requests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hitpay/refs/heads/main/openapi/hitpay-openapi.yml
- filename: hitpay-openapi.yml
  format: yaml
  label: HitPay Recurring Billing API
  slug: hitpay-recurring-billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hitpay/refs/heads/main/openapi/hitpay-openapi.yml
- filename: hitpay-openapi.yml
  format: yaml
  label: HitPay Subscription Plans API
  slug: hitpay-subscription-plans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hitpay/refs/heads/main/openapi/hitpay-openapi.yml
- filename: hitpay-openapi.yml
  format: yaml
  label: HitPay Refunds API
  slug: hitpay-refunds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hitpay/refs/heads/main/openapi/hitpay-openapi.yml
- filename: hitpay-openapi.yml
  format: yaml
  label: HitPay Platform API
  slug: hitpay-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hitpay/refs/heads/main/openapi/hitpay-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Hitpay Authentication
name_suffix: Authentication
oauth_flows: []
overview: HitPay secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: HitPay
provider_slug: hitpay
scheme_count: 2
schemes:
- description: Per-merchant business API key from Dashboard > Settings > Payment Gateway > API Keys. Sent on every request. Sandbox uses a separate test key against https://api.sandbox.hit-pay.com/v1.
  headerName: X-BUSINESS-API-KEY
  in: header
  name: businessApiKey
  sources:
  - openapi/hitpay-openapi.yml
  - https://docs.hitpayapp.com/apis
  type: apiKey
- description: Additional key sent alongside X-BUSINESS-API-KEY by e-commerce platforms / aggregators using the Platform APIs to act on behalf of onboarded merchants.
  headerName: X-PLATFORM-KEY
  in: header
  name: platformKey
  sources:
  - https://docs.hitpayapp.com/apis/guide/platform-apis
  type: apiKey
slug: hitpay-authentication
source_filename: hitpay-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: derived\nsource: openapi/hitpay-openapi.yml\nsummary:\n  types:\n  - apiKey\nschemes:\n- name: businessApiKey\n  type: apiKey\n  in: header\n  headerName: X-BUSINESS-API-KEY\n  description: >-\n    Per-merchant business API key from Dashboard > Settings > Payment Gateway >\n    API Keys. Sent on every request. Sandbox uses a separate test key against\n    https://api.sandbox.hit-pay.com/v1.\n  sources:\n  - openapi/hitpay-openapi.yml\n  - https://docs.hitpayapp.com/apis\n- name: platformKey\n  type: apiKey\n  in: header\n  headerName: X-PLATFORM-KEY\n  description: >-\n    Additional key sent alongside X-BUSINESS-API-KEY by e-commerce platforms /\n    aggregators using the Platform APIs to act on behalf of onboarded merchants.\n  sources:\n  - https://docs.hitpayapp.com/apis/guide/platform-apis\nwebhookVerification:\n  header: Hitpay-Signature\n  algorithm: HMAC-SHA256\n  secret: merchant salt value (Dashboard > Payment Gateway > API)\n  note:\
  \ >-\n    Webhook authenticity is verified by computing HMAC-SHA256 of the JSON payload\n    using the salt value as the key and comparing against the Hitpay-Signature\n    header. This is inbound webhook verification, distinct from request auth.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hitpay/refs/heads/main/authentication/hitpay-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Payments
- Fintech
- PayNow
- Southeast Asia
- SMB
---
