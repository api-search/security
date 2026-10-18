---
anonymous_access: false
api_key_in: []
api_specs:
- filename: pagar-me-contestations-api-openapi.yml
  format: yaml
  label: Pagar.me Contestations API
  slug: pagar-me-contestations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pagar-me/refs/heads/main/openapi/pagar-me-contestations-api-openapi.yml
- filename: pagar-me-customers-api-openapi.yml
  format: yaml
  label: Pagar.me Customers API
  slug: pagar-me-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pagar-me/refs/heads/main/openapi/pagar-me-customers-api-openapi.yml
- filename: pagar-me-disputas-api-openapi.yml
  format: yaml
  label: Pagar.me Disputas API
  slug: pagar-me-disputas-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pagar-me/refs/heads/main/openapi/pagar-me-disputas-api-openapi.yml
- filename: pagar-me-hooks-api-openapi.yml
  format: yaml
  label: Pagar.me Hooks API
  slug: pagar-me-hooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pagar-me/refs/heads/main/openapi/pagar-me-hooks-api-openapi.yml
- filename: pagar-me-invoices-api-openapi.yml
  format: yaml
  label: Pagar.me Invoices API
  slug: pagar-me-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pagar-me/refs/heads/main/openapi/pagar-me-invoices-api-openapi.yml
- filename: pagar-me-orders-api-openapi.yml
  format: yaml
  label: Pagar.me Orders API
  slug: pagar-me-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pagar-me/refs/heads/main/openapi/pagar-me-orders-api-openapi.yml
- filename: pagar-me-paymentlinks-api-openapi.yml
  format: yaml
  label: Pagar.me Paymentlinks API
  slug: pagar-me-paymentlinks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pagar-me/refs/heads/main/openapi/pagar-me-paymentlinks-api-openapi.yml
- filename: pagar-me-plans-api-openapi.yml
  format: yaml
  label: Pagar.me Plans API
  slug: pagar-me-plans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pagar-me/refs/heads/main/openapi/pagar-me-plans-api-openapi.yml
- filename: pagar-me-recipients-api-openapi.yml
  format: yaml
  label: Pagar.me Recipients API
  slug: pagar-me-recipients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pagar-me/refs/heads/main/openapi/pagar-me-recipients-api-openapi.yml
- filename: pagar-me-settlement-obligations-api-openapi.yml
  format: yaml
  label: Pagar.me Settlement Obligations API
  slug: pagar-me-settlement-obligations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pagar-me/refs/heads/main/openapi/pagar-me-settlement-obligations-api-openapi.yml
- filename: pagar-me-settlements-api-openapi.yml
  format: yaml
  label: Pagar.me Settlements API
  slug: pagar-me-settlements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pagar-me/refs/heads/main/openapi/pagar-me-settlements-api-openapi.yml
- filename: pagar-me-subscriptions-api-openapi.yml
  format: yaml
  label: Pagar.me Subscriptions API
  slug: pagar-me-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pagar-me/refs/heads/main/openapi/pagar-me-subscriptions-api-openapi.yml
- filename: pagar-me-tokens-api-openapi.yml
  format: yaml
  label: Pagar.me Tokens API
  slug: pagar-me-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pagar-me/refs/heads/main/openapi/pagar-me-tokens-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Pagar Me Authentication
name_suffix: Authentication
oauth_flows: []
overview: Pagar.me secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Pagar.me
provider_slug: pagar-me
scheme_count: 1
schemes:
- name: sec0
  scheme: basic
  sources:
  - openapi/pagar-me-pagarme-api-openapi.yml
  - openapi/pagar-me-pagarme-api-register-v5-openapi.yml
  type: http
slug: pagar-me-authentication
source_filename: pagar-me-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: derived\nsource: openapi/pagar-me-pagarme-api-openapi.yml, openapi/pagar-me-pagarme-api-register-v5-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: sec0\n  type: http\n  scheme: basic\n  sources:\n  - openapi/pagar-me-pagarme-api-openapi.yml\n  - openapi/pagar-me-pagarme-api-register-v5-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pagar-me/refs/heads/main/authentication/pagar-me-authentication.yml
summary_line: http · 1 scheme
tags:
- Payments
- Financial Services
- Fintech
- Brazil
- Latin America
- Stone Co
- Pix
- Boleto
- Credit Cards
- Marketplace
- Split Payments
- Subscription
- Recurring Billing
- Fraud Prevention
- 3D
- Checkout
- Payment Links
- Webhook
- E-Commerce
- Anticipation
---
