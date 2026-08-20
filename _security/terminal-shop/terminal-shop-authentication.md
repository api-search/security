---
api_key_in: []
api_specs:
- filename: terminal-shop-address-api-openapi.yml
  format: yaml
  label: Terminal Address API
  slug: terminal-shop-address-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/terminal-shop/refs/heads/main/openapi/terminal-shop-address-api-openapi.yml
- filename: terminal-shop-app-api-openapi.yml
  format: yaml
  label: Terminal App API
  slug: terminal-shop-app-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/terminal-shop/refs/heads/main/openapi/terminal-shop-app-api-openapi.yml
- filename: terminal-shop-card-api-openapi.yml
  format: yaml
  label: Terminal Card API
  slug: terminal-shop-card-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/terminal-shop/refs/heads/main/openapi/terminal-shop-card-api-openapi.yml
- filename: terminal-shop-cart-api-openapi.yml
  format: yaml
  label: Terminal Cart API
  slug: terminal-shop-cart-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/terminal-shop/refs/heads/main/openapi/terminal-shop-cart-api-openapi.yml
- filename: terminal-shop-email-api-openapi.yml
  format: yaml
  label: Terminal Email API
  slug: terminal-shop-email-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/terminal-shop/refs/heads/main/openapi/terminal-shop-email-api-openapi.yml
- filename: terminal-shop-order-api-openapi.yml
  format: yaml
  label: Terminal Order API
  slug: terminal-shop-order-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/terminal-shop/refs/heads/main/openapi/terminal-shop-order-api-openapi.yml
- filename: terminal-shop-product-api-openapi.yml
  format: yaml
  label: Terminal Product API
  slug: terminal-shop-product-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/terminal-shop/refs/heads/main/openapi/terminal-shop-product-api-openapi.yml
- filename: terminal-shop-profile-api-openapi.yml
  format: yaml
  label: Terminal Profile API
  slug: terminal-shop-profile-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/terminal-shop/refs/heads/main/openapi/terminal-shop-profile-api-openapi.yml
- filename: terminal-shop-subscription-api-openapi.yml
  format: yaml
  label: Terminal Subscription API
  slug: terminal-shop-subscription-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/terminal-shop/refs/heads/main/openapi/terminal-shop-subscription-api-openapi.yml
- filename: terminal-shop-token-api-openapi.yml
  format: yaml
  label: Terminal Token API
  slug: terminal-shop-token-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/terminal-shop/refs/heads/main/openapi/terminal-shop-token-api-openapi.yml
- filename: terminal-shop-view-api-openapi.yml
  format: yaml
  label: Terminal View API
  slug: terminal-shop-view-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/terminal-shop/refs/heads/main/openapi/terminal-shop-view-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Terminal Shop Authentication
name_suffix: Authentication
oauth_flows: []
overview: Terminal secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Terminal
provider_slug: terminal-shop
scheme_count: 1
schemes:
- description: 'Personal access token (`trm_live_*` in production, `trm_test_*` in the dev sandbox) or OAuth 2.0 access token, passed as `Authorization: Bearer <token>`.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/terminal-shop-openapi.yml
  type: http
slug: terminal-shop-authentication
source_filename: terminal-shop-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/terminal-shop-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'Personal access token (`trm_live_*` in production, `trm_test_*` in the dev sandbox)\n    or OAuth 2.0 access token, passed as `Authorization: Bearer <token>`.'\n  sources:\n  - openapi/terminal-shop-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/terminal-shop/refs/heads/main/authentication/terminal-shop-authentication.yml
summary_line: http · 1 scheme
tags:
- Coffee
- E-Commerce
- Developers
- SSH
- Ordering
---
