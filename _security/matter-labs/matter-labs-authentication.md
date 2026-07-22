---
api_key_in: []
auth_types:
- none
description: ''
kind: authentication
layout: security
method: searched
name: Matter Labs Authentication
name_suffix: Authentication
oauth_flows: []
overview: Matter Labs secures its APIs with none across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Matter Labs
provider_slug: matter-labs
scheme_count: 1
schemes:
- description: The ZKsync Era JSON-RPC endpoints (mainnet.era.zksync.dev, sepolia.era.zksync.dev) are public and require no API key, token, or OAuth. Access control is economic (transactions must be signed with an Ethereum ECDSA / EIP-712 key and pay gas), not an API credential. Higher-throughput / dedicated access is offered by third-party RPC providers (e.g. Alchemy, QuickNode, Chainstack) under their own API keys, not by Matter Labs.
  name: public-rpc
  sources:
  - docs.zksync.io/zksync-protocol/api
  type: none
slug: matter-labs-authentication
source_filename: matter-labs-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://docs.zksync.io/zksync-protocol/api\nsummary:\n  types: [none]\n  api_key_in: []\n  oauth2_flows: []\nschemes:\n  - name: public-rpc\n    type: none\n    description: >-\n      The ZKsync Era JSON-RPC endpoints (mainnet.era.zksync.dev, sepolia.era.zksync.dev)\n      are public and require no API key, token, or OAuth. Access control is economic\n      (transactions must be signed with an Ethereum ECDSA / EIP-712 key and pay gas), not\n      an API credential. Higher-throughput / dedicated access is offered by third-party RPC\n      providers (e.g. Alchemy, QuickNode, Chainstack) under their own API keys, not by\n      Matter Labs.\n    sources: [docs.zksync.io/zksync-protocol/api]\ntransaction_signing:\n  scheme: ECDSA / EIP-712\n  note: >-\n    Write operations (eth_sendRawTransaction, zks_sendRawTransactionWithDetailedOutput)\n    require a transaction signed by the sender's Ethereum private key; ZKsync also supports\n\
  \    native account abstraction (custom signature schemes) and paymasters.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/matter-labs/refs/heads/main/authentication/matter-labs-authentication.yml
summary_line: none · 1 scheme
tags:
- Company
- Blockchain
- Ethereum
- Layer 2
- Zero-Knowledge Proofs
- Rollup
- JSON-RPC
- Web3
- Cryptography
- Scaling
---
