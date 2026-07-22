---
api_key_in:
- header
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Loop Crypto Authentication
name_suffix: Authentication
oauth_flows: []
overview: Loop Crypto secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Loop Crypto
provider_slug: loop-crypto
scheme_count: 2
schemes:
- description: Loop-issued API key. Created in the dashboard developer tab; keys can be restricted to a permission set.
  in: header
  name: api-key
  parameter: api-key
  sources:
  - https://docs.loopcrypto.xyz/docs/get-set-up
  type: apiKey
- description: Identifier for the Loop entity the request acts on behalf of. Required alongside api-key.
  in: header
  name: entity-id
  parameter: entity-id
  sources:
  - https://docs.loopcrypto.xyz/docs/get-set-up
  type: apiKey
slug: loop-crypto-authentication
source_filename: loop-crypto-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://docs.loopcrypto.xyz/docs/get-set-up\ndocs: https://docs.loopcrypto.xyz/docs/authorization-signatures\nsummary:\n  types: [apiKey]\n  api_key_in: [header]\n  oauth2_flows: []\n  notes: >-\n    Loop Crypto authenticates API requests with two required headers rather than a\n    single bearer token: an api-key header carrying a Loop-issued key, and an\n    entity-id header identifying the calling entity. Keys are created in the Loop\n    dashboard developer tab. Loop issues \"restricted\" keys scoped to a granular set\n    of API permissions (for example the GetWebhooks permission is required to call\n    the List Webhooks endpoint), so each key only grants the operations it was\n    provisioned for.\nschemes:\n  - name: api-key\n    type: apiKey\n    in: header\n    parameter: api-key\n    description: Loop-issued API key. Created in the dashboard developer tab; keys can be restricted to a permission set.\n    sources:\
  \ [https://docs.loopcrypto.xyz/docs/get-set-up]\n  - name: entity-id\n    type: apiKey\n    in: header\n    parameter: entity-id\n    description: Identifier for the Loop entity the request acts on behalf of. Required alongside api-key.\n    sources: [https://docs.loopcrypto.xyz/docs/get-set-up]\npermissions_model:\n  style: restricted-key-permissions\n  description: Restricted API keys are provisioned with a discrete list of permissions gating which operations they may call.\n  example_permissions:\n    - GetWebhooks\nwebhook_verification:\n  method: authorization-signatures\n  docs: https://docs.loopcrypto.xyz/docs/authorization-signatures\n  description: Inbound webhook deliveries are verified with authorization signatures so recipients can confirm the payload originated from Loop.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/loop-crypto/refs/heads/main/authentication/loop-crypto-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Company
- Payments
- Cryptocurrency
- Stablecoins
- Web3
- Payment Processing
- Billing
- Solana
- Ethereum
---
