---
api_key_in: []
auth_types:
- none
- wallet-signature
description: ''
kind: authentication
layout: security
method: searched
name: Mirror Authentication
name_suffix: Authentication
oauth_flows: []
overview: Mirror secures its APIs with none and wallet-signature across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Mirror
provider_slug: mirror
scheme_count: 2
schemes:
- description: The Mirror API is a public, read-only GraphQL data service exposing protocol state (assets, prices, positions, staking). No API key, OAuth, or bearer token is required or documented; queries are submitted as unauthenticated HTTP POST requests.
  endpoints:
  - https://graph.mirror.finance/graphql
  - https://bombay-graph.mirror.finance/graphql
  name: MirrorAPIPublic
  surface: Mirror API (GraphQL data service)
  type: none
- description: State-changing operations (mint, trade, borrow, stake, governance) are not authenticated at an API layer; they are Terra blockchain transactions built as MsgExecuteContract objects and signed with the caller's wallet key (MnemonicKey via terra.js). Authorization is enforced on-chain by the Mirror CosmWasm contracts, not by an API credential.
  name: TerraWalletSignature
  surface: On-chain protocol (mirror.js / mirrorcli execute)
  type: wallet-signature
slug: mirror-authentication
source_filename: mirror-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://docs.mirror.finance/developer-tools/mirror-api\nsummary:\n  types: [none, wallet-signature]\n  api_key_in: []\n  oauth2_flows: []\nschemes:\n  - name: MirrorAPIPublic\n    type: none\n    surface: Mirror API (GraphQL data service)\n    endpoints:\n      - https://graph.mirror.finance/graphql\n      - https://bombay-graph.mirror.finance/graphql\n    description: >-\n      The Mirror API is a public, read-only GraphQL data service exposing\n      protocol state (assets, prices, positions, staking). No API key, OAuth,\n      or bearer token is required or documented; queries are submitted as\n      unauthenticated HTTP POST requests.\n  - name: TerraWalletSignature\n    type: wallet-signature\n    surface: On-chain protocol (mirror.js / mirrorcli execute)\n    description: >-\n      State-changing operations (mint, trade, borrow, stake, governance) are\n      not authenticated at an API layer; they are Terra blockchain\
  \ transactions\n      built as MsgExecuteContract objects and signed with the caller's wallet\n      key (MnemonicKey via terra.js). Authorization is enforced on-chain by the\n      Mirror CosmWasm contracts, not by an API credential.\nnotes: >-\n  No OAuth scopes surface exists (skip scopes/). Auth is bimodal: unauthenticated\n  public GraphQL reads, and wallet-signed on-chain writes.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mirror/refs/heads/main/authentication/mirror-authentication.yml
summary_line: none/wallet-signature · 2 schemes
tags:
- Company
- DeFi
- Cryptocurrency
- Blockchain
- Synthetic Assets
- GraphQL
- Terra
- Web3
- Financial Services
---
