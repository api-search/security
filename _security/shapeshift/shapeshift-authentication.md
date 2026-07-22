---
api_key_in: []
api_specs:
- filename: shapeshift-ethereum-openapi.json
  format: json
  label: ShapeShift Unchained — Ethereum (EVM) API
  slug: shapeshift-unchained-ethereum-evm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shapeshift/refs/heads/main/openapi/shapeshift-ethereum-openapi.json
- filename: shapeshift-bitcoin-openapi.json
  format: json
  label: ShapeShift Unchained — Bitcoin (UTXO) API
  slug: shapeshift-unchained-bitcoin-utxo-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shapeshift/refs/heads/main/openapi/shapeshift-bitcoin-openapi.json
- filename: shapeshift-solana-openapi.json
  format: json
  label: ShapeShift Unchained — Solana API
  slug: shapeshift-unchained-solana-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shapeshift/refs/heads/main/openapi/shapeshift-solana-openapi.json
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Shapeshift Authentication
name_suffix: Authentication
oauth_flows: []
overview: Shapeshift declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Shapeshift
provider_slug: shapeshift
scheme_count: 0
schemes: []
slug: shapeshift-authentication
source_filename: shapeshift-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: openapi/shapeshift-ethereum-openapi.json, openapi/shapeshift-bitcoin-openapi.json, openapi/shapeshift-solana-openapi.json\nsummary:\n  types: []\n  model: public\n  api_key_required: false\n  oauth2_flows: []\nschemes: []\nnotes: >-\n  The ShapeShift unchained public blockchain APIs declare NO securitySchemes in\n  their OpenAPI documents and require no API key, token, or OAuth to read\n  account/transaction data or to broadcast a signed transaction. Access is open\n  over HTTPS on the per-chain api.<chain>.shapeshift.com hosts. Write safety is\n  enforced by the blockchain itself — the /api/v1/send endpoint only accepts\n  transactions already signed client-side, so no server-side credential governs\n  it. (Self-hosted unchained deployments may set upstream node provider API keys\n  via env, but the hosted ShapeShift API surface is unauthenticated.)\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/shapeshift/refs/heads/main/authentication/shapeshift-authentication.yml
summary_line: 0 schemes
tags:
- Company
- Cryptocurrency
- Blockchain
- Bitcoin
- Ethereum
- Web3
- DeFi
- Wallet
- Trading
- Multichain
- API
---
