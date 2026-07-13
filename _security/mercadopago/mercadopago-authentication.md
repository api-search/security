---
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Mercadopago Authentication
name_suffix: Authentication
oauth_flows: []
overview: Mercado Pago secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Mercado Pago
provider_slug: mercadopago
scheme_count: 1
schemes:
- bearerFormat: access_token
  description: 'Mercado Pago access token (ENV_ACCESS_TOKEN). Send as

    "Authorization: Bearer {ACCESS_TOKEN}". HTTPS is required.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/mercadopago-openapi.yml
  type: http
slug: mercadopago-authentication
source_filename: mercadopago-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/mercadopago-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: access_token\n  description: |-\n    Mercado Pago access token (ENV_ACCESS_TOKEN). Send as\n    \"Authorization: Bearer {ACCESS_TOKEN}\". HTTPS is required.\n  sources:\n  - openapi/mercadopago-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mercadopago/refs/heads/main/authentication/mercadopago-authentication.yml
summary_line: http · 1 scheme
tags:
- Payments
- Checkout
- Subscriptions
- POS
- QR
- SDKs
- Latin America
- Brazil
- Argentina
- Mexico
- Fintech
---
