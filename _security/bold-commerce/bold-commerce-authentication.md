---
anonymous_access: false
api_key_in: []
api_specs:
- filename: bold-commerce-customers-api-openapi.yml
  format: yaml
  label: Bold Commerce Customers API
  slug: bold-commerce-customers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bold-commerce/openapi/bold-commerce-customers-api-openapi.yml
- filename: bold-commerce-shops-api-openapi.yml
  format: yaml
  label: Bold Commerce Shops API
  slug: bold-commerce-shops-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bold-commerce/openapi/bold-commerce-shops-api-openapi.yml
- filename: bold-commerce-subscriptions-api-openapi.yml
  format: yaml
  label: Bold Commerce Subscriptions API
  slug: bold-commerce-subscriptions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bold-commerce/openapi/bold-commerce-subscriptions-api-openapi.yml
- filename: bold-commerce-convertible-adjustments-api-openapi.yml
  format: yaml
  label: Bold Commerce Convertible Adjustments API
  slug: bold-commerce-convertible-adjustments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bold-commerce/openapi/bold-commerce-convertible-adjustments-api-openapi.yml
- filename: bold-commerce-future-orders-api-openapi.yml
  format: yaml
  label: Bold Commerce Future Orders API
  slug: bold-commerce-future-orders-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bold-commerce/openapi/bold-commerce-future-orders-api-openapi.yml
- filename: bold-commerce-payment-methods-api-openapi.yml
  format: yaml
  label: Bold Commerce Payment Methods API
  slug: bold-commerce-payment-methods-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bold-commerce/openapi/bold-commerce-payment-methods-api-openapi.yml
- filename: bold-commerce-subscription-adjustments-api-openapi.yml
  format: yaml
  label: Bold Commerce Subscription Adjustments API
  slug: bold-commerce-subscription-adjustments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bold-commerce/openapi/bold-commerce-subscription-adjustments-api-openapi.yml
- filename: bold-commerce-subscription-groups-api-openapi.yml
  format: yaml
  label: Bold Commerce Subscription Groups API
  slug: bold-commerce-subscription-groups-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bold-commerce/openapi/bold-commerce-subscription-groups-api-openapi.yml
- filename: bold-commerce-subscription-line-items-api-openapi.yml
  format: yaml
  label: Bold Commerce Subscription Line Items API
  slug: bold-commerce-subscription-line-items-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bold-commerce/openapi/bold-commerce-subscription-line-items-api-openapi.yml
- filename: bold-commerce-subscription-orders-api-openapi.yml
  format: yaml
  label: Bold Commerce Subscription Orders API
  slug: bold-commerce-subscription-orders-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bold-commerce/openapi/bold-commerce-subscription-orders-api-openapi.yml
- filename: bold-commerce-webhook-events-api-openapi.yml
  format: yaml
  label: Bold Commerce Webhook Events API
  slug: bold-commerce-webhook-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bold-commerce/openapi/bold-commerce-webhook-events-api-openapi.yml
- filename: bold-commerce-webhook-subscriptions-api-openapi.yml
  format: yaml
  label: Bold Commerce Webhook Subscriptions API
  slug: bold-commerce-webhook-subscriptions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bold-commerce/openapi/bold-commerce-webhook-subscriptions-api-openapi.yml
- filename: bold-commerce-webhook-topics-api-openapi.yml
  format: yaml
  label: Bold Commerce Webhook Topics API
  slug: bold-commerce-webhook-topics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bold-commerce/openapi/bold-commerce-webhook-topics-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Bold Commerce Authentication
name_suffix: Authentication
oauth_flows: []
overview: Bold Commerce secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Bold Commerce
provider_slug: bold-commerce
scheme_count: 1
schemes:
- description: 'OAuth 2.0 access token (public integrations) or scoped API access token (private integrations), passed as Authorization: Bearer {token}.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/bold-commerce-openapi.yml
  type: http
slug: bold-commerce-authentication
source_filename: bold-commerce-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/bold-commerce-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'OAuth 2.0 access token (public integrations) or scoped API access token (private\n    integrations), passed as Authorization: Bearer {token}.'\n  sources:\n  - openapi/bold-commerce-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/bold-commerce/authentication/bold-commerce-authentication.yml
summary_line: http · 1 scheme
tags:
- E-Commerce
- Subscription
- Checkout
- Pricing
- Headless Commerce
- Shopify
---
