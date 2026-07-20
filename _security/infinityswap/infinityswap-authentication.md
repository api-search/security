---
api_key_in: []
auth_types:
- none
description: ''
kind: authentication
layout: security
method: searched
name: Infinityswap Authentication
name_suffix: Authentication
oauth_flows: []
overview: InfinitySwap secures its APIs with none across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: InfinitySwap
provider_slug: infinityswap
scheme_count: 1
schemes:
- description: Public EVM JSON-RPC endpoint; no API-level authentication. Requests are unauthenticated; on-chain writes are authorized by the transaction signer's private key (secp256k1 / EIP-155), submitted via eth_sendRawTransaction.
  name: publicRpc
  sources:
  - 'live probe: https://mainnet.bitfinity.network'
  type: none
slug: infinityswap-authentication
source_filename: infinityswap-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://docs.bitfinity.network/getting-started\nnotes: >-\n  The Bitfinity EVM JSON-RPC endpoint is a public, keyless blockchain RPC. There\n  is no API key, OAuth, or bearer credential — any client (MetaMask, ethers.js,\n  Hardhat) connects directly by network URL and chain ID. Authorization for state\n  changes is enforced at the protocol layer by ECDSA transaction signatures\n  (the sender's private key), not by an API access credential. Confirmed by live\n  probing: read/query methods succeed with no auth header.\nsummary:\n  types: [none]\n  api_key_in: []\n  oauth2_flows: []\n  protocol_auth: ecdsa-transaction-signature\nschemes:\n- name: publicRpc\n  type: none\n  description: >-\n    Public EVM JSON-RPC endpoint; no API-level authentication. Requests are\n    unauthenticated; on-chain writes are authorized by the transaction signer's\n    private key (secp256k1 / EIP-155), submitted via eth_sendRawTransaction.\n  sources:\
  \ [\"live probe: https://mainnet.bitfinity.network\"]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/infinityswap/refs/heads/main/authentication/infinityswap-authentication.yml
summary_line: none · 1 scheme
tags:
- Company
- Defi
- Blockchain
- Ethereum
- EVM
- Bitcoin
- Layer 2
- Internet Computer
- Smart Contracts
- JSON-RPC
- Web3
- Cryptocurrency
---
