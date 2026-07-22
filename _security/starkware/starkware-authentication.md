---
api_key_in:
- header
auth_types:
- none
- api-key-at-provider
description: ''
kind: authentication
layout: security
method: searched
name: Starkware Authentication
name_suffix: Authentication
oauth_flows: []
overview: Starkware secures its APIs with none and api-key-at-provider across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Starkware
provider_slug: starkware
scheme_count: 3
schemes:
- description: Direct JSON-RPC 2.0 to a Starknet full node. No API-level authentication in the spec; access control is deployment-specific.
  name: node-endpoint
  scheme: json-rpc
  sources:
  - openrpc/starkware-starknet_api_openrpc.json
  type: none
- description: Commercial RPC providers front the Starknet JSON-RPC methods with an issued API key (URL path token or header). Not part of the StarkWare spec; documented per provider.
  in: header
  name: provider-api-key
  parameter_name: x-api-key
  sources:
  - docs
  type: apiKey
- description: Write methods (addInvoke/addDeclare/addDeployAccount) require a transaction signed by the Starknet account contract; validation and nonce replay protection happen on-chain, not via API auth.
  name: account-signature
  scheme: ecdsa/account-abstraction
  sources:
  - openrpc/starkware-starknet_write_api.json
  type: protocol
slug: starkware-authentication
source_filename: starkware-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://docs.starknet.io/ , openrpc/starkware-starknet_api_openrpc.json\nsummary:\n  types: [none, api-key-at-provider]\n  api_key_in: [header]\n  oauth2_flows: []\n  notes: >-\n    The Starknet Node JSON-RPC API defines no securitySchemes in its OpenRPC\n    spec: methods are served by full nodes (Juno, Pathfinder, etc.). Public and\n    self-hosted nodes are typically unauthenticated; commercial RPC providers\n    (Infura, Alchemy, Nethermind, Blast, etc.) gate the same JSON-RPC surface\n    behind a provider-issued API key embedded in the endpoint URL or an\n    x-api-key header. Write and account operations are authorized cryptographically\n    at the protocol layer: transactions are signed with the account's key and\n    replay-protected by an account nonce (Starknet native account abstraction),\n    not by an API credential.\nschemes:\n- name: node-endpoint\n  type: none\n  scheme: json-rpc\n  description: >-\n    Direct\
  \ JSON-RPC 2.0 to a Starknet full node. No API-level authentication in\n    the spec; access control is deployment-specific.\n  sources: [openrpc/starkware-starknet_api_openrpc.json]\n- name: provider-api-key\n  type: apiKey\n  in: header\n  parameter_name: x-api-key\n  description: >-\n    Commercial RPC providers front the Starknet JSON-RPC methods with an issued\n    API key (URL path token or header). Not part of the StarkWare spec; documented\n    per provider.\n  sources: [docs]\n- name: account-signature\n  type: protocol\n  scheme: ecdsa/account-abstraction\n  description: >-\n    Write methods (addInvoke/addDeclare/addDeployAccount) require a transaction\n    signed by the Starknet account contract; validation and nonce replay\n    protection happen on-chain, not via API auth.\n  sources: [openrpc/starkware-starknet_write_api.json]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/starkware/refs/heads/main/authentication/starkware-authentication.yml
summary_line: none/api-key-at-provider · 3 schemes
tags:
- Company
- Blockchain
- Ethereum
- Layer 2
- ZK-Rollup
- Zero-Knowledge Proofs
- JSON-RPC
- Cryptography
- Cairo
- Web3
- Scaling
- Starknet
---
