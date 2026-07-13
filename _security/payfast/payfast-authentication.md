---
api_key_in:
- header
api_specs:
- filename: openapi.yml
  format: yaml
  label: PayFast Payments API
  slug: payfast-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payfast/refs/heads/main/openapi/openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Payfast Authentication
name_suffix: Authentication
oauth_flows: []
overview: PayFast secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: PayFast
provider_slug: payfast
scheme_count: 1
schemes:
- description: PayFast API authentication uses an MD5 signature derived from the merchant ID, passphrase, timestamp, and request data. Required headers include merchant-id, version, timestamp, and signature.
  in: header
  name: merchantAuth
  parameter: merchant-id
  sources:
  - openapi/openapi.yml
  type: apiKey
slug: payfast-authentication
source_filename: payfast-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: merchantAuth\n  type: apiKey\n  in: header\n  parameter: merchant-id\n  description: PayFast API authentication uses an MD5 signature derived from the merchant ID,\n    passphrase, timestamp, and request data. Required headers include merchant-id, version,\n    timestamp, and signature.\n  sources:\n  - openapi/openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/payfast/refs/heads/main/authentication/payfast-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Payments
- Payment Gateway
- South Africa
- Subscriptions
- Recurring Billing
- Tokenization
- Instant EFT
- QR Code Payments
- Refunds
- Fintech
---
