---
api_key_in: []
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
