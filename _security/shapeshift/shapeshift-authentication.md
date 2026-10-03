---
anonymous_access: false
api_key_in: []
api_specs:
- filename: shapeshift-account-api-openapi.yml
  format: yaml
  label: Shapeshift Account API
  slug: shapeshift-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shapeshift/refs/heads/main/openapi/shapeshift-account-api-openapi.yml
- filename: shapeshift-fees-api-openapi.yml
  format: yaml
  label: Shapeshift Fees API
  slug: shapeshift-fees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shapeshift/refs/heads/main/openapi/shapeshift-fees-api-openapi.yml
- filename: shapeshift-gas-api-openapi.yml
  format: yaml
  label: Shapeshift Gas API
  slug: shapeshift-gas-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shapeshift/refs/heads/main/openapi/shapeshift-gas-api-openapi.yml
- filename: shapeshift-info-api-openapi.yml
  format: yaml
  label: Shapeshift Info API
  slug: shapeshift-info-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shapeshift/refs/heads/main/openapi/shapeshift-info-api-openapi.yml
- filename: shapeshift-jsonrpc-api-openapi.yml
  format: yaml
  label: Shapeshift Jsonrpc API
  slug: shapeshift-jsonrpc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shapeshift/refs/heads/main/openapi/shapeshift-jsonrpc-api-openapi.yml
- filename: shapeshift-send-api-openapi.yml
  format: yaml
  label: Shapeshift Send API
  slug: shapeshift-send-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shapeshift/refs/heads/main/openapi/shapeshift-send-api-openapi.yml
- filename: shapeshift-token-api-openapi.yml
  format: yaml
  label: Shapeshift Token API
  slug: shapeshift-token-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shapeshift/refs/heads/main/openapi/shapeshift-token-api-openapi.yml
- filename: shapeshift-tx-api-openapi.yml
  format: yaml
  label: Shapeshift Tx API
  slug: shapeshift-tx-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shapeshift/refs/heads/main/openapi/shapeshift-tx-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 0
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
- Wallets
- Trading
- Multi-Chain
---
