---
api_key_in: []
auth_types:
- none
description: ''
kind: authentication
layout: security
method: searched
name: Sorella Labs Authentication
name_suffix: Authentication
oauth_flows: []
overview: Sorella Labs secures its APIs with none across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Sorella Labs
provider_slug: sorella-labs
scheme_count: 1
schemes:
- endpoints:
  - https://mainnet.node-lb.angstrom.xyz
  - wss://mainnet.node-lb.angstrom.xyz
  - https://mainnet.node.data.angstrom.xyz
  name: public-json-rpc
  sources:
  - docs.angstrom.xyz/api/intro
  transport:
  - https
  - websocket
  type: none
slug: sorella-labs-authentication
source_filename: sorella-labs-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://docs.angstrom.xyz/api/intro\nsummary:\n  types: [none]\n  notes: >-\n    The Angstrom API is a public, decentralized JSON-RPC surface. The\n    documentation (https://docs.angstrom.xyz/api/intro) documents open\n    HTTPS/WebSocket node endpoints and a Data API with no API-key, OAuth, or\n    bearer-token requirement described. Authorization of state-changing actions\n    is enforced on-chain (transactions are signed with the caller's Ethereum\n    key and validated by the Angstrom Uniswap V4 hook), not by an API\n    credential.\nschemes:\n- name: public-json-rpc\n  type: none\n  transport: [https, websocket]\n  endpoints:\n  - https://mainnet.node-lb.angstrom.xyz\n  - wss://mainnet.node-lb.angstrom.xyz\n  - https://mainnet.node.data.angstrom.xyz\n  sources: [docs.angstrom.xyz/api/intro]\nonchain_authorization: >-\n  State-changing operations are authorized by Ethereum transaction signatures\n  and validated by the\
  \ Angstrom smart contracts (Uniswap V4 hook), not by an\n  API-layer credential.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sorella-labs/refs/heads/main/authentication/sorella-labs-authentication.yml
summary_line: none · 1 scheme
tags:
- Company
- Crypto Infrastructure
- DeFi
- Decentralized Exchange
- MEV
- Ethereum
- Uniswap V4
- JSON-RPC
- Blockchain
- Trading
---
