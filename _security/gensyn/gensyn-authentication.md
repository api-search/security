---
api_key_in:
- environment
auth_types:
- apiKey
- wallet-signing
description: ''
kind: authentication
layout: security
method: searched
name: Gensyn Authentication
name_suffix: Authentication
oauth_flows: []
overview: Gensyn secures its APIs with apiKey and wallet-signing across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Gensyn
provider_slug: gensyn
scheme_count: 2
schemes:
- description: REST API access key required for authenticated Delphi REST endpoints (market and position queries). The public health endpoint requires no auth.
  in: environment
  issued_at:
    mainnet: https://api-access.delphi.fyi/
    testnet: https://delphi-api-access.gensyn.ai/
  name: DelphiApiAccessKey
  type: apiKey
  variable: DELPHI_API_ACCESS_KEY
- description: On-chain transactions (buy/sell shares, redeem, liquidate, ERC-20 approvals) are signed by a wallet. Two options are supported.
  methods:
  - private-key
  - coinbase-cdp-server-wallet
  name: WalletSigning
  type: wallet-signing
slug: gensyn-authentication
source_filename: gensyn-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://github.com/gensyn-ai/gensyn-delphi-sdk#readme\ndocs: https://github.com/gensyn-ai/gensyn-delphi-sdk#readme\nsummary:\n  types: [apiKey, wallet-signing]\n  api_key_in: [environment]\n  notes: >-\n    The Delphi API combines a REST API-access key with on-chain wallet signing.\n    No OpenAPI securitySchemes are published, so this profile is captured from the\n    published SDK documentation rather than derived from a spec.\nschemes:\n- name: DelphiApiAccessKey\n  type: apiKey\n  in: environment\n  variable: DELPHI_API_ACCESS_KEY\n  description: >-\n    REST API access key required for authenticated Delphi REST endpoints (market\n    and position queries). The public health endpoint requires no auth.\n  issued_at:\n    testnet: https://delphi-api-access.gensyn.ai/\n    mainnet: https://api-access.delphi.fyi/\n- name: WalletSigning\n  type: wallet-signing\n  description: >-\n    On-chain transactions (buy/sell shares, redeem,\
  \ liquidate, ERC-20 approvals)\n    are signed by a wallet. Two options are supported.\n  methods:\n  - private-key\n  - coinbase-cdp-server-wallet\nenvironments:\n  testnet:\n    base_url: https://delphi-api.gensyn.ai/\n    rpc: https://gensyn-testnet.g.alchemy.com/public\n  mainnet:\n    base_url: https://api.delphi.fyi/\n    rpc: https://gensyn-mainnet.g.alchemy.com/public\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gensyn/refs/heads/main/authentication/gensyn-authentication.yml
summary_line: apiKey/wallet-signing · 2 schemes
tags:
- Company
- Ai
- Machine Learning
- Decentralized Compute
- Blockchain
- Prediction Markets
- Agents
- Web3
---
