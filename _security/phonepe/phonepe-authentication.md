---
api_key_in:
- header
api_specs:
- filename: phonepe-openapi.yml
  format: yaml
  label: PhonePe Payment Gateway API
  slug: pg
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phonepe/refs/heads/main/openapi/phonepe-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Phonepe Authentication
name_suffix: Authentication
oauth_flows: []
overview: PhonePe secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: PhonePe
provider_slug: phonepe
scheme_count: 1
schemes:
- description: 'Bearer-style merchant auth token issued by PhonePe. Sent as

    `Authorization: O-Bearer <merchant-auth-token>`. Partner integrations

    also include `X-MERCHANT-ID: <end-merchant-id>`.'
  in: header
  name: merchantToken
  parameter: Authorization
  sources:
  - openapi/phonepe-openapi.yml
  type: apiKey
slug: phonepe-authentication
source_filename: phonepe-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/phonepe-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: merchantToken\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: |-\n    Bearer-style merchant auth token issued by PhonePe. Sent as\n    `Authorization: O-Bearer <merchant-auth-token>`. Partner integrations\n    also include `X-MERCHANT-ID: <end-merchant-id>`.\n  sources:\n  - openapi/phonepe-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/phonepe/refs/heads/main/authentication/phonepe-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Payments
- Payment Gateway
- UPI
- QR
- EDC
- App Store
- Fintech
- India
---
