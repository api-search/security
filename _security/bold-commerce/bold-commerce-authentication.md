---
api_key_in: []
api_specs:
- filename: bold-commerce-openapi.yml
  format: yaml
  label: Bold Subscriptions API
  slug: bold-commerce-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bold-commerce/refs/heads/main/openapi/bold-commerce-openapi.yml
- filename: bold-commerce-openapi.yml
  format: yaml
  label: Bold Checkout API
  slug: bold-commerce-checkout-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bold-commerce/refs/heads/main/openapi/bold-commerce-openapi.yml
- filename: bold-commerce-openapi.yml
  format: yaml
  label: Bold Price Rules API
  slug: bold-commerce-price-rules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bold-commerce/refs/heads/main/openapi/bold-commerce-openapi.yml
- filename: bold-commerce-openapi.yml
  format: yaml
  label: Bold Products API
  slug: bold-commerce-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bold-commerce/refs/heads/main/openapi/bold-commerce-openapi.yml
- filename: bold-commerce-openapi.yml
  format: yaml
  label: Bold Customers API
  slug: bold-commerce-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bold-commerce/refs/heads/main/openapi/bold-commerce-openapi.yml
- filename: bold-commerce-openapi.yml
  format: yaml
  label: Bold Shops API
  slug: bold-commerce-shops-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bold-commerce/refs/heads/main/openapi/bold-commerce-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
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
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bold-commerce/refs/heads/main/authentication/bold-commerce-authentication.yml
summary_line: http · 1 scheme
tags:
- E-Commerce
- Subscriptions
- Checkout
- Pricing
- Headless Commerce
- Shopify
---
