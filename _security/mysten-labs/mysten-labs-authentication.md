---
api_key_in: []
auth_types:
- none
description: ''
kind: authentication
layout: security
method: searched
name: Mysten Labs Authentication
name_suffix: Authentication
oauth_flows: []
overview: Mysten Labs secures its APIs with none across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Mysten Labs
provider_slug: mysten-labs
scheme_count: 1
schemes:
- description: No transport-level authentication on public full-node endpoints. Rate limits and access controls are applied by the specific RPC provider hosting the node.
  name: none
  sources:
  - openrpc/mysten-labs-sui-jsonrpc-openrpc.json
  type: none
slug: mysten-labs-authentication
source_filename: mysten-labs-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://docs.sui.io/references/sui-api\nsummary:\n  types: [none]\n  api_key_in: []\n  oauth2_flows: []\n  note: >-\n    Public Sui full-node RPC endpoints (JSON-RPC, GraphQL RPC, gRPC) are open and\n    require no API key or bearer token — anyone can read chain state and submit\n    signed transactions against public endpoints such as\n    fullnode.mainnet.sui.io:443 and graphql.mainnet.sui.io/graphql. Authorization\n    is performed cryptographically at the transaction layer, not at the API layer.\nschemes:\n- name: none\n  type: none\n  description: >-\n    No transport-level authentication on public full-node endpoints. Rate limits\n    and access controls are applied by the specific RPC provider hosting the node.\n  sources: [openrpc/mysten-labs-sui-jsonrpc-openrpc.json]\ntransaction_layer_auth:\n  description: >-\n    Requests that mutate state (executeTransactionBlock) carry a client-side\n    cryptographic signature\
  \ over the transaction bytes. Sui supports Ed25519,\n    ECDSA Secp256k1, ECDSA Secp256r1, multisig, and zkLogin signature schemes.\n  schemes: [Ed25519, Secp256k1, Secp256r1, multisig, zkLogin]\n  zklogin:\n    description: OAuth/OIDC-based (Google, Facebook, Twitch, Apple, etc.) zero-knowledge login that derives a Sui address from a JWT without exposing identity on-chain.\n    docs: https://docs.sui.io/concepts/cryptography/zklogin\n    sdk: \"@mysten/enoki\"\n  proto: grpc/sui/rpc/v2/signature_verification_service.proto\nnotes: >-\n  Managed RPC providers (e.g. via the RPC providers list) may layer their own API\n  keys on top of the public endpoints, but the Mysten-published node software\n  exposes unauthenticated read/execute RPC. This is not derivable from the OpenRPC\n  spec (no securitySchemes concept in OpenRPC); documented from the Sui docs.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mysten-labs/refs/heads/main/authentication/mysten-labs-authentication.yml
summary_line: none · 1 scheme
tags:
- Company
- Blockchain
- Web3
- Sui
- Move
- JSON-RPC
- GraphQL
- gRPC
- SDK
- Smart Contracts
- Decentralized Storage
- Cryptocurrency
---
