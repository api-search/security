---
anonymous_access: false
api_key_in: []
api_specs:
- filename: checkoutpage-com-account-api-openapi.yml
  format: yaml
  label: Checkout Page Account API
  slug: checkoutpage-com-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/checkoutpage-com/openapi/checkoutpage-com-account-api-openapi.yml
- filename: checkoutpage-com-checkout-pages-api-openapi.yml
  format: yaml
  label: Checkout Page Checkout Pages API
  slug: checkoutpage-com-checkout-pages-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/checkoutpage-com/openapi/checkoutpage-com-checkout-pages-api-openapi.yml
- filename: checkoutpage-com-coupons-api-openapi.yml
  format: yaml
  label: Checkout Page Coupons API
  slug: checkoutpage-com-coupons-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/checkoutpage-com/openapi/checkoutpage-com-coupons-api-openapi.yml
- filename: checkoutpage-com-customers-api-openapi.yml
  format: yaml
  label: Checkout Page Customers API
  slug: checkoutpage-com-customers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/checkoutpage-com/openapi/checkoutpage-com-customers-api-openapi.yml
- filename: checkoutpage-com-events-api-openapi.yml
  format: yaml
  label: Checkout Page Events API
  slug: checkoutpage-com-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/checkoutpage-com/openapi/checkoutpage-com-events-api-openapi.yml
- filename: checkoutpage-com-files-api-openapi.yml
  format: yaml
  label: Checkout Page Files API
  slug: checkoutpage-com-files-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/checkoutpage-com/openapi/checkoutpage-com-files-api-openapi.yml
- filename: checkoutpage-com-forms-api-openapi.yml
  format: yaml
  label: Checkout Page Forms API
  slug: checkoutpage-com-forms-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/checkoutpage-com/openapi/checkoutpage-com-forms-api-openapi.yml
- filename: checkoutpage-com-invoices-api-openapi.yml
  format: yaml
  label: Checkout Page Invoices API
  slug: checkoutpage-com-invoices-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/checkoutpage-com/openapi/checkoutpage-com-invoices-api-openapi.yml
- filename: checkoutpage-com-payments-api-openapi.yml
  format: yaml
  label: Checkout Page Payments API
  slug: checkoutpage-com-payments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/checkoutpage-com/openapi/checkoutpage-com-payments-api-openapi.yml
- filename: checkoutpage-com-products-api-openapi.yml
  format: yaml
  label: Checkout Page Products API
  slug: checkoutpage-com-products-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/checkoutpage-com/openapi/checkoutpage-com-products-api-openapi.yml
- filename: checkoutpage-com-subscription-payments-api-openapi.yml
  format: yaml
  label: Checkout Page Subscription Payments API
  slug: checkoutpage-com-subscription-payments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/checkoutpage-com/openapi/checkoutpage-com-subscription-payments-api-openapi.yml
- filename: checkoutpage-com-subscriptions-api-openapi.yml
  format: yaml
  label: Checkout Page Subscriptions API
  slug: checkoutpage-com-subscriptions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/checkoutpage-com/openapi/checkoutpage-com-subscriptions-api-openapi.yml
- filename: checkoutpage-com-tax-rates-api-openapi.yml
  format: yaml
  label: Checkout Page Tax Rates API
  slug: checkoutpage-com-tax-rates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/checkoutpage-com/openapi/checkoutpage-com-tax-rates-api-openapi.yml
- filename: checkoutpage-com-themes-api-openapi.yml
  format: yaml
  label: Checkout Page Themes API
  slug: checkoutpage-com-themes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/checkoutpage-com/openapi/checkoutpage-com-themes-api-openapi.yml
- filename: checkoutpage-com-webhooks-api-openapi.yml
  format: yaml
  label: Checkout Page Webhooks API
  slug: checkoutpage-com-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/checkoutpage-com/openapi/checkoutpage-com-webhooks-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Checkout Page Authentication
name_suffix: Authentication
oauth_flows: []
overview: Checkout Page secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Checkout Page
provider_slug: checkoutpage-com
scheme_count: 1
schemes:
- bearerFormat: API Key
  description: API key authentication. Use "Bearer YOUR_API_KEY" format.
  failure:
    body:
      error: Unauthorized
      message: Missing or invalid API key
    status: 401
  header: 'Authorization: Bearer YOUR_API_KEY'
  issuance: Settings > API Keys in the seller dashboard; key is shown once
  key_prefixes:
  - sk_live_
  - sk_test_
  name: api_key_auth
  scheme: bearer
  sources:
  - openapi/checkoutpage-com-openapi.yml
  type: http
slug: checkoutpage-com-authentication
source_filename: checkoutpage-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: searched\nsource:\n- openapi/checkoutpage-com-openapi.yml\n- https://checkoutpage.com/docs/api/authentication\nsummary:\n  types:\n  - http\nschemes:\n- name: api_key_auth\n  type: http\n  scheme: bearer\n  bearerFormat: API Key\n  description: API key authentication. Use \"Bearer YOUR_API_KEY\" format.\n  sources:\n  - openapi/checkoutpage-com-openapi.yml\n  header: 'Authorization: Bearer YOUR_API_KEY'\n  key_prefixes:\n  - sk_live_\n  - sk_test_\n  issuance: Settings > API Keys in the seller dashboard; key is shown once\n  failure:\n    status: 401\n    body:\n      error: Unauthorized\n      message: Missing or invalid API key\ndocs: https://checkoutpage.com/docs/api/authentication\noauth: false\n"
source_yaml_url: https://artifacts.apis.io/checkoutpage-com/authentication/checkoutpage-com-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Payments
- Checkout
- Stripe
- No-Code
- E-Commerce
- Subscription
- Event Ticketing
---
