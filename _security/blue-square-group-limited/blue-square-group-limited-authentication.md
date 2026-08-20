---
api_key_in:
- cookie-session
api_specs:
- filename: blue-square-group-limited-streams.yml
  format: yaml
  label: GRVT Market Data API
  slug: grvt-market-data-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/blue-square-group-limited/refs/heads/main/asyncapi/blue-square-group-limited-streams.yml
auth_types:
- apiKey
- signature
description: ''
kind: authentication
layout: security
method: searched
name: Blue Square Group Limited Authentication
name_suffix: Authentication
oauth_flows: []
overview: Blue Square Group Limited secures its APIs with apiKey and signature across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Blue Square Group Limited
provider_slug: blue-square-group-limited
scheme_count: 2
schemes:
- in: cookie
  login_endpoint: https://edge.grvt.io/auth/api_key/login
  name: apiKeyLogin
  request: '{ "api_key": "<GRVT_TRADING_API_KEY>" }'
  returns: session cookie + sub_account_id
  testnet_login_endpoint: https://edge.testnet.grvt.io/auth/api_key/login
  type: apiKey
- name: requestSignature
  notes: 'Signature validation is enforced server-side (see error codes 2000-2008, 1012, 1400, 4015): unauthorized signer, expired signature/session key, payload mismatch, chain-id, and per-permission (trade/transfer) checks.'
  payload_format: EIP-712 typed data
  scheme: ecdsa-secp256k1
  session_keys: true
  signer_permissions:
  - trade
  - transfer
  type: signature
slug: blue-square-group-limited-authentication
source_filename: blue-square-group-limited-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://github.com/gravity-technologies/api-spec ; grvt-skills SKILL prerequisites\ndocs: https://api-docs.grvt.io/\nsummary:\n  types: [apiKey, signature]\n  api_key_in: [cookie-session]\n  signature_scheme: ecdsa-secp256k1\n  account_types: [trading, funding]\nmodel: >-\n  GRVT uses a two-part authentication model. (1) An API Key (issued from the GRVT exchange UI,\n  e.g. GRVT_TRADING_API_KEY / GRVT_FUNDING_API_KEY) is exchanged for a session at the edge host\n  (POST https://edge.grvt.io/auth/api_key/login -> {sub_account_id} + session cookie;\n  edge.testnet.grvt.io on testnet). (2) State-changing requests (orders, transfers, withdrawals)\n  are additionally signed with the private key associated with the API key using Ethereum-style\n  ECDSA (secp256k1) signatures over an EIP-712 typed payload; session keys with scoped signer\n  permissions (trade, transfer) and expirations are supported.\nschemes:\n  - name: apiKeyLogin\n\
  \    type: apiKey\n    in: cookie\n    login_endpoint: https://edge.grvt.io/auth/api_key/login\n    testnet_login_endpoint: https://edge.testnet.grvt.io/auth/api_key/login\n    request: '{ \"api_key\": \"<GRVT_TRADING_API_KEY>\" }'\n    returns: session cookie + sub_account_id\n  - name: requestSignature\n    type: signature\n    scheme: ecdsa-secp256k1\n    payload_format: EIP-712 typed data\n    session_keys: true\n    signer_permissions: [trade, transfer]\n    notes: >-\n      Signature validation is enforced server-side (see error codes 2000-2008, 1012, 1400, 4015):\n      unauthorized signer, expired signature/session key, payload mismatch, chain-id, and per-permission\n      (trade/transfer) checks.\npublic_endpoints: >-\n  All Market Data RPCs (instrument, ticker, orderbook, trade, candlestick, funding) are public\n  (auth_required=false); all Trading RPCs require authentication.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/blue-square-group-limited/refs/heads/main/authentication/blue-square-group-limited-authentication.yml
summary_line: apiKey/signature · 2 schemes
tags:
- Company
- Cryptocurrency
- Derivatives Exchange
- Trading
- Perpetual Futures
- Market Data
- Blockchain
- WebSocket
- Financial-Services
---
