---
api_key_in: []
api_specs:
- filename: setup
  format: yaml
  label: Quai Network JSON-RPC API
  slug: quai-network-json-rpc-api
  spec_type: Postman
  url: https://docs.qu.ai/build/apis/postman/setup
auth_types:
- none
description: ''
kind: authentication
layout: security
method: searched
name: Quai Network Authentication
name_suffix: Authentication
oauth_flows: []
overview: Quai Network secures its APIs with none across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Quai Network
provider_slug: quai-network
scheme_count: 2
schemes:
- detail: No credential required for read methods or for submitting pre-signed transactions.
  name: public-rpc
  type: none
- detail: secp256k1 transaction signatures (via the Quais SDK) authorize on-chain state changes; Qi UTXO transactions use the Qi ledger signing model.
  name: transaction-signature
  type: signature
slug: quai-network-authentication
source_filename: quai-network-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://docs.qu.ai/build/playground/overview + https://docs.qu.ai/build/introduction\nsummary:\n  types: [none]\n  detail: >-\n    The Quai Network JSON-RPC and GraphQL endpoints are public and unauthenticated\n    (no API key or token). This is standard for a public blockchain node RPC.\n    State-changing operations are not authorized by an API credential but by\n    cryptographic transaction signatures: clients sign transactions with an\n    account private key (Quais SDK Wallet / QuaiHDWallet / QiHDWallet) and submit\n    the signed, Protobuf-encoded transaction via quai_sendRawTransaction.\nschemes:\n- name: public-rpc\n  type: none\n  detail: No credential required for read methods or for submitting pre-signed transactions.\n- name: transaction-signature\n  type: signature\n  detail: secp256k1 transaction signatures (via the Quais SDK) authorize on-chain state changes; Qi UTXO transactions use the Qi ledger signing model.\n\
  notes:\n- Operators exposing a private/authenticated node may front the RPC with their own gateway auth; that is deployment-specific and not part of the public API contract.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/quai-network/refs/heads/main/authentication/quai-network-authentication.yml
summary_line: none · 2 schemes
tags:
- Company
- Layer 1
- Blockchain
- Cryptocurrency
- Web3
- Smart Contracts
- EVM
- JSON-RPC
- Proof of Work
- Developer Tools
---
