---
api_key_in: []
api_specs:
- filename: pagseguro-accounts-api-openapi.yml
  format: yaml
  label: PagSeguro / PagBank Accounts API
  slug: pagseguro-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pagseguro/refs/heads/main/openapi/pagseguro-accounts-api-openapi.yml
- filename: pagseguro-charges-api-openapi.yml
  format: yaml
  label: PagSeguro / PagBank Charges API
  slug: pagseguro-charges-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pagseguro/refs/heads/main/openapi/pagseguro-charges-api-openapi.yml
- filename: pagseguro-checkout-api-openapi.yml
  format: yaml
  label: PagSeguro / PagBank Checkout API
  slug: pagseguro-checkout-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pagseguro/refs/heads/main/openapi/pagseguro-checkout-api-openapi.yml
- filename: pagseguro-connect-api-openapi.yml
  format: yaml
  label: PagSeguro / PagBank Connect API
  slug: pagseguro-connect-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pagseguro/refs/heads/main/openapi/pagseguro-connect-api-openapi.yml
- filename: pagseguro-coupons-api-openapi.yml
  format: yaml
  label: PagSeguro / PagBank Coupons API
  slug: pagseguro-coupons-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pagseguro/refs/heads/main/openapi/pagseguro-coupons-api-openapi.yml
- filename: pagseguro-invoices-api-openapi.yml
  format: yaml
  label: PagSeguro / PagBank Invoices API
  slug: pagseguro-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pagseguro/refs/heads/main/openapi/pagseguro-invoices-api-openapi.yml
- filename: pagseguro-orders-api-openapi.yml
  format: yaml
  label: PagSeguro / PagBank Orders API
  slug: pagseguro-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pagseguro/refs/heads/main/openapi/pagseguro-orders-api-openapi.yml
- filename: pagseguro-plans-api-openapi.yml
  format: yaml
  label: PagSeguro / PagBank Plans API
  slug: pagseguro-plans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pagseguro/refs/heads/main/openapi/pagseguro-plans-api-openapi.yml
- filename: pagseguro-publickeys-api-openapi.yml
  format: yaml
  label: PagSeguro / PagBank PublicKeys API
  slug: pagseguro-publickeys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pagseguro/refs/heads/main/openapi/pagseguro-publickeys-api-openapi.yml
- filename: pagseguro-refunds-api-openapi.yml
  format: yaml
  label: PagSeguro / PagBank Refunds API
  slug: pagseguro-refunds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pagseguro/refs/heads/main/openapi/pagseguro-refunds-api-openapi.yml
- filename: pagseguro-subscribers-api-openapi.yml
  format: yaml
  label: PagSeguro / PagBank Subscribers API
  slug: pagseguro-subscribers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pagseguro/refs/heads/main/openapi/pagseguro-subscribers-api-openapi.yml
- filename: pagseguro-subscriptions-api-openapi.yml
  format: yaml
  label: PagSeguro / PagBank Subscriptions API
  slug: pagseguro-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pagseguro/refs/heads/main/openapi/pagseguro-subscriptions-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Pagseguro Authentication
name_suffix: Authentication
oauth_flows: []
overview: PagSeguro / PagBank secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: PagSeguro / PagBank
provider_slug: pagseguro
scheme_count: 1
schemes:
- bearerFormat: access_token
  description: 'PagBank access token issued via the developer portal (or via the

    Connect flow). Send as "Authorization: Bearer {ACCESS_TOKEN}". All

    requests must be HTTPS.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/pagseguro-openapi.yml
  type: http
slug: pagseguro-authentication
source_filename: pagseguro-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/pagseguro-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: access_token\n  description: |-\n    PagBank access token issued via the developer portal (or via the\n    Connect flow). Send as \"Authorization: Bearer {ACCESS_TOKEN}\". All\n    requests must be HTTPS.\n  sources:\n  - openapi/pagseguro-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pagseguro/refs/heads/main/authentication/pagseguro-authentication.yml
summary_line: http · 1 scheme
tags:
- Payments
- Checkout
- Pix
- Boleto
- Cards
- Subscriptions
- Recurring
- POS
- Card Reader
- Marketplace
- Split
- Payouts
- Digital Bank
- Brazil
- Latin America
- Fintech
---
