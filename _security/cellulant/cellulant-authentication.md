---
api_key_in:
- header
api_specs:
- filename: cellulant-checkout-api-openapi.yml
  format: yaml
  label: Cellulant Tingg Checkout API
  slug: cellulant-tingg-checkout-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cellulant/refs/heads/main/openapi/cellulant-checkout-api-openapi.yml
- filename: cellulant-payouts-api-openapi.yml
  format: yaml
  label: Cellulant Tingg Payouts API
  slug: cellulant-tingg-payouts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cellulant/refs/heads/main/openapi/cellulant-payouts-api-openapi.yml
- filename: cellulant-engage-api-openapi.yml
  format: yaml
  label: Cellulant Tingg Engage API
  slug: cellulant-tingg-engage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cellulant/refs/heads/main/openapi/cellulant-engage-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Cellulant Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cellulant secures its APIs with apiKey and http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Cellulant
provider_slug: cellulant
scheme_count: 3
schemes:
- bearerFormat: JWT
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/cellulant-checkout-api-openapi.yml
  - openapi/cellulant-engage-api-openapi.yml
  type: http
- description: Merchant apiKey issued in the Tingg integration dashboard.
  in: header
  name: ApiKeyAuth
  parameter: apikey
  sources:
  - openapi/cellulant-checkout-api-openapi.yml
  type: apiKey
- description: Beep credentials supplied as Basic auth in addition to credentials in the payload.
  name: BasicAuth
  scheme: basic
  sources:
  - openapi/cellulant-payouts-api-openapi.yml
  type: http
slug: cellulant-authentication
source_filename: cellulant-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/cellulant-checkout-api-openapi.yml, openapi/cellulant-engage-api-openapi.yml,\n  openapi/cellulant-payouts-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/cellulant-checkout-api-openapi.yml\n  - openapi/cellulant-engage-api-openapi.yml\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: apikey\n  description: Merchant apiKey issued in the Tingg integration dashboard.\n  sources:\n  - openapi/cellulant-checkout-api-openapi.yml\n- name: BasicAuth\n  type: http\n  scheme: basic\n  description: Beep credentials supplied as Basic auth in addition to credentials in the payload.\n  sources:\n  - openapi/cellulant-payouts-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cellulant/refs/heads/main/authentication/cellulant-authentication.yml
summary_line: apiKey/http · 3 schemes
tags:
- Payments
- Mobile Money
- Checkout
- Payouts
- Disbursement
- Africa
- Pan-African
- Fintech
- Bank Transfer
- Cards
- Airtime
- Bill Payment
- SMS
- OTP
- Tingg
---
