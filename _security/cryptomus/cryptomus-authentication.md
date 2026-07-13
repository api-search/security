---
api_key_in:
- header
api_specs:
- filename: openapi.yml
  format: yaml
  label: Cryptomus Merchant Payment API
  slug: cryptomus-merchant-payment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cryptomus/refs/heads/main/openapi/openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Cryptomus Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cryptomus secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Cryptomus
provider_slug: cryptomus
scheme_count: 1
schemes:
- description: Merchant UUID from personal account settings. All requests also require a `sign` header computed as MD5(base64_encode(request_body) + API_KEY).
  in: header
  name: MerchantAuth
  parameter: merchant
  sources:
  - openapi/openapi.yml
  type: apiKey
slug: cryptomus-authentication
source_filename: cryptomus-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: MerchantAuth\n  type: apiKey\n  in: header\n  parameter: merchant\n  description: Merchant UUID from personal account settings. All requests also require a `sign`\n    header computed as MD5(base64_encode(request_body) + API_KEY).\n  sources:\n  - openapi/openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cryptomus/refs/heads/main/authentication/cryptomus-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Cryptocurrency
- Payments
- Invoices
- Payouts
- Exchange Rates
- Crypto Gateway
---
