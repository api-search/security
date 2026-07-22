---
api_key_in: []
auth_types:
- none
- cryptographic-signature
description: 'ThunderCore''s public API surface is unauthenticated. The JSON-RPC endpoints (mainnet and testnet, HTTP and WebSocket) and the BlockScout explorer API require no API key — access is controlled by rate limiting (10K/hr on the public mainnet endpoint) rather than credentials. Transaction submission is authorized cryptographically: transactions are signed with the sender''s ECDSA (secp256k1) private key per the Ethereum transaction model, with EIP-155 chain-id replay protection (chain ID 108 mainnet / 18 testnet). For hosted key management and social-login auth, the docs point to Particle Network''s MPC-based Auth Service as a partner offering.'
kind: authentication
layout: security
method: searched
name: Thundercore Authentication
name_suffix: Authentication
oauth_flows: []
overview: ThunderCore secures its APIs with none and cryptographic-signature across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: ThunderCore
provider_slug: thundercore
scheme_count: 3
schemes:
- description: Public HTTP/WebSocket JSON-RPC endpoints with no API key; rate limited to 10K requests/hour on mainnet.
  endpoints:
  - https://mainnet-rpc.thundercore.com
  - https://testnet-rpc.thundercore.com
  name: public-json-rpc
  type: none
- description: State-changing operations (eth_sendRawTransaction) are authorized by an ECDSA signature over the transaction with the account's private key; EIP-155 chain-id (108/18) provides replay protection. Any Ethereum wallet (MetaMask, Trust Wallet, etc.) works.
  name: transaction-signing
  scheme: secp256k1-ecdsa
  type: cryptographic-signature
- description: Optional MPC (Multi-Party Computation) threshold-signature auth service provided by partner Particle Network for wallet-less/social login in dApps.
  docs: https://docs.developers.thundercore.com/tool/tools/auth-service
  name: partner-auth-service
  type: third-party
slug: thundercore-authentication
source_filename: thundercore-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://docs.developers.thundercore.com/network-details/thundercore-mainnet\ndescription: >-\n  ThunderCore's public API surface is unauthenticated. The JSON-RPC endpoints\n  (mainnet and testnet, HTTP and WebSocket) and the BlockScout explorer API\n  require no API key — access is controlled by rate limiting (10K/hr on the\n  public mainnet endpoint) rather than credentials. Transaction submission is\n  authorized cryptographically: transactions are signed with the sender's\n  ECDSA (secp256k1) private key per the Ethereum transaction model, with\n  EIP-155 chain-id replay protection (chain ID 108 mainnet / 18 testnet).\n  For hosted key management and social-login auth, the docs point to Particle\n  Network's MPC-based Auth Service as a partner offering.\nsummary:\n  types: [none, cryptographic-signature]\n  api_key_in: []\n  oauth2_flows: []\nschemes:\n  - name: public-json-rpc\n    type: none\n    description: >-\n    \
  \  Public HTTP/WebSocket JSON-RPC endpoints with no API key; rate limited to\n      10K requests/hour on mainnet.\n    endpoints:\n      - https://mainnet-rpc.thundercore.com\n      - https://testnet-rpc.thundercore.com\n  - name: transaction-signing\n    type: cryptographic-signature\n    scheme: secp256k1-ecdsa\n    description: >-\n      State-changing operations (eth_sendRawTransaction) are authorized by an\n      ECDSA signature over the transaction with the account's private key;\n      EIP-155 chain-id (108/18) provides replay protection. Any Ethereum wallet\n      (MetaMask, Trust Wallet, etc.) works.\n  - name: partner-auth-service\n    type: third-party\n    description: >-\n      Optional MPC (Multi-Party Computation) threshold-signature auth service\n      provided by partner Particle Network for wallet-less/social login in\n      dApps.\n    docs: https://docs.developers.thundercore.com/tool/tools/auth-service\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/thundercore/refs/heads/main/authentication/thundercore-authentication.yml
summary_line: none/cryptographic-signature · 3 schemes
tags:
- Company
- Crypto
- Blockchain
- EVM
- JSON-RPC
- Web3
- Layer 1
---
