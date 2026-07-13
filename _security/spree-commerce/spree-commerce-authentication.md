---
api_key_in:
- header
api_specs:
- filename: spree-commerce-store-api-openapi.yml
  format: yaml
  label: Spree Store API
  slug: store-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spree-commerce/refs/heads/main/openapi/spree-commerce-store-api-openapi.yml
- filename: spree-commerce-admin-api-openapi.yml
  format: yaml
  label: Spree Admin API
  slug: admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spree-commerce/refs/heads/main/openapi/spree-commerce-admin-api-openapi.yml
- filename: spree-commerce-platform-api-openapi.yml
  format: yaml
  label: Spree Platform API
  slug: platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spree-commerce/refs/heads/main/openapi/spree-commerce-platform-api-openapi.yml
- filename: spree-commerce-storefront-api-openapi.yml
  format: yaml
  label: Spree Storefront API (JSON:API)
  slug: storefront-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spree-commerce/refs/heads/main/openapi/spree-commerce-storefront-api-openapi.yml
- filename: spree-commerce-oauth-api-openapi.yml
  format: yaml
  label: Spree OAuth API
  slug: oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spree-commerce/refs/heads/main/openapi/spree-commerce-oauth-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Spree Commerce Authentication
name_suffix: Authentication
oauth_flows: []
overview: Spree Commerce secures its APIs with apiKey and http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Spree Commerce
provider_slug: spree-commerce
scheme_count: 3
schemes:
- description: Secret API key for admin access
  in: header
  name: api_key
  parameter: x-spree-api-key
  sources:
  - openapi/spree-commerce-admin-api-openapi.yml
  - openapi/spree-commerce-store-api-openapi.yml
  type: apiKey
- bearerFormat: JWT
  description: JWT token for admin user authentication
  name: bearer_auth
  scheme: bearer
  sources:
  - openapi/spree-commerce-admin-api-openapi.yml
  - openapi/spree-commerce-platform-api-openapi.yml
  - openapi/spree-commerce-store-api-openapi.yml
  - openapi/spree-commerce-storefront-api-openapi.yml
  type: http
- description: 'Order token to authorize Cart and Checkout requests.


    [How to obtain X-Spree-Order-Token](../authentication#for-guest-users)'
  in: header
  name: orderToken
  parameter: X-Spree-Order-Token
  sources:
  - openapi/spree-commerce-storefront-api-openapi.yml
  type: apiKey
slug: spree-commerce-authentication
source_filename: spree-commerce-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/spree-commerce-admin-api-openapi.yml, openapi/spree-commerce-platform-api-openapi.yml,\n  openapi/spree-commerce-store-api-openapi.yml, openapi/spree-commerce-storefront-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: api_key\n  type: apiKey\n  in: header\n  parameter: x-spree-api-key\n  description: Secret API key for admin access\n  sources:\n  - openapi/spree-commerce-admin-api-openapi.yml\n  - openapi/spree-commerce-store-api-openapi.yml\n- name: bearer_auth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: JWT token for admin user authentication\n  sources:\n  - openapi/spree-commerce-admin-api-openapi.yml\n  - openapi/spree-commerce-platform-api-openapi.yml\n  - openapi/spree-commerce-store-api-openapi.yml\n  - openapi/spree-commerce-storefront-api-openapi.yml\n- name: orderToken\n  type: apiKey\n  in: header\n  parameter: X-Spree-Order-Token\n\
  \  description: |-\n    Order token to authorize Cart and Checkout requests.\n\n    [How to obtain X-Spree-Order-Token](../authentication#for-guest-users)\n  sources:\n  - openapi/spree-commerce-storefront-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/spree-commerce/refs/heads/main/authentication/spree-commerce-authentication.yml
summary_line: apiKey/http · 3 schemes
tags:
- Commerce
- Headless
- eCommerce
- Open Source
- Ruby on Rails
- Ruby
- TypeScript
---
