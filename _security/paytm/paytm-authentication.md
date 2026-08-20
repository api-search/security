---
api_key_in:
- header
api_specs:
- filename: paytm-payments-api-openapi.yml
  format: yaml
  label: Paytm Payments API
  slug: paytm-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paytm/refs/heads/main/openapi/paytm-payments-api-openapi.yml
- filename: paytm-refunds-api-openapi.yml
  format: yaml
  label: Paytm Refunds API
  slug: paytm-refunds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paytm/refs/heads/main/openapi/paytm-refunds-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Paytm Authentication
name_suffix: Authentication
oauth_flows: []
overview: Paytm secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Paytm
provider_slug: paytm
scheme_count: 1
schemes:
- description: Checksum signature computed over the request body using Paytm's merchant key. Carried in the request head.signature property and/or as a request header per endpoint guidance.
  in: header
  name: paytmChecksum
  parameter: signature
  sources:
  - openapi/paytm-openapi.yml
  type: apiKey
slug: paytm-authentication
source_filename: paytm-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/paytm-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: paytmChecksum\n  type: apiKey\n  in: header\n  parameter: signature\n  description: Checksum signature computed over the request body using Paytm's merchant key.\n    Carried in the request head.signature property and/or as a request header per endpoint guidance.\n  sources:\n  - openapi/paytm-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/paytm/refs/heads/main/authentication/paytm-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Payments
- Payment Gateway
- UPI
- Payouts
- Subscription
- Refunds
- Settlement
- QR
- EDC
- Fintech
- India
---
