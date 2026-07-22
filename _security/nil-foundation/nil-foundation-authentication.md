---
api_key_in: []
auth_types:
- none
- signature
description: ''
kind: authentication
layout: security
method: searched
name: Nil Foundation Authentication
name_suffix: Authentication
oauth_flows: []
overview: =nil; Foundation secures its APIs with none and signature across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: =nil; Foundation
provider_slug: nil-foundation
scheme_count: 2
schemes:
- description: Read-only JSON-RPC methods require no credentials.
  name: public-read
  operations:
  - GetBlockByNumber
  - GetBalance
  - GetCode
  - Call
  - GasPrice
  - ChainId
  type: none
- description: Write operations are authorized by a signed raw transaction (external message) submitted via SendRawTransaction; signing is handled client-side by niljs WalletV1 / SmartAccountV1 using the account private key.
  name: signed-transaction
  operations:
  - SendRawTransaction
  scheme: ecdsa
  type: signature
slug: nil-foundation-authentication
source_filename: nil-foundation-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://docs.nil.foundation/nil/references/json-rpc-api/\ndocs: https://docs.nil.foundation/nil/reference/client/\nsummary:\n  model: blockchain-signature\n  types: [none, signature]\n  oauth2_flows: []\n  api_key_in: []\nnotes: >-\n  The =nil; JSON-RPC API is a public blockchain RPC endpoint. It uses no API keys, OAuth,\n  or bearer tokens. Read-only methods (via niljs PublicClient) require no authentication.\n  State-changing operations are authorized by ECDSA-signed transactions submitted through\n  SendRawTransaction: the niljs WalletV1 / SmartAccountV1 classes sign external messages\n  with the account's private key. All accounts on =nil; are smart contracts (no EOAs), so\n  authorization is enforced on-chain by the smart account contract rather than by an API\n  credential.\nschemes:\n  - name: public-read\n    type: none\n    description: Read-only JSON-RPC methods require no credentials.\n    operations: [GetBlockByNumber,\
  \ GetBalance, GetCode, Call, GasPrice, ChainId]\n  - name: signed-transaction\n    type: signature\n    scheme: ecdsa\n    description: >-\n      Write operations are authorized by a signed raw transaction (external message)\n      submitted via SendRawTransaction; signing is handled client-side by niljs\n      WalletV1 / SmartAccountV1 using the account private key.\n    operations: [SendRawTransaction]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nil-foundation/refs/heads/main/authentication/nil-foundation-authentication.yml
summary_line: none/signature · 2 schemes
tags:
- Company
- Zk Infrastructure
- Blockchain
- Layer 2
- Ethereum
- Zero Knowledge Proofs
- zkSharding
- JSON-RPC
- Smart Contracts
- Developer Tools
---
