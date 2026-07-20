---
api_key_in:
- header
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Blockvision Authentication
name_suffix: Authentication
oauth_flows: []
overview: BlockVision secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: BlockVision
provider_slug: blockvision
scheme_count: 1
schemes:
- description: All BlockVision Indexing / Data API requests require an API key issued from the BlockVision dashboard (https://dashboard.blockvision.org/app), passed in the x-api-key request header. A request without a key returns HTTP 403 with the JSON envelope {"code":-32002,"message":"apikey must"} (confirmed live 2026-07-18).
  evidence:
  - observed: HTTP 403 {"code":-32002,"message":"apikey must"}
    source: live probe https://api.blockvision.org/v2/sui/account/coins
  in: header
  name: ApiKeyAuth
  parameter_name: x-api-key
  type: apiKey
slug: blockvision-authentication
source_filename: blockvision-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://docs.blockvision.org/reference/ ; confirmed via live probe of api.blockvision.org\nsummary:\n  types: [apiKey]\n  api_key_in: [header]\n  oauth2_flows: []\nschemes:\n  - name: ApiKeyAuth\n    type: apiKey\n    in: header\n    parameter_name: x-api-key\n    description: >-\n      All BlockVision Indexing / Data API requests require an API key issued from the\n      BlockVision dashboard (https://dashboard.blockvision.org/app), passed in the\n      x-api-key request header. A request without a key returns HTTP 403 with the JSON\n      envelope {\"code\":-32002,\"message\":\"apikey must\"} (confirmed live 2026-07-18).\n    evidence:\n      - source: live probe https://api.blockvision.org/v2/sui/account/coins\n        observed: 'HTTP 403 {\"code\":-32002,\"message\":\"apikey must\"}'\nnotes: >-\n  Key issuance and quota are managed per-project in the dashboard; usage is metered in\n  Compute Units (see conventions/ and\
  \ lifecycle/). No OAuth2/OIDC surface is documented.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/blockvision/refs/heads/main/authentication/blockvision-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Blockchain
- Web3
- Data Infrastructure
- Sui
- Monad
- NFT
- DeFi
- RPC Node
- Indexing
- Cryptocurrency
- Smart Contracts
---
