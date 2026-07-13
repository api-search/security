---
api_key_in: []
api_specs:
- filename: paypal-billing-subscriptions-openapi-original.yml
  format: yaml
  label: PayPal Billing Subscriptions API
  slug: paypal-billing-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paypal/refs/heads/main/openapi/paypal-billing-subscriptions-openapi-original.yml
- filename: paypal-catalog-products-openapi-original.yml
  format: yaml
  label: PayPal Catalog Products API
  slug: paypal-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paypal/refs/heads/main/openapi/paypal-catalog-products-openapi-original.yml
- filename: paypal-checkout-orders-openapi-original.yml
  format: yaml
  label: PayPal Orders API
  slug: paypal-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paypal/refs/heads/main/openapi/paypal-checkout-orders-openapi-original.yml
- filename: paypal-customer-disputes-openapi-original.yml
  format: yaml
  label: PayPal Customer Disputes API
  slug: paypal-disputes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paypal/refs/heads/main/openapi/paypal-customer-disputes-openapi-original.yml
- filename: paypal-customer-partner-referrals-openapi-original.yml
  format: yaml
  label: PayPal Partner Referrals API
  slug: paypal-partner-referrals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paypal/refs/heads/main/openapi/paypal-customer-partner-referrals-openapi-original.yml
- filename: paypal-invoicing-openapi-original.yml
  format: yaml
  label: PayPal Invoicing API
  slug: paypal-invoicing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paypal/refs/heads/main/openapi/paypal-invoicing-openapi-original.yml
- filename: paypal-notification-webhooks-openapi-original.yml
  format: yaml
  label: PayPal Notification Webhooks API
  slug: paypal-notification-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paypal/refs/heads/main/openapi/paypal-notification-webhooks-openapi-original.yml
- filename: paypal-payment-experience-openapi-original.yml
  format: yaml
  label: PayPal Payment Experience API
  slug: paypal-payment-experience-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paypal/refs/heads/main/openapi/paypal-payment-experience-openapi-original.yml
- filename: paypal-payments-openapi-original.yml
  format: yaml
  label: PayPal Payments API
  slug: paypal-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paypal/refs/heads/main/openapi/paypal-payments-openapi-original.yml
- filename: paypal-payouts-openapi-original.yml
  format: yaml
  label: PayPal Payouts API
  slug: paypal-payouts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paypal/refs/heads/main/openapi/paypal-payouts-openapi-original.yml
- filename: paypal-reporting-transactions-openapi-original.yml
  format: yaml
  label: PayPal Transaction Search (Reporting) API
  slug: paypal-reporting-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paypal/refs/heads/main/openapi/paypal-reporting-transactions-openapi-original.yml
- filename: paypal-shipping-tracking-openapi-original.yml
  format: yaml
  label: PayPal Shipping Tracking API
  slug: paypal-shipping-tracking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paypal/refs/heads/main/openapi/paypal-shipping-tracking-openapi-original.yml
- filename: paypal-vault-payment-tokens-openapi-original.yml
  format: yaml
  label: PayPal Vault Payment Tokens API
  slug: paypal-payment-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paypal/refs/heads/main/openapi/paypal-vault-payment-tokens-openapi-original.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Paypal Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: PayPal secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: PayPal
provider_slug: paypal
scheme_count: 1
schemes:
- description: Oauth 2.0 authentication
  flows:
  - flow: clientCredentials
    scopes: 1
    tokenUrl: /v1/oauth2/token
  name: Oauth2
  sources:
  - openapi/paypal-billing-subscriptions-openapi-original.yml
  - openapi/paypal-catalog-products-openapi-original.yml
  - openapi/paypal-checkout-orders-openapi-original.yml
  - openapi/paypal-customer-disputes-openapi-original.yml
  - openapi/paypal-customer-partner-referrals-openapi-original.yml
  - openapi/paypal-invoicing-openapi-original.yml
  - openapi/paypal-notification-webhooks-openapi-original.yml
  - openapi/paypal-payment-experience-openapi-original.yml
  - openapi/paypal-payments-openapi-original.yml
  - openapi/paypal-payouts-openapi-original.yml
  - openapi/paypal-reporting-transactions-openapi-original.yml
  - openapi/paypal-shipping-tracking-openapi-original.yml
  - openapi/paypal-vault-payment-tokens-openapi-original.yml
  type: oauth2
slug: paypal-authentication
source_filename: paypal-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/paypal-billing-subscriptions-openapi-original.yml, openapi/paypal-catalog-products-openapi-original.yml,\n  openapi/paypal-checkout-orders-openapi-original.yml, openapi/paypal-customer-disputes-openapi-original.yml,\n  openapi/paypal-customer-partner-referrals-openapi-original.yml, openapi/paypal-invoicing-openapi-original.yml,\n  openapi/paypal-notification-webhooks-openapi-original.yml, openapi/paypal-payment-experience-openapi-original.yml,\n  openapi/paypal-payments-openapi-original.yml, openapi/paypal-payouts-openapi-original.yml,\n  openapi/paypal-reporting-transactions-openapi-original.yml, openapi/paypal-shipping-tracking-openapi-original.yml\n  ...\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: Oauth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /v1/oauth2/token\n    scopes: 1\n  description: Oauth 2.0 authentication\n  sources:\n  - openapi/paypal-billing-subscriptions-openapi-original.yml\n\
  \  - openapi/paypal-catalog-products-openapi-original.yml\n  - openapi/paypal-checkout-orders-openapi-original.yml\n  - openapi/paypal-customer-disputes-openapi-original.yml\n  - openapi/paypal-customer-partner-referrals-openapi-original.yml\n  - openapi/paypal-invoicing-openapi-original.yml\n  - openapi/paypal-notification-webhooks-openapi-original.yml\n  - openapi/paypal-payment-experience-openapi-original.yml\n  - openapi/paypal-payments-openapi-original.yml\n  - openapi/paypal-payouts-openapi-original.yml\n  - openapi/paypal-reporting-transactions-openapi-original.yml\n  - openapi/paypal-shipping-tracking-openapi-original.yml\n  - openapi/paypal-vault-payment-tokens-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/paypal/refs/heads/main/authentication/paypal-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Billing
- Commerce
- Disputes
- Invoices
- Orders
- Payments
- Payouts
- Subscriptions
- Tokens
- Webhooks
---
