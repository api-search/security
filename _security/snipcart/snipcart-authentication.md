---
api_key_in: []
api_specs:
- filename: snipcart-abandonedcarts-api-openapi.yml
  format: yaml
  label: Snipcart AbandonedCarts API
  slug: snipcart-abandonedcarts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snipcart/refs/heads/main/openapi/snipcart-abandonedcarts-api-openapi.yml
- filename: snipcart-customers-api-openapi.yml
  format: yaml
  label: Snipcart Customers API
  slug: snipcart-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snipcart/refs/heads/main/openapi/snipcart-customers-api-openapi.yml
- filename: snipcart-discounts-api-openapi.yml
  format: yaml
  label: Snipcart Discounts API
  slug: snipcart-discounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snipcart/refs/heads/main/openapi/snipcart-discounts-api-openapi.yml
- filename: snipcart-domains-api-openapi.yml
  format: yaml
  label: Snipcart Domains API
  slug: snipcart-domains-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snipcart/refs/heads/main/openapi/snipcart-domains-api-openapi.yml
- filename: snipcart-notifications-api-openapi.yml
  format: yaml
  label: Snipcart Notifications API
  slug: snipcart-notifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snipcart/refs/heads/main/openapi/snipcart-notifications-api-openapi.yml
- filename: snipcart-orders-api-openapi.yml
  format: yaml
  label: Snipcart Orders API
  slug: snipcart-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snipcart/refs/heads/main/openapi/snipcart-orders-api-openapi.yml
- filename: snipcart-products-api-openapi.yml
  format: yaml
  label: Snipcart Products API
  slug: snipcart-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snipcart/refs/heads/main/openapi/snipcart-products-api-openapi.yml
- filename: snipcart-refunds-api-openapi.yml
  format: yaml
  label: Snipcart Refunds API
  slug: snipcart-refunds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snipcart/refs/heads/main/openapi/snipcart-refunds-api-openapi.yml
- filename: snipcart-usersessions-api-openapi.yml
  format: yaml
  label: Snipcart UserSessions API
  slug: snipcart-usersessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snipcart/refs/heads/main/openapi/snipcart-usersessions-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Snipcart Authentication
name_suffix: Authentication
oauth_flows: []
overview: Snipcart secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Snipcart
provider_slug: snipcart
scheme_count: 1
schemes:
- description: 'Use your secret API key as the username with an empty password. Base64-encode as {API_KEY}: and pass as Authorization: Basic {encoded}.'
  name: basicAuth
  scheme: basic
  sources:
  - openapi/snipcart-rest-api-openapi.yml
  type: http
slug: snipcart-authentication
source_filename: snipcart-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/snipcart-rest-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: 'Use your secret API key as the username with an empty password. Base64-encode\n    as {API_KEY}: and pass as Authorization: Basic {encoded}.'\n  sources:\n  - openapi/snipcart-rest-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/snipcart/refs/heads/main/authentication/snipcart-authentication.yml
summary_line: http · 1 scheme
tags:
- E-Commerce
- Shopping Cart
- Order
- Product
- Payments
- Webhook
- Headless Commerce
- Jamstack
---
