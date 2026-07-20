---
api_key_in:
- header
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Hashflow Authentication
name_suffix: Authentication
oauth_flows: []
overview: Hashflow secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Hashflow
provider_slug: hashflow
scheme_count: 1
schemes:
- description: Provider-issued credential key sent on every Taker API v3 request.
  in: header
  name: ApiKeyAuth
  parameter_name: Authorization
  sources:
  - docs.hashflow.com/hashflow/taker/getting-started-api-v3
  type: apiKey
slug: hashflow-authentication
source_filename: hashflow-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://docs.hashflow.com/hashflow/taker/getting-started-api-v3\ndocs: https://docs.hashflow.com/hashflow/taker/getting-started-api-v3\nsummary:\n  types: [apiKey]\n  api_key_in: [header]\n  oauth2_flows: []\n  notes: >-\n    The Hashflow Taker API v3 authenticates with a provider-issued credential\n    key passed in the HTTP Authorization header. Access is granted per source\n    identifier; aggregators supply their own `source`, while single-wallet\n    integrators use `source: \"api\"` plus a `wallet` parameter. Trade settlement\n    on-chain is authorized separately by EIP-712 market-maker signatures returned\n    on each quote (verified by the HashflowRouter contract), not by the API key.\nschemes:\n  - name: ApiKeyAuth\n    type: apiKey\n    in: header\n    parameter_name: Authorization\n    description: Provider-issued credential key sent on every Taker API v3 request.\n    sources: [docs.hashflow.com/hashflow/taker/getting-started-api-v3]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hashflow/refs/heads/main/authentication/hashflow-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Defi
- DEX
- RFQ
- Trading
- Crypto
- Market Making
- Cross-Chain
- Blockchain
- Web3
---
