---
api_key_in:
- cookie
- header
api_specs:
- filename: openapi.yaml
  format: yaml
  label: Safe Transaction Service API
  slug: transaction-service
  spec_type: OpenAPI
  url: https://safe-transaction-mainnet.safe.global/api/schema/swagger-ui/
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Gnosis Safe Authentication
name_suffix: Authentication
oauth_flows: []
overview: Safe (Gnosis Safe) secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Safe (Gnosis Safe)
provider_slug: gnosis-safe
scheme_count: 2
schemes:
- in: cookie
  name: cookieAuth
  parameter: sessionid
  sources:
  - openapi/gnosis-safe-transaction-service-openapi.json
  type: apiKey
- description: Token-based authentication with required prefix "Token"
  in: header
  name: tokenAuth
  parameter: Authorization
  sources:
  - openapi/gnosis-safe-transaction-service-openapi.json
  type: apiKey
slug: gnosis-safe-authentication
source_filename: gnosis-safe-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/gnosis-safe-transaction-service-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - cookie\n  - header\nschemes:\n- name: cookieAuth\n  type: apiKey\n  in: cookie\n  parameter: sessionid\n  sources:\n  - openapi/gnosis-safe-transaction-service-openapi.json\n- name: tokenAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Token-based authentication with required prefix \"Token\"\n  sources:\n  - openapi/gnosis-safe-transaction-service-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gnosis-safe/refs/heads/main/authentication/gnosis-safe-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Multisig
- Smart Contract
- Ethereum
- Web3
- Blockchain
- DeFi
- Safe
- Gnosis
- Wallet
---
