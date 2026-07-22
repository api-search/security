---
api_key_in: []
auth_types:
- none
description: ''
kind: authentication
layout: security
method: searched
name: Nervos Authentication
name_suffix: Authentication
oauth_flows: []
overview: Nervos secures its APIs with none across 0 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Nervos
provider_slug: nervos
scheme_count: 0
schemes: []
slug: nervos-authentication
source_filename: nervos-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://docs.nervos.org/docs/getting-started/rpcs\nsummary:\n  types: [none]\n  note: >-\n    The CKB JSON-RPC API is an unauthenticated, public JSON-RPC 2.0 interface. Public\n    RPC endpoints (mainnet.ckb.dev, testnet.ckb.dev, rpc.ankr.com/nervos) require no\n    API key, token, or OAuth. Security is provided at the protocol layer: state changes\n    are authorized by CKB lock scripts and signatures inside transactions (witnesses),\n    not by an API credential. Operators running their own public RPC node are advised\n    to restrict method exposure and place the node behind a reverse proxy / rate limiter.\nschemes: []\ntransaction_authorization:\n  model: script-based\n  detail: >-\n    Spending a Cell requires satisfying its lock script (e.g. Secp256k1/blake160,\n    Omnilock, Anyone-Can-Pay). Signatures are supplied off-chain in the transaction\n    witness and verified on-chain by CKB-VM. See docs how-to \"How to Sign\
  \ a Transaction\".\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nervos/refs/heads/main/authentication/nervos-authentication.yml
summary_line: none · 0 schemes
tags:
- Company
- Crypto Web3
- Blockchain
- Layer 1
- JSON-RPC
- Smart Contracts
- Web3 Infrastructure
- Developer Tools
---
