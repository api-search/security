---
api_key_in:
- header
api_specs:
- filename: coinsph-account-openapi.json
  format: json
  label: Coins.ph Coins Pro — Account
  slug: coinsph-coins-pro-account
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coinsph/refs/heads/main/openapi/coinsph-account-openapi.json
- filename: coinsph-account-validation-openapi.json
  format: json
  label: Coins.ph Account Validation
  slug: coinsph-account-validation
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coinsph/refs/heads/main/openapi/coinsph-account-validation-openapi.json
- filename: coinsph-convert-openapi.json
  format: json
  label: Coins.ph Coins Pro — Convert
  slug: coinsph-coins-pro-convert
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coinsph/refs/heads/main/openapi/coinsph-convert-openapi.json
- filename: coinsph-listenkey-openapi.json
  format: json
  label: Coins.ph Coins Pro — User Data Stream
  slug: coinsph-coins-pro-user-data-stream
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coinsph/refs/heads/main/openapi/coinsph-listenkey-openapi.json
- filename: coinsph-markets-openapi.json
  format: json
  label: Coins.ph Coins Pro — Market Data
  slug: coinsph-coins-pro-market-data
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coinsph/refs/heads/main/openapi/coinsph-markets-openapi.json
- filename: coinsph-payment-openapi.json
  format: json
  label: Coins.ph Payment / Partner Integration
  slug: coinsph-payment-partner-integration
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coinsph/refs/heads/main/openapi/coinsph-payment-openapi.json
- filename: coinsph-ramp-openapi.json
  format: json
  label: Coins.ph ON/OFF Ramp
  slug: coinsph-onoff-ramp
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coinsph/refs/heads/main/openapi/coinsph-ramp-openapi.json
- filename: coinsph-spot-openapi.json
  format: json
  label: Coins.ph Coins Pro — Spot Trading
  slug: coinsph-coins-pro-spot-trading
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coinsph/refs/heads/main/openapi/coinsph-spot-openapi.json
- filename: coinsph-sub-account-openapi.json
  format: json
  label: Coins.ph Coins Pro — Sub-Account
  slug: coinsph-coins-pro-sub-account
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coinsph/refs/heads/main/openapi/coinsph-sub-account-openapi.json
- filename: coinsph-system-openapi.json
  format: json
  label: Coins.ph Coins Pro — System
  slug: coinsph-coins-pro-system
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coinsph/refs/heads/main/openapi/coinsph-system-openapi.json
- filename: coinsph-wallet-openapi.json
  format: json
  label: Coins.ph Coins Pro — Wallet
  slug: coinsph-coins-pro-wallet
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coinsph/refs/heads/main/openapi/coinsph-wallet-openapi.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Coinsph Authentication
name_suffix: Authentication
oauth_flows: []
overview: Coins.ph secures its APIs with apiKey across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Coins.ph
provider_slug: coinsph
scheme_count: 3
schemes:
- in: header
  name: ApiKeyAuth
  parameter: X-COINS-APIKEY
  sources:
  - openapi/coinsph-account-openapi.json
  - openapi/coinsph-account-validation-openapi.json
  - openapi/coinsph-convert-openapi.json
  - openapi/coinsph-payment-openapi.json
  - openapi/coinsph-ramp-openapi.json
  - openapi/coinsph-spot-openapi.json
  - openapi/coinsph-sub-account-openapi.json
  - openapi/coinsph-wallet-openapi.json
  type: apiKey
- description: Unix timestamp of the request
  in: header
  name: TimestampAuth
  parameter: Timestamp
  sources:
  - openapi/coinsph-payment-openapi.json
  - openapi/coinsph-ramp-openapi.json
  type: apiKey
- description: HMAC-SHA256 signature of the request
  in: header
  name: SignatureAuth
  parameter: Signature
  sources:
  - openapi/coinsph-payment-openapi.json
  - openapi/coinsph-ramp-openapi.json
  type: apiKey
slug: coinsph-authentication
source_filename: coinsph-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: derived\nsource: openapi/coinsph-account-openapi.json, openapi/coinsph-account-validation-openapi.json,\n  openapi/coinsph-convert-openapi.json, openapi/coinsph-payment-openapi.json, openapi/coinsph-ramp-openapi.json,\n  openapi/coinsph-spot-openapi.json, openapi/coinsph-sub-account-openapi.json, openapi/coinsph-wallet-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-COINS-APIKEY\n  sources:\n  - openapi/coinsph-account-openapi.json\n  - openapi/coinsph-account-validation-openapi.json\n  - openapi/coinsph-convert-openapi.json\n  - openapi/coinsph-payment-openapi.json\n  - openapi/coinsph-ramp-openapi.json\n  - openapi/coinsph-spot-openapi.json\n  - openapi/coinsph-sub-account-openapi.json\n  - openapi/coinsph-wallet-openapi.json\n- name: TimestampAuth\n  type: apiKey\n  in: header\n  parameter: Timestamp\n  description: Unix timestamp of the request\n\
  \  sources:\n  - openapi/coinsph-payment-openapi.json\n  - openapi/coinsph-ramp-openapi.json\n- name: SignatureAuth\n  type: apiKey\n  in: header\n  parameter: Signature\n  description: HMAC-SHA256 signature of the request\n  sources:\n  - openapi/coinsph-payment-openapi.json\n  - openapi/coinsph-ramp-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/coinsph/refs/heads/main/authentication/coinsph-authentication.yml
summary_line: apiKey · 3 schemes
tags:
- Company
- Crypto
- Cryptocurrency Exchange
- Payments
- Fintech
- Wallet
- Philippines
- Trading
---
