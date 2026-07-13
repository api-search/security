---
api_key_in:
- header
api_specs:
- filename: spree-store-api.yaml
  format: yaml
  label: Spree Store API
  slug: spree-store-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spree/refs/heads/main/openapi/spree-store-api.yaml
- filename: spree-admin-api.yaml
  format: yaml
  label: Spree Admin API
  slug: spree-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spree/refs/heads/main/openapi/spree-admin-api.yaml
- filename: spree-storefront-api.yaml
  format: yaml
  label: Spree Storefront API
  slug: spree-storefront-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spree/refs/heads/main/openapi/spree-storefront-api.yaml
- filename: spree-platform-api.yaml
  format: yaml
  label: Spree Platform API
  slug: spree-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spree/refs/heads/main/openapi/spree-platform-api.yaml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Spree Authentication
name_suffix: Authentication
oauth_flows: []
overview: Spree Commerce secures its APIs with apiKey and http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Spree Commerce
provider_slug: spree
scheme_count: 3
schemes:
- description: Secret API key for admin access
  in: header
  name: api_key
  parameter: x-spree-api-key
  sources:
  - openapi/spree-admin-api.yaml
  - openapi/spree-store-api.yaml
  type: apiKey
- bearerFormat: JWT
  description: JWT token for admin user authentication
  name: bearer_auth
  scheme: bearer
  sources:
  - openapi/spree-admin-api.yaml
  - openapi/spree-platform-api.yaml
  - openapi/spree-store-api.yaml
  - openapi/spree-storefront-api.yaml
  type: http
- description: 'Order token to authorize Cart and Checkout requests.


    [How to obtain X-Spree-Order-Token](../authentication#for-guest-users)'
  in: header
  name: orderToken
  parameter: X-Spree-Order-Token
  sources:
  - openapi/spree-storefront-api.yaml
  type: apiKey
slug: spree-authentication
source_filename: spree-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/spree-admin-api.yaml, openapi/spree-platform-api.yaml, openapi/spree-store-api.yaml,\n  openapi/spree-storefront-api.yaml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: api_key\n  type: apiKey\n  in: header\n  parameter: x-spree-api-key\n  description: Secret API key for admin access\n  sources:\n  - openapi/spree-admin-api.yaml\n  - openapi/spree-store-api.yaml\n- name: bearer_auth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: JWT token for admin user authentication\n  sources:\n  - openapi/spree-admin-api.yaml\n  - openapi/spree-platform-api.yaml\n  - openapi/spree-store-api.yaml\n  - openapi/spree-storefront-api.yaml\n- name: orderToken\n  type: apiKey\n  in: header\n  parameter: X-Spree-Order-Token\n  description: |-\n    Order token to authorize Cart and Checkout requests.\n\n    [How to obtain X-Spree-Order-Token](../authentication#for-guest-users)\n\
  \  sources:\n  - openapi/spree-storefront-api.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/spree/refs/heads/main/authentication/spree-authentication.yml
summary_line: apiKey/http · 3 schemes
tags:
- E-Commerce
- Headless Commerce
- Products
- Orders
- Inventory
- Payments
- Promotions
- Open Source
- Ruby on Rails
---
