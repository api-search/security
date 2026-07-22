---
api_key_in: []
auth_types:
- signature
description: ''
kind: authentication
layout: security
method: searched
name: Hamsa Authentication
name_suffix: Authentication
oauth_flows: []
overview: Hamsa secures its APIs with signature across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Hamsa
provider_slug: hamsa
scheme_count: 1
schemes:
- description: Sign a message with the account private key (e.g. deployer.signMessage) and pass the signer address and signature. Used to gate privacy-sensitive (protected) JSON-RPC methods.
  name: EthereumMessageSignature
  scheme: ethereum-eip191
  sources:
  - https://developer.hamsa.com/reference/api-documentation
  type: signature
slug: hamsa-authentication
source_filename: hamsa-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://developer.hamsa.com/reference/api-documentation\ndocs: https://developer.hamsa.com/reference/api-documentation\nsummary:\n  types:\n  - signature\n  scheme: ethereum-message-signature\n  note: >-\n    The Hamsa Unified Confidential Ledger (UCL) / Hamsa Privacy JSON-RPC API does\n    not use API keys or OAuth. Callers authenticate protected methods by signing\n    an Ethereum message with their private key and supplying their address plus\n    the resulting signature (EIP-191 personal_sign style). Authorization is\n    role-based access control (RBAC) enforced on-chain.\nschemes:\n- name: EthereumMessageSignature\n  type: signature\n  scheme: ethereum-eip191\n  description: >-\n    Sign a message with the account private key (e.g. deployer.signMessage) and\n    pass the signer address and signature. Used to gate privacy-sensitive\n    (protected) JSON-RPC methods.\n  sources:\n  - https://developer.hamsa.com/reference/api-documentation\n\
  roles:\n- id: 0\n  name: normal-user\n  description: Can query own balances and transactions only.\n- id: 1\n  name: administrator\n  description: Can query all balances and transactions.\nprotected_methods:\n- eth_safeGetBalance\n- eth_getTransactionHistory\nunprotected_methods:\n- eth_estimateGas\n- eth_getNonce\n- eth_getBalance\n- eth_getTransactionByHash\n- eth_checkTransactionBundle\n- eth_blockNumber\n- eth_call\n- eth_chainId\n- eth_gasPrice\n- eth_getBlockByHash\n- eth_getBlockByNumber\n- eth_getBlockTransactionCountByHash\n- eth_getBlockTransactionCountByNumber\n- eth_getTransactionReceipt\n- eth_sendRawTransaction\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hamsa/refs/heads/main/authentication/hamsa-authentication.yml
summary_line: signature · 1 scheme
tags:
- Company
- Financial Services
- Blockchain
- Payments
- Tokenization
- Privacy
- Zero-Knowledge Proofs
- CBDC
- Settlement
- DeFi
- EVM
- JSON-RPC
---
