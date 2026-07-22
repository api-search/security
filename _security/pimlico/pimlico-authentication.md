---
api_key_in:
- query
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Pimlico Authentication
name_suffix: Authentication
oauth_flows: []
overview: Pimlico secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Pimlico
provider_slug: pimlico
scheme_count: 1
schemes:
- dashboard: https://dashboard.pimlico.io
  description: All Pimlico bundler, paymaster, and platform API calls are authenticated with an API key passed as the `apikey` query parameter on the per-chain JSON-RPC endpoint, e.g. https://api.pimlico.io/v2/{chainId or chain-name}/rpc?apikey=YOUR_API_KEY.
  docs: https://docs.pimlico.io/guides/how-to/platform/create-api-key
  in: query
  name: apiKey
  parameter: apikey
  type: apiKey
slug: pimlico-authentication
source_filename: pimlico-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://docs.pimlico.io + https://www.pimlico.io/.well-known/security.txt\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\n  oauth2_flows: []\nschemes:\n- name: apiKey\n  type: apiKey\n  in: query\n  parameter: apikey\n  description: >-\n    All Pimlico bundler, paymaster, and platform API calls are authenticated\n    with an API key passed as the `apikey` query parameter on the per-chain\n    JSON-RPC endpoint, e.g.\n    https://api.pimlico.io/v2/{chainId or chain-name}/rpc?apikey=YOUR_API_KEY.\n  dashboard: https://dashboard.pimlico.io\n  docs: https://docs.pimlico.io/guides/how-to/platform/create-api-key\nnotes:\n  - >-\n    API keys are created and scoped (chain / IP / domain allowlists,\n    sponsorship policies) in the Pimlico dashboard.\n  - >-\n    End-user authentication and account/user management for the Pimlico\n    dashboard are handled by Clerk (per the published security.txt).\n  - >-\n    The endpoint\
  \ also accepts a legacy /v1/ path in addition to the current\n    /v2/ path; the chain segment accepts either a numeric chain id or a chain\n    name (e.g. sepolia).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pimlico/refs/heads/main/authentication/pimlico-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Account Abstraction
- ERC-4337
- Blockchain
- Ethereum
- Web3
- Paymaster
- Bundler
- Smart Accounts
- Gas Sponsorship
- Wallets
- Infrastructure
---
