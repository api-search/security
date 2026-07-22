---
api_key_in:
- header
api_specs:
- filename: robinhood-crypto-trading-openapi.yml
  format: yaml
  label: Robinhood Crypto Trading API
  slug: robinhood-crypto-trading-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/robinhood/refs/heads/main/openapi/robinhood-crypto-trading-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Robinhood Authentication
name_suffix: Authentication
oauth_flows: []
overview: Robinhood secures its APIs with apiKey across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Robinhood
provider_slug: robinhood
scheme_count: 3
schemes:
- description: The API key issued in the Robinhood API Credentials Portal.
  in: header
  name: ApiKeyAuth
  parameter: x-api-key
  sources:
  - openapi/robinhood-crypto-trading-openapi.yml
  type: apiKey
- description: Current UNIX timestamp (seconds) included in the signed message.
  in: header
  name: ApiTimestamp
  parameter: x-timestamp
  sources:
  - openapi/robinhood-crypto-trading-openapi.yml
  type: apiKey
- description: Base64 Ed25519 signature over api_key + timestamp + path + method + body.
  in: header
  name: ApiSignature
  parameter: x-signature
  sources:
  - openapi/robinhood-crypto-trading-openapi.yml
  type: apiKey
slug: robinhood-authentication
source_filename: robinhood-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: derived\nsource: openapi/robinhood-crypto-trading-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: The API key issued in the Robinhood API Credentials Portal.\n  sources:\n  - openapi/robinhood-crypto-trading-openapi.yml\n- name: ApiTimestamp\n  type: apiKey\n  in: header\n  parameter: x-timestamp\n  description: Current UNIX timestamp (seconds) included in the signed message.\n  sources:\n  - openapi/robinhood-crypto-trading-openapi.yml\n- name: ApiSignature\n  type: apiKey\n  in: header\n  parameter: x-signature\n  description: Base64 Ed25519 signature over api_key + timestamp + path + method + body.\n  sources:\n  - openapi/robinhood-crypto-trading-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/robinhood/refs/heads/main/authentication/robinhood-authentication.yml
summary_line: apiKey · 3 schemes
tags:
- Company
- Fintech
- Cryptocurrency
- Trading
- Brokerage
- Investing
- Financial Services
- Crypto
---
