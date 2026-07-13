---
api_key_in:
- query
api_specs:
- filename: lbank-spot-market-rest-api.json
  format: json
  label: LBank Spot Market REST API
  slug: spot-market-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lbank/refs/heads/main/openapi/lbank-spot-market-rest-api.json
- filename: lbank-spot-trading-rest-api.json
  format: json
  label: LBank Spot Trading REST API
  slug: spot-trading-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lbank/refs/heads/main/openapi/lbank-spot-trading-rest-api.json
- filename: lbank-wallet-rest-api.json
  format: json
  label: LBank Wallet REST API
  slug: wallet-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lbank/refs/heads/main/openapi/lbank-wallet-rest-api.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Lbank Authentication
name_suffix: Authentication
oauth_flows: []
overview: LBank secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: LBank
provider_slug: lbank
scheme_count: 1
schemes:
- description: LBank API key with HMAC or RSA request signing
  in: query
  name: ApiKeyAuth
  parameter: api_key
  sources:
  - openapi/lbank-spot-trading-rest-api.json
  - openapi/lbank-wallet-rest-api.json
  type: apiKey
slug: lbank-authentication
source_filename: lbank-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/lbank-spot-trading-rest-api.json, openapi/lbank-wallet-rest-api.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: query\n  parameter: api_key\n  description: LBank API key with HMAC or RSA request signing\n  sources:\n  - openapi/lbank-spot-trading-rest-api.json\n  - openapi/lbank-wallet-rest-api.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lbank/refs/heads/main/authentication/lbank-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Cryptocurrency
- Exchange
- Trading
- Market Data
- Finance
- Blockchain
---
