---
api_key_in:
- header
api_specs:
- filename: payfast-subscriptions-api-openapi.yml
  format: yaml
  label: PayFast Subscriptions API
  slug: payfast-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payfast/refs/heads/main/openapi/payfast-subscriptions-api-openapi.yml
- filename: payfast-tokenization-api-openapi.yml
  format: yaml
  label: PayFast Tokenization API
  slug: payfast-tokenization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payfast/refs/heads/main/openapi/payfast-tokenization-api-openapi.yml
- filename: payfast-transaction-history-api-openapi.yml
  format: yaml
  label: PayFast Transaction History API
  slug: payfast-transaction-history-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payfast/refs/heads/main/openapi/payfast-transaction-history-api-openapi.yml
- filename: payfast-credit-card-transactions-api-openapi.yml
  format: yaml
  label: PayFast Credit Card Transactions API
  slug: payfast-credit-card-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payfast/refs/heads/main/openapi/payfast-credit-card-transactions-api-openapi.yml
- filename: payfast-refunds-api-openapi.yml
  format: yaml
  label: PayFast Refunds API
  slug: payfast-refunds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payfast/refs/heads/main/openapi/payfast-refunds-api-openapi.yml
- filename: payfast-credit-card-transactions-api-openapi.yml
  format: yaml
  label: PayFast Credit Card Transactions API
  slug: payfast-credit-card-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payfast/refs/heads/main/openapi/payfast-credit-card-transactions-api-openapi.yml
- filename: payfast-notifications-api-openapi.yml
  format: yaml
  label: PayFast Notifications API
  slug: payfast-notifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payfast/refs/heads/main/openapi/payfast-notifications-api-openapi.yml
- filename: payfast-onsite-checkout-api-openapi.yml
  format: yaml
  label: PayFast Onsite Checkout API
  slug: payfast-onsite-checkout-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payfast/refs/heads/main/openapi/payfast-onsite-checkout-api-openapi.yml
- filename: payfast-payment-form-api-openapi.yml
  format: yaml
  label: PayFast Payment Form API
  slug: payfast-payment-form-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payfast/refs/heads/main/openapi/payfast-payment-form-api-openapi.yml
- filename: payfast-refunds-api-openapi.yml
  format: yaml
  label: PayFast Refunds API
  slug: payfast-refunds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payfast/refs/heads/main/openapi/payfast-refunds-api-openapi.yml
- filename: payfast-subscriptions-api-openapi.yml
  format: yaml
  label: PayFast Subscriptions API
  slug: payfast-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payfast/refs/heads/main/openapi/payfast-subscriptions-api-openapi.yml
- filename: payfast-tokenization-api-openapi.yml
  format: yaml
  label: PayFast Tokenization API
  slug: payfast-tokenization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payfast/refs/heads/main/openapi/payfast-tokenization-api-openapi.yml
- filename: payfast-transaction-history-api-openapi.yml
  format: yaml
  label: PayFast Transaction History API
  slug: payfast-transaction-history-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payfast/refs/heads/main/openapi/payfast-transaction-history-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Payfast Authentication
name_suffix: Authentication
oauth_flows: []
overview: PayFast secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: PayFast
provider_slug: payfast
scheme_count: 1
schemes:
- description: PayFast API authentication uses an MD5 signature derived from the merchant ID, passphrase, timestamp, and request data. Required headers include merchant-id, version, timestamp, and signature.
  in: header
  name: merchantAuth
  parameter: merchant-id
  sources:
  - openapi/openapi.yml
  type: apiKey
slug: payfast-authentication
source_filename: payfast-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: merchantAuth\n  type: apiKey\n  in: header\n  parameter: merchant-id\n  description: PayFast API authentication uses an MD5 signature derived from the merchant ID,\n    passphrase, timestamp, and request data. Required headers include merchant-id, version,\n    timestamp, and signature.\n  sources:\n  - openapi/openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/payfast/refs/heads/main/authentication/payfast-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Payments
- Payment Gateway
- South Africa
- Subscriptions
- Recurring Billing
- Tokenization
- Instant EFT
- QR Code Payments
- Refunds
- Fintech
---
