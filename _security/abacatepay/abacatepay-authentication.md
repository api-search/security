---
api_key_in: []
api_specs:
- filename: abacatepay-billing-api-openapi.yml
  format: yaml
  label: AbacatePay Billing API
  slug: abacatepay-billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/abacatepay/refs/heads/main/openapi/abacatepay-billing-api-openapi.yml
- filename: abacatepay-coupon-api-openapi.yml
  format: yaml
  label: AbacatePay Coupon API
  slug: abacatepay-coupon-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/abacatepay/refs/heads/main/openapi/abacatepay-coupon-api-openapi.yml
- filename: abacatepay-customer-api-openapi.yml
  format: yaml
  label: AbacatePay Customer API
  slug: abacatepay-customer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/abacatepay/refs/heads/main/openapi/abacatepay-customer-api-openapi.yml
- filename: abacatepay-pix-qr-code-api-openapi.yml
  format: yaml
  label: AbacatePay Pix QR Code API
  slug: abacatepay-pix-qr-code-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/abacatepay/refs/heads/main/openapi/abacatepay-pix-qr-code-api-openapi.yml
- filename: abacatepay-withdraw-api-openapi.yml
  format: yaml
  label: AbacatePay Withdraw API
  slug: abacatepay-withdraw-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/abacatepay/refs/heads/main/openapi/abacatepay-withdraw-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Abacatepay Authentication
name_suffix: Authentication
oauth_flows: []
overview: AbacatePay secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: AbacatePay
provider_slug: abacatepay
scheme_count: 1
schemes:
- bearerFormat: API Key
  description: 'Authenticate with your AbacatePay API key as a Bearer token: `Authorization: Bearer <abacatepay-api-key>`.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/abacatepay-openapi.yml
  type: http
slug: abacatepay-authentication
source_filename: abacatepay-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/abacatepay-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: API Key\n  description: 'Authenticate with your AbacatePay API key as a Bearer token: `Authorization:\n    Bearer <abacatepay-api-key>`.'\n  sources:\n  - openapi/abacatepay-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/abacatepay/refs/heads/main/authentication/abacatepay-authentication.yml
summary_line: http · 1 scheme
tags:
- Payments
- Pix
- Brazil
- Fintech
- Developers
---
