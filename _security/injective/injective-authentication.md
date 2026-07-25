---
api_key_in: []
auth_types:
- none-public
- signature-based-transactions
description: 'Injective''s public read APIs (Chain LCD/REST, Tendermint RPC, and the Indexer gRPC/gRPC-web/REST + Chain Stream WebSocket) are open, permissionless endpoints that require no API key or OAuth token — they are rate-limited public infrastructure. WRITE access is not key-based: state changes are performed by broadcasting cryptographically signed transactions. Signing uses either native Cosmos secp256k1 (bech32 inj1... accounts) or Ethereum EIP-712 typed-data signing (0x... keys), with optional AuthZ grant delegation for session-based auto-signing.'
kind: authentication
layout: security
method: searched
name: Injective Authentication
name_suffix: Authentication
oauth_flows: []
overview: Injective secures its APIs with none-public and signature-based-transactions across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Injective
provider_slug: injective
scheme_count: 4
schemes:
- applies_to:
  - Chain LCD/REST
  - Tendermint RPC
  - Indexer gRPC/REST
  - Chain Stream WS
  name: public-read
  note: no credential required; rate-limited public sentry endpoints
  type: none
- applies_to:
  - transaction broadcast
  name: cosmos-signature
  scheme: secp256k1 (Cosmos), bech32 address inj1...
  type: transaction-signature
- applies_to:
  - transaction broadcast
  - Injective EVM
  name: eip712-signature
  scheme: EIP-712 typed data, EVM address 0x...
  type: transaction-signature
- docs: https://github.com/InjectiveLabs/agent-skills (injective-trading-autosign)
  name: authz-delegation
  scheme: Cosmos AuthZ MsgGrant for session-based/auto signing
  type: on-chain-grant
slug: injective-authentication
source_filename: injective-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://docs.injective.network/developers-native/query-chain + query-indexer\nsummary:\n  types: [none-public, signature-based-transactions]\n  api_key_in: []\n  oauth2_flows: []\ndescription: >-\n  Injective's public read APIs (Chain LCD/REST, Tendermint RPC, and the Indexer\n  gRPC/gRPC-web/REST + Chain Stream WebSocket) are open, permissionless endpoints\n  that require no API key or OAuth token — they are rate-limited public\n  infrastructure. WRITE access is not key-based: state changes are performed by\n  broadcasting cryptographically signed transactions. Signing uses either native\n  Cosmos secp256k1 (bech32 inj1... accounts) or Ethereum EIP-712 typed-data signing\n  (0x... keys), with optional AuthZ grant delegation for session-based auto-signing.\nschemes:\n- name: public-read\n  type: none\n  applies_to: [Chain LCD/REST, Tendermint RPC, Indexer gRPC/REST, Chain Stream WS]\n  note: no credential required; rate-limited\
  \ public sentry endpoints\n- name: cosmos-signature\n  type: transaction-signature\n  scheme: secp256k1 (Cosmos), bech32 address inj1...\n  applies_to: [transaction broadcast]\n- name: eip712-signature\n  type: transaction-signature\n  scheme: EIP-712 typed data, EVM address 0x...\n  applies_to: [transaction broadcast, Injective EVM]\n- name: authz-delegation\n  type: on-chain-grant\n  scheme: Cosmos AuthZ MsgGrant for session-based/auto signing\n  docs: https://github.com/InjectiveLabs/agent-skills (injective-trading-autosign)\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/injective/refs/heads/main/authentication/injective-authentication.yml
summary_line: none-public/signature-based-transactions · 4 schemes
tags:
- Company
- Crypto
- Blockchain
- DeFi
- Trading
- Derivatives
- Web3
- Layer 1
- Cosmos
- Tokenization
- Payments
- AI Agents
---
