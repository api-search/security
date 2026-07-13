---
api_key_in: []
api_specs:
- filename: checkout
  format: yaml
  label: Verifone Checkout API
  slug: verifone-checkout-api
  spec_type: OpenAPI
  url: https://docs.verifone.com/api-reference/open-api-references/checkout
- filename: ecommerce-api.json
  format: json
  label: Verifone eCommerce API
  slug: verifone-ecommerce-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/verifone/refs/heads/main/openapi/ecommerce-api.json
- filename: customer
  format: yaml
  label: Verifone Customer API
  slug: verifone-customer-api
  spec_type: OpenAPI
  url: https://docs.verifone.com/api-reference/open-api-references/customer
- filename: order-service
  format: yaml
  label: Verifone Order Service API
  slug: verifone-order-service-api
  spec_type: OpenAPI
  url: https://docs.verifone.com/api-reference/open-api-references/order-service
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Verifone Authentication
name_suffix: Authentication
oauth_flows: []
overview: Verifone secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Verifone
provider_slug: verifone
scheme_count: 2
schemes:
- bearerFormat: JWT
  description: 'JWT Bearer token. Pass as: `Authorization: Bearer <token>`. The JWT must be signed with your Verifone-provisioned private key and must include `entity_id`, `sub` (user_id), and `roles` claims.'
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/3ds-authentication-api.json
  - openapi/checkout-api.json
  - openapi/customer-api.json
  - openapi/paypal-ecommerce-api.json
  - openapi/reporting-api.json
  type: http
- description: 'HTTP Basic authentication. Pass base64-encoded `username:password` as: `Authorization: Basic <credentials>`.'
  name: BasicAuth
  scheme: basic
  sources:
  - openapi/3ds-authentication-api.json
  - openapi/checkout-api.json
  - openapi/customer-api.json
  - openapi/ecommerce-api.json
  - openapi/reporting-api.json
  type: http
slug: verifone-authentication
source_filename: verifone-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/3ds-authentication-api.json, openapi/checkout-api.json, openapi/customer-api.json,\n  openapi/ecommerce-api.json, openapi/paypal-ecommerce-api.json, openapi/reporting-api.json\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: 'JWT Bearer token. Pass as: `Authorization: Bearer <token>`. The JWT must be\n    signed with your Verifone-provisioned private key and must include `entity_id`, `sub` (user_id),\n    and `roles` claims.'\n  sources:\n  - openapi/3ds-authentication-api.json\n  - openapi/checkout-api.json\n  - openapi/customer-api.json\n  - openapi/paypal-ecommerce-api.json\n  - openapi/reporting-api.json\n- name: BasicAuth\n  type: http\n  scheme: basic\n  description: 'HTTP Basic authentication. Pass base64-encoded `username:password` as: `Authorization:\n    Basic <credentials>`.'\n  sources:\n  - openapi/3ds-authentication-api.json\n\
  \  - openapi/checkout-api.json\n  - openapi/customer-api.json\n  - openapi/ecommerce-api.json\n  - openapi/reporting-api.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/verifone/refs/heads/main/authentication/verifone-authentication.yml
summary_line: http · 2 schemes
tags:
- Payments
- POS
- Terminal Management
- eCommerce
- FinTech
- Payment Processing
- Omnichannel
---
