---
api_key_in: []
api_specs:
- filename: paymongo-openapi.yml
  format: yaml
  label: PayMongo Payment Intents API
  slug: paymongo-payment-intents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paymongo/refs/heads/main/openapi/paymongo-openapi.yml
- filename: paymongo-openapi.yml
  format: yaml
  label: PayMongo Payment Methods API
  slug: paymongo-payment-methods-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paymongo/refs/heads/main/openapi/paymongo-openapi.yml
- filename: paymongo-openapi.yml
  format: yaml
  label: PayMongo Payments API
  slug: paymongo-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paymongo/refs/heads/main/openapi/paymongo-openapi.yml
- filename: paymongo-openapi.yml
  format: yaml
  label: PayMongo Sources API
  slug: paymongo-sources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paymongo/refs/heads/main/openapi/paymongo-openapi.yml
- filename: paymongo-openapi.yml
  format: yaml
  label: PayMongo Checkout Sessions API
  slug: paymongo-checkout-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paymongo/refs/heads/main/openapi/paymongo-openapi.yml
- filename: paymongo-openapi.yml
  format: yaml
  label: PayMongo Payment Links API
  slug: paymongo-payment-links-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paymongo/refs/heads/main/openapi/paymongo-openapi.yml
- filename: paymongo-openapi.yml
  format: yaml
  label: PayMongo Customers API
  slug: paymongo-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paymongo/refs/heads/main/openapi/paymongo-openapi.yml
- filename: paymongo-openapi.yml
  format: yaml
  label: PayMongo Refunds API
  slug: paymongo-refunds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paymongo/refs/heads/main/openapi/paymongo-openapi.yml
- filename: paymongo-openapi.yml
  format: yaml
  label: PayMongo QR Ph API
  slug: paymongo-qr-ph-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paymongo/refs/heads/main/openapi/paymongo-openapi.yml
- filename: paymongo-openapi.yml
  format: yaml
  label: PayMongo Webhooks API
  slug: paymongo-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paymongo/refs/heads/main/openapi/paymongo-openapi.yml
- filename: paymongo-openapi.yml
  format: yaml
  label: PayMongo Subscriptions & Plans API
  slug: paymongo-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paymongo/refs/heads/main/openapi/paymongo-openapi.yml
- filename: paymongo-openapi.yml
  format: yaml
  label: PayMongo Money Movement API
  slug: paymongo-money-movement-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paymongo/refs/heads/main/openapi/paymongo-openapi.yml
- filename: paymongo-openapi.yml
  format: yaml
  label: PayMongo Forex API
  slug: paymongo-forex-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paymongo/refs/heads/main/openapi/paymongo-openapi.yml
- filename: paymongo-openapi.yml
  format: yaml
  label: PayMongo Fraud Detection API
  slug: paymongo-fraud-detection-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paymongo/refs/heads/main/openapi/paymongo-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Paymongo Authentication
name_suffix: Authentication
oauth_flows: []
overview: PayMongo secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: PayMongo
provider_slug: paymongo
scheme_count: 1
schemes:
- name: basic_auth
  scheme: basic
  sources:
  - openapi/paymongo-openapi.yml
  - https://docs.paymongo.com/reference/authentication-1
  type: http
slug: paymongo-authentication
source_filename: paymongo-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: derived\nsource: openapi/paymongo-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basic_auth\n  type: http\n  scheme: basic\n  sources:\n  - openapi/paymongo-openapi.yml\n  - https://docs.paymongo.com/reference/authentication-1\nnotes: >-\n  PayMongo uses HTTP Basic authentication. The API key is supplied as the\n  Basic-auth username (base64-encoded per the Basic scheme); the password\n  field is left blank for single-key calls. Secret keys (sk_test_* / sk_live_*)\n  are used for server-side calls; the public key (pk_test_* / pk_live_*) may be\n  used client-side for Payment Method creation. Some newer Workflow / Ledgers\n  surfaces additionally require an Organization-Id header. Webhook payloads are\n  verified separately via the Paymongo-Signature header (HMAC with the webhook\n  signing secret), which is a payload-integrity mechanism rather than a request\n  auth scheme. Live probe: GET https://api.paymongo.com/v1/payment_intents\n\
  \  returned HTTP 401 without credentials, confirming Basic auth is enforced.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/paymongo/refs/heads/main/authentication/paymongo-authentication.yml
summary_line: http · 1 scheme
tags:
- Payments
- FinTech
- Philippines
- Southeast Asia
- GCash
- E-Wallet
- Card Payments
---
