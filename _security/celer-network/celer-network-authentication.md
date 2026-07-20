---
api_key_in: []
auth_types:
- none
- signature
description: ''
kind: authentication
layout: security
method: searched
name: Celer Network Authentication
name_suffix: Authentication
oauth_flows: []
overview: Celer Network secures its APIs with none and signature across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Celer Network
provider_slug: celer-network
scheme_count: 2
schemes:
- applies_to: read/query operations
  name: public
  sources:
  - grpc/celer-network-gateway.proto
  type: none
- applies_to: WithdrawLiquidity
  name: client-signature
  scheme: wallet-signed request (EIP-712 style)
  sources:
  - grpc/celer-network-gateway.proto
  type: signature
slug: celer-network-authentication
source_filename: celer-network-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://cbridge-docs.celer.network/developer/cbridge-sdk + grpc/celer-network-gateway.proto\ndocs: https://cbridge-docs.celer.network/developer/cbridge-sdk\nsummary:\n  types: [none, signature]\n  api_key_in: []\n  oauth2_flows: []\n  note: >-\n    The cBridge gateway API carries no API-key, OAuth, or bearer authentication.\n    Read/query operations (getTransferConfigs, getTokenInfo, estimateAmt,\n    getTransferStatus, transferHistory, estimateWithdrawAmt) are public. The\n    only state-changing gateway call, withdrawLiquidity, is authorized by a\n    client-side cryptographic signature over the serialized WithdrawReq\n    (withdraw_req + sig fields) produced by the user's wallet — the SGN validators\n    verify the signature on chain, so there is no server-issued API credential.\nschemes:\n  - name: public\n    type: none\n    applies_to: read/query operations\n    sources: [grpc/celer-network-gateway.proto]\n  - name:\
  \ client-signature\n    type: signature\n    scheme: wallet-signed request (EIP-712 style)\n    applies_to: WithdrawLiquidity\n    sources: [grpc/celer-network-gateway.proto]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/celer-network/refs/heads/main/authentication/celer-network-authentication.yml
summary_line: none/signature · 2 schemes
tags:
- Company
- Crypto
- Blockchain
- Interoperability
- Cross-Chain
- Bridge
- DeFi
- Web3
---
