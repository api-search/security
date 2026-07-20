---
api_key_in: []
auth_types:
- none
description: Aurora's public JSON-RPC endpoints (mainnet.aurora.dev and testnet.aurora.dev) are open and require no API key or bearer token; access control is performed at the protocol layer by cryptographic signing of transactions with an Ethereum-compatible private key (secp256k1), exactly as on Ethereum. Read (eth_call, eth_getBalance, etc.) calls are unauthenticated; state changes (eth_sendRawTransaction) require a client-signed transaction, not an HTTP credential. Dedicated per-project RPC endpoints provisioned through Aurora Cloud may carry their own API key.
kind: authentication
layout: security
method: searched
name: Aurora Authentication
name_suffix: Authentication
oauth_flows: []
overview: Aurora secures its APIs with none across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Aurora
provider_slug: aurora
scheme_count: 1
schemes:
- description: No HTTP authentication on shared public endpoints. Write operations are authorized by an secp256k1-signed transaction submitted via eth_sendRawTransaction.
  in: transaction-signature
  name: none-public-rpc
  sources:
  - https://mainnet.aurora.dev
  - https://testnet.aurora.dev
  type: none
slug: aurora-authentication
source_filename: aurora-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://doc.aurora.dev/\nsummary:\n  types: [none]\n  api_key_in: []\n  oauth2_flows: []\ndescription: >-\n  Aurora's public JSON-RPC endpoints (mainnet.aurora.dev and testnet.aurora.dev) are open and\n  require no API key or bearer token; access control is performed at the protocol layer by\n  cryptographic signing of transactions with an Ethereum-compatible private key (secp256k1),\n  exactly as on Ethereum. Read (eth_call, eth_getBalance, etc.) calls are unauthenticated; state\n  changes (eth_sendRawTransaction) require a client-signed transaction, not an HTTP credential.\n  Dedicated per-project RPC endpoints provisioned through Aurora Cloud may carry their own API key.\nschemes:\n- name: none-public-rpc\n  type: none\n  in: transaction-signature\n  description: >-\n    No HTTP authentication on shared public endpoints. Write operations are authorized by an\n    secp256k1-signed transaction submitted via eth_sendRawTransaction.\n\
  \  sources:\n  - https://mainnet.aurora.dev\n  - https://testnet.aurora.dev\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aurora/refs/heads/main/authentication/aurora-authentication.yml
summary_line: none · 1 scheme
tags:
- Company
- Blockchain
- EVM
- Web3
- JSON-RPC
- NEAR
- Ethereum
- Layer 2
- Smart Contracts
- DeFi
---
