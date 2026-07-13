---
api_key_in: []
api_specs:
- filename: terminal-shop-openapi.yml
  format: yaml
  label: Terminal Products API
  slug: products
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/terminal-shop/refs/heads/main/openapi/terminal-shop-openapi.yml
- filename: terminal-shop-openapi.yml
  format: yaml
  label: Terminal Cart API
  slug: cart
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/terminal-shop/refs/heads/main/openapi/terminal-shop-openapi.yml
- filename: terminal-shop-openapi.yml
  format: yaml
  label: Terminal Orders API
  slug: orders
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/terminal-shop/refs/heads/main/openapi/terminal-shop-openapi.yml
- filename: terminal-shop-openapi.yml
  format: yaml
  label: Terminal Subscriptions API
  slug: subscriptions
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/terminal-shop/refs/heads/main/openapi/terminal-shop-openapi.yml
- filename: terminal-shop-openapi.yml
  format: yaml
  label: Terminal Addresses & Cards API
  slug: addresses-cards
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/terminal-shop/refs/heads/main/openapi/terminal-shop-openapi.yml
- filename: terminal-shop-openapi.yml
  format: yaml
  label: Terminal Profile API
  slug: profile
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/terminal-shop/refs/heads/main/openapi/terminal-shop-openapi.yml
- filename: terminal-shop-openapi.yml
  format: yaml
  label: Terminal Tokens & Apps API
  slug: tokens
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/terminal-shop/refs/heads/main/openapi/terminal-shop-openapi.yml
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
- Developer
- SSH
- Ordering
---
