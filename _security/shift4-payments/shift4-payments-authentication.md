---
api_key_in: []
api_specs:
- filename: shift4-payments-blacklist-api-openapi.yml
  format: yaml
  label: Shift4 Payments Blacklist API
  slug: shift4-payments-blacklist-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shift4-payments/refs/heads/main/openapi/shift4-payments-blacklist-api-openapi.yml
- filename: shift4-payments-cards-api-openapi.yml
  format: yaml
  label: Shift4 Payments Cards API
  slug: shift4-payments-cards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shift4-payments/refs/heads/main/openapi/shift4-payments-cards-api-openapi.yml
- filename: shift4-payments-charges-api-openapi.yml
  format: yaml
  label: Shift4 Payments Charges API
  slug: shift4-payments-charges-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shift4-payments/refs/heads/main/openapi/shift4-payments-charges-api-openapi.yml
- filename: shift4-payments-checkout-sessions-api-openapi.yml
  format: yaml
  label: Shift4 Payments Checkout Sessions API
  slug: shift4-payments-checkout-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shift4-payments/refs/heads/main/openapi/shift4-payments-checkout-sessions-api-openapi.yml
- filename: shift4-payments-credits-api-openapi.yml
  format: yaml
  label: Shift4 Payments Credits API
  slug: shift4-payments-credits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shift4-payments/refs/heads/main/openapi/shift4-payments-credits-api-openapi.yml
- filename: shift4-payments-customers-api-openapi.yml
  format: yaml
  label: Shift4 Payments Customers API
  slug: shift4-payments-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shift4-payments/refs/heads/main/openapi/shift4-payments-customers-api-openapi.yml
- filename: shift4-payments-disputes-api-openapi.yml
  format: yaml
  label: Shift4 Payments Disputes API
  slug: shift4-payments-disputes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shift4-payments/refs/heads/main/openapi/shift4-payments-disputes-api-openapi.yml
- filename: shift4-payments-events-api-openapi.yml
  format: yaml
  label: Shift4 Payments Events API
  slug: shift4-payments-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shift4-payments/refs/heads/main/openapi/shift4-payments-events-api-openapi.yml
- filename: shift4-payments-file-uploads-api-openapi.yml
  format: yaml
  label: Shift4 Payments File Uploads API
  slug: shift4-payments-file-uploads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shift4-payments/refs/heads/main/openapi/shift4-payments-file-uploads-api-openapi.yml
- filename: shift4-payments-fraud-warnings-api-openapi.yml
  format: yaml
  label: Shift4 Payments Fraud Warnings API
  slug: shift4-payments-fraud-warnings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shift4-payments/refs/heads/main/openapi/shift4-payments-fraud-warnings-api-openapi.yml
- filename: shift4-payments-payment-links-api-openapi.yml
  format: yaml
  label: Shift4 Payments Payment Links API
  slug: shift4-payments-payment-links-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shift4-payments/refs/heads/main/openapi/shift4-payments-payment-links-api-openapi.yml
- filename: shift4-payments-payment-methods-api-openapi.yml
  format: yaml
  label: Shift4 Payments Payment Methods API
  slug: shift4-payments-payment-methods-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shift4-payments/refs/heads/main/openapi/shift4-payments-payment-methods-api-openapi.yml
- filename: shift4-payments-payouts-api-openapi.yml
  format: yaml
  label: Shift4 Payments Payouts API
  slug: shift4-payments-payouts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shift4-payments/refs/heads/main/openapi/shift4-payments-payouts-api-openapi.yml
- filename: shift4-payments-plans-api-openapi.yml
  format: yaml
  label: Shift4 Payments Plans API
  slug: shift4-payments-plans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shift4-payments/refs/heads/main/openapi/shift4-payments-plans-api-openapi.yml
- filename: shift4-payments-refunds-api-openapi.yml
  format: yaml
  label: Shift4 Payments Refunds API
  slug: shift4-payments-refunds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shift4-payments/refs/heads/main/openapi/shift4-payments-refunds-api-openapi.yml
- filename: shift4-payments-subscriptions-api-openapi.yml
  format: yaml
  label: Shift4 Payments Subscriptions API
  slug: shift4-payments-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shift4-payments/refs/heads/main/openapi/shift4-payments-subscriptions-api-openapi.yml
- filename: shift4-payments-tokens-api-openapi.yml
  format: yaml
  label: Shift4 Payments Tokens API
  slug: shift4-payments-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shift4-payments/refs/heads/main/openapi/shift4-payments-tokens-api-openapi.yml
- filename: shift4-payments-webhook-endpoints-api-openapi.yml
  format: yaml
  label: Shift4 Payments Webhook Endpoints API
  slug: shift4-payments-webhook-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shift4-payments/refs/heads/main/openapi/shift4-payments-webhook-endpoints-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Shift4 Payments Authentication
name_suffix: Authentication
oauth_flows: []
overview: Shift4 Payments secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Shift4 Payments
provider_slug: shift4-payments
scheme_count: 1
schemes:
- description: Use your secret API key as the username with an empty password.
  name: BasicAuth
  scheme: basic
  sources:
  - openapi/shift4-api-openapi.yml
  type: http
slug: shift4-payments-authentication
source_filename: shift4-payments-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/shift4-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BasicAuth\n  type: http\n  scheme: basic\n  description: Use your secret API key as the username with an empty password.\n  sources:\n  - openapi/shift4-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/shift4-payments/refs/heads/main/authentication/shift4-payments-authentication.yml
summary_line: http · 1 scheme
tags:
- Payments
- Fintech
- Commerce
- Checkout
---
