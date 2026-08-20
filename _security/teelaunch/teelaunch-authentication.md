---
api_key_in: []
api_specs:
- filename: teelaunch-account-api-openapi.yml
  format: yaml
  label: Teelaunch Account API
  slug: teelaunch-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teelaunch/refs/heads/main/openapi/teelaunch-account-api-openapi.yml
- filename: teelaunch-account-payment-api-openapi.yml
  format: yaml
  label: Teelaunch Account Payment API
  slug: teelaunch-account-payment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teelaunch/refs/heads/main/openapi/teelaunch-account-payment-api-openapi.yml
- filename: teelaunch-account-settings-api-openapi.yml
  format: yaml
  label: Teelaunch Account Settings API
  slug: teelaunch-account-settings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teelaunch/refs/heads/main/openapi/teelaunch-account-settings-api-openapi.yml
- filename: teelaunch-blank-api-openapi.yml
  format: yaml
  label: Teelaunch Blank API
  slug: teelaunch-blank-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teelaunch/refs/heads/main/openapi/teelaunch-blank-api-openapi.yml
- filename: teelaunch-blank-category-api-openapi.yml
  format: yaml
  label: Teelaunch Blank Category API
  slug: teelaunch-blank-category-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teelaunch/refs/heads/main/openapi/teelaunch-blank-category-api-openapi.yml
- filename: teelaunch-orders-api-openapi.yml
  format: yaml
  label: Teelaunch Orders API
  slug: teelaunch-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teelaunch/refs/heads/main/openapi/teelaunch-orders-api-openapi.yml
- filename: teelaunch-platform-store-product-variants-api-openapi.yml
  format: yaml
  label: Teelaunch Platform Store Product Variants API
  slug: teelaunch-platform-store-product-variants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teelaunch/refs/heads/main/openapi/teelaunch-platform-store-product-variants-api-openapi.yml
- filename: teelaunch-platform-store-products-api-openapi.yml
  format: yaml
  label: Teelaunch Platform Store Products API
  slug: teelaunch-platform-store-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teelaunch/refs/heads/main/openapi/teelaunch-platform-store-products-api-openapi.yml
- filename: teelaunch-platform-stores-api-openapi.yml
  format: yaml
  label: Teelaunch Platform Stores API
  slug: teelaunch-platform-stores-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teelaunch/refs/heads/main/openapi/teelaunch-platform-stores-api-openapi.yml
- filename: teelaunch-platforms-api-openapi.yml
  format: yaml
  label: Teelaunch Platforms API
  slug: teelaunch-platforms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teelaunch/refs/heads/main/openapi/teelaunch-platforms-api-openapi.yml
- filename: teelaunch-products-api-openapi.yml
  format: yaml
  label: Teelaunch Products API
  slug: teelaunch-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teelaunch/refs/heads/main/openapi/teelaunch-products-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Teelaunch Authentication
name_suffix: Authentication
oauth_flows: []
overview: Teelaunch secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Teelaunch
provider_slug: teelaunch
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/teelaunch-openapi.yml
  type: http
slug: teelaunch-authentication
source_filename: teelaunch-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/teelaunch-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/teelaunch-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/teelaunch/refs/heads/main/authentication/teelaunch-authentication.yml
summary_line: http · 1 scheme
tags:
- Print on Demand
- POD
- E-Commerce
- Fulfillment
- Dropshipping
- Order
- Shipping
---
