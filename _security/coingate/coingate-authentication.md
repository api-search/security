---
api_key_in: []
api_specs:
- filename: openapi.json
  format: json
  label: CoinGate Payment Gateway API
  slug: coingate-payment-gateway-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coingate/refs/heads/main/openapi/openapi.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Coingate Authentication
name_suffix: Authentication
oauth_flows: []
overview: CoinGate secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: CoinGate
provider_slug: coingate
scheme_count: 1
schemes:
- description: API Token authentication. Obtain your API token from the CoinGate merchant dashboard.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/openapi.json
  type: http
slug: coingate-authentication
source_filename: coingate-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: API Token authentication. Obtain your API token from the CoinGate merchant dashboard.\n  sources:\n  - openapi/openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/coingate/refs/heads/main/authentication/coingate-authentication.yml
summary_line: http · 1 scheme
tags:
- Cryptocurrency
- Payments
- Payment Gateway
- Crypto
- Fintech
- Bitcoin
- Ethereum
- Merchant Services
---
