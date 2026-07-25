---
api_key_in: []
api_specs:
- filename: paystack-webhooks-asyncapi.yml
  format: yaml
  label: Paystack Webhooks
  slug: paystack-webhooks
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/paystack/refs/heads/main/asyncapi/paystack-webhooks-asyncapi.yml
- filename: paystack-balance-api-openapi.yml
  format: yaml
  label: Paystack Balance API
  slug: paystack-balance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paystack/refs/heads/main/openapi/paystack-balance-api-openapi.yml
- filename: paystack-bulk-charge-api-openapi.yml
  format: yaml
  label: Paystack Bulk Charge API
  slug: paystack-bulk-charge-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paystack/refs/heads/main/openapi/paystack-bulk-charge-api-openapi.yml
- filename: paystack-charge-api-openapi.yml
  format: yaml
  label: Paystack Charge API
  slug: paystack-charge-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paystack/refs/heads/main/openapi/paystack-charge-api-openapi.yml
- filename: paystack-customer-api-openapi.yml
  format: yaml
  label: Paystack Customer API
  slug: paystack-customer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paystack/refs/heads/main/openapi/paystack-customer-api-openapi.yml
- filename: paystack-dedicated-virtual-account-api-openapi.yml
  format: yaml
  label: Paystack Dedicated Virtual Account API
  slug: paystack-dedicated-virtual-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paystack/refs/heads/main/openapi/paystack-dedicated-virtual-account-api-openapi.yml
- filename: paystack-dispute-api-openapi.yml
  format: yaml
  label: Paystack Dispute API
  slug: paystack-dispute-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paystack/refs/heads/main/openapi/paystack-dispute-api-openapi.yml
- filename: paystack-integration-api-openapi.yml
  format: yaml
  label: Paystack Integration API
  slug: paystack-integration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paystack/refs/heads/main/openapi/paystack-integration-api-openapi.yml
- filename: paystack-page-api-openapi.yml
  format: yaml
  label: Paystack Page API
  slug: paystack-page-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paystack/refs/heads/main/openapi/paystack-page-api-openapi.yml
- filename: paystack-payment-request-api-openapi.yml
  format: yaml
  label: Paystack Payment Request API
  slug: paystack-payment-request-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paystack/refs/heads/main/openapi/paystack-payment-request-api-openapi.yml
- filename: paystack-plan-api-openapi.yml
  format: yaml
  label: Paystack Plan API
  slug: paystack-plan-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paystack/refs/heads/main/openapi/paystack-plan-api-openapi.yml
- filename: paystack-product-api-openapi.yml
  format: yaml
  label: Paystack Product API
  slug: paystack-product-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paystack/refs/heads/main/openapi/paystack-product-api-openapi.yml
- filename: paystack-refund-api-openapi.yml
  format: yaml
  label: Paystack Refund API
  slug: paystack-refund-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paystack/refs/heads/main/openapi/paystack-refund-api-openapi.yml
- filename: paystack-settlement-api-openapi.yml
  format: yaml
  label: Paystack Settlement API
  slug: paystack-settlement-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paystack/refs/heads/main/openapi/paystack-settlement-api-openapi.yml
- filename: paystack-split-api-openapi.yml
  format: yaml
  label: Paystack Split API
  slug: paystack-split-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paystack/refs/heads/main/openapi/paystack-split-api-openapi.yml
- filename: paystack-subaccount-api-openapi.yml
  format: yaml
  label: Paystack Subaccount API
  slug: paystack-subaccount-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paystack/refs/heads/main/openapi/paystack-subaccount-api-openapi.yml
- filename: paystack-subscription-api-openapi.yml
  format: yaml
  label: Paystack Subscription API
  slug: paystack-subscription-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paystack/refs/heads/main/openapi/paystack-subscription-api-openapi.yml
- filename: paystack-transaction-api-openapi.yml
  format: yaml
  label: Paystack Transaction API
  slug: paystack-transaction-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paystack/refs/heads/main/openapi/paystack-transaction-api-openapi.yml
- filename: paystack-transfer-api-openapi.yml
  format: yaml
  label: Paystack Transfer API
  slug: paystack-transfer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paystack/refs/heads/main/openapi/paystack-transfer-api-openapi.yml
- filename: paystack-transfer-recipient-api-openapi.yml
  format: yaml
  label: Paystack Transfer Recipient API
  slug: paystack-transfer-recipient-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paystack/refs/heads/main/openapi/paystack-transfer-recipient-api-openapi.yml
- filename: paystack-verification-api-openapi.yml
  format: yaml
  label: Paystack Verification API
  slug: paystack-verification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paystack/refs/heads/main/openapi/paystack-verification-api-openapi.yml
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
