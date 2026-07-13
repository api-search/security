---
api_key_in: []
api_specs:
- filename: paystack-accept-payments-openapi.yml
  format: yaml
  label: Paystack Accept Payments API
  slug: paystack-accept-payments
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paystack/refs/heads/main/openapi/paystack-accept-payments-openapi.yml
- filename: paystack-subscriptions-openapi.yml
  format: yaml
  label: Paystack Subscriptions API
  slug: paystack-subscriptions
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paystack/refs/heads/main/openapi/paystack-subscriptions-openapi.yml
- filename: paystack-customers-openapi.yml
  format: yaml
  label: Paystack Customers API
  slug: paystack-customers
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paystack/refs/heads/main/openapi/paystack-customers-openapi.yml
- filename: paystack-transfers-openapi.yml
  format: yaml
  label: Paystack Transfers API
  slug: paystack-transfers
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paystack/refs/heads/main/openapi/paystack-transfers-openapi.yml
- filename: paystack-splits-subaccounts-openapi.yml
  format: yaml
  label: Paystack Splits and Subaccounts API
  slug: paystack-splits-subaccounts
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paystack/refs/heads/main/openapi/paystack-splits-subaccounts-openapi.yml
- filename: paystack-dedicated-virtual-accounts-openapi.yml
  format: yaml
  label: Paystack Dedicated Virtual Accounts API
  slug: paystack-dedicated-virtual-accounts
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paystack/refs/heads/main/openapi/paystack-dedicated-virtual-accounts-openapi.yml
- filename: paystack-products-pages-openapi.yml
  format: yaml
  label: Paystack Products and Payment Pages API
  slug: paystack-products-pages
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paystack/refs/heads/main/openapi/paystack-products-pages-openapi.yml
- filename: paystack-payment-requests-openapi.yml
  format: yaml
  label: Paystack Payment Requests API
  slug: paystack-payment-requests
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paystack/refs/heads/main/openapi/paystack-payment-requests-openapi.yml
- filename: paystack-refunds-disputes-openapi.yml
  format: yaml
  label: Paystack Refunds and Disputes API
  slug: paystack-refunds-disputes
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paystack/refs/heads/main/openapi/paystack-refunds-disputes-openapi.yml
- filename: paystack-settlements-openapi.yml
  format: yaml
  label: Paystack Settlements API
  slug: paystack-settlements
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paystack/refs/heads/main/openapi/paystack-settlements-openapi.yml
- filename: paystack-verification-openapi.yml
  format: yaml
  label: Paystack Verification API
  slug: paystack-verification
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paystack/refs/heads/main/openapi/paystack-verification-openapi.yml
- filename: paystack-balance-openapi.yml
  format: yaml
  label: Paystack Balance API
  slug: paystack-balance
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paystack/refs/heads/main/openapi/paystack-balance-openapi.yml
- filename: paystack-integration-openapi.yml
  format: yaml
  label: Paystack Integration Settings API
  slug: paystack-integration
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paystack/refs/heads/main/openapi/paystack-integration-openapi.yml
- filename: paystack-webhooks-asyncapi.yml
  format: yaml
  label: Paystack Webhooks
  slug: paystack-webhooks
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/paystack/refs/heads/main/asyncapi/paystack-webhooks-asyncapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Paystack Authentication
name_suffix: Authentication
oauth_flows: []
overview: Paystack secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Paystack
provider_slug: paystack
scheme_count: 1
schemes:
- name: bearerAuth
  scheme: bearer
  sources:
  - openapi/paystack-accept-payments-openapi.yml
  - openapi/paystack-balance-openapi.yml
  - openapi/paystack-customers-openapi.yml
  - openapi/paystack-dedicated-virtual-accounts-openapi.yml
  - openapi/paystack-integration-openapi.yml
  - openapi/paystack-openapi-original.yml
  - openapi/paystack-payment-requests-openapi.yml
  - openapi/paystack-products-pages-openapi.yml
  - openapi/paystack-refunds-disputes-openapi.yml
  - openapi/paystack-settlements-openapi.yml
  - openapi/paystack-splits-subaccounts-openapi.yml
  - openapi/paystack-subscriptions-openapi.yml
  - openapi/paystack-transfers-openapi.yml
  - openapi/paystack-verification-openapi.yml
  type: http
slug: paystack-authentication
source_filename: paystack-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/paystack-accept-payments-openapi.yml, openapi/paystack-balance-openapi.yml,\n  openapi/paystack-customers-openapi.yml, openapi/paystack-dedicated-virtual-accounts-openapi.yml,\n  openapi/paystack-integration-openapi.yml, openapi/paystack-openapi-original.yml, openapi/paystack-payment-requests-openapi.yml,\n  openapi/paystack-products-pages-openapi.yml, openapi/paystack-refunds-disputes-openapi.yml,\n  openapi/paystack-settlements-openapi.yml, openapi/paystack-splits-subaccounts-openapi.yml,\n  openapi/paystack-subscriptions-openapi.yml ...\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/paystack-accept-payments-openapi.yml\n  - openapi/paystack-balance-openapi.yml\n  - openapi/paystack-customers-openapi.yml\n  - openapi/paystack-dedicated-virtual-accounts-openapi.yml\n  - openapi/paystack-integration-openapi.yml\n  - openapi/paystack-openapi-original.yml\n\
  \  - openapi/paystack-payment-requests-openapi.yml\n  - openapi/paystack-products-pages-openapi.yml\n  - openapi/paystack-refunds-disputes-openapi.yml\n  - openapi/paystack-settlements-openapi.yml\n  - openapi/paystack-splits-subaccounts-openapi.yml\n  - openapi/paystack-subscriptions-openapi.yml\n  - openapi/paystack-transfers-openapi.yml\n  - openapi/paystack-verification-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/paystack/refs/heads/main/authentication/paystack-authentication.yml
summary_line: http · 1 scheme
tags:
- Payments
- Africa
- Fintech
- Recurring Billing
- Marketplaces
- Payouts
- Mobile Money
- Stripe
---
