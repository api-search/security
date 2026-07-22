---
api_key_in: []
auth_types:
- none
- jwt
- wallet-signature
description: ''
kind: authentication
layout: security
method: searched
name: Morph Authentication
name_suffix: Authentication
oauth_flows: []
overview: Morph secures its APIs with none, jwt, and wallet-signature across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Morph
provider_slug: morph
scheme_count: 4
schemes:
- description: Ethereum-compatible JSON-RPC, no API key required.
  endpoint: https://rpc.morph.network/
  name: json-rpc-public
  type: none
- description: Blockscout REST API, public reads, no API key required.
  endpoint: https://explorer-api.morph.network/api/v2
  name: explorer-blockscout
  type: none
- description: Write operations (transfers, swaps, agent identity, x402 payments) are authorized by client-side wallet signatures over the private key; no server-issued token.
  name: wallet-signature
  schemes:
  - secp256k1-tx
  - EIP-712
  - EIP-191
  - EIP-3009
  type: signature
- description: Cross-chain bridge order management requires a JWT via bridge-login.
  endpoint: https://api.bulbaswap.io
  name: bridge-jwt
  scheme: bearer
  type: http
slug: morph-authentication
source_filename: morph-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://github.com/morph-l2/morph-skill (Data Sources table) + https://docs.morph.network/\nsummary:\n  types: [none, jwt, wallet-signature]\n  notes: >-\n    Morph is an EVM Layer-2. Public JSON-RPC (rpc.morph.network) and the\n    Blockscout explorer API (explorer-api.morph.network/api/v2) require NO\n    authentication for reads. State-changing operations are authenticated by\n    Ethereum wallet signatures (private-key / EIP-712 / EIP-191 / EIP-3009), not\n    an API credential. The BulbaSwap DEX aggregator bridge order-management\n    surface requires a JWT (obtained via bridge-login).\nschemes:\n- name: json-rpc-public\n  type: none\n  endpoint: https://rpc.morph.network/\n  description: Ethereum-compatible JSON-RPC, no API key required.\n- name: explorer-blockscout\n  type: none\n  endpoint: https://explorer-api.morph.network/api/v2\n  description: Blockscout REST API, public reads, no API key required.\n- name: wallet-signature\n\
  \  type: signature\n  schemes: [secp256k1-tx, EIP-712, EIP-191, EIP-3009]\n  description: >-\n    Write operations (transfers, swaps, agent identity, x402 payments) are\n    authorized by client-side wallet signatures over the private key; no\n    server-issued token.\n- name: bridge-jwt\n  type: http\n  scheme: bearer\n  endpoint: https://api.bulbaswap.io\n  description: Cross-chain bridge order management requires a JWT via bridge-login.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/morph/refs/heads/main/authentication/morph-authentication.yml
summary_line: none/jwt/wallet-signature · 4 schemes
tags:
- Company
- Crypto
- Blockchain
- Layer 2
- Ethereum
- zkEVM
- Web3
- Developer Tools
---
