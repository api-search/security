---
api_key_in: []
api_specs:
- filename: derivadex-exchange-openapi.yml
  format: yaml
  label: DerivaDEX Exchange & Stats API
  slug: derivadex-exchange-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/derivadex/refs/heads/main/openapi/derivadex-exchange-openapi.yml
auth_types:
- none
- wallet-signature
description: ''
kind: authentication
layout: security
method: searched
name: Derivadex Authentication
name_suffix: Authentication
oauth_flows: []
overview: DerivaDEX secures its APIs with none and wallet-signature across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: DerivaDEX
provider_slug: derivadex
scheme_count: 2
schemes:
- applies_to: openapi/derivadex-exchange-openapi.yml
  description: Public REST market-data and stats endpoints require no credentials.
  name: public
  type: none
- description: Authenticated/trading operations are authorized by signing EIP-712 typed-data with the trader's Ethereum wallet; there is no server-issued API key or OAuth token. Not modeled in the public OpenAPI (public surface only).
  docs: https://docs.derivadex.io/technical-and-developer/api
  name: walletSignature
  scheme: eip712
  type: wallet-signature
slug: derivadex-authentication
source_filename: derivadex-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://exchange.derivadex.com/api-docs\ndocs: https://docs.derivadex.io/technical-and-developer/api\nsummary:\n  types: [none, wallet-signature]\n  api_key_in: []\n  oauth2_flows: []\n  notes: >-\n    The documented public REST endpoints require no authentication (\"This\n    operation does not require authentication\"). DerivaDEX additionally exposes\n    an Authenticated REST API and a Realtime API; as a non-custodial on-chain\n    exchange, authenticated/trading actions are authorized by Ethereum wallet\n    signatures (EIP-712 typed-data) rather than API keys or OAuth. The public\n    market-data and stats surface captured in openapi/ is fully unauthenticated.\nschemes:\n  - name: public\n    type: none\n    description: Public REST market-data and stats endpoints require no credentials.\n    applies_to: openapi/derivadex-exchange-openapi.yml\n  - name: walletSignature\n    type: wallet-signature\n    scheme: eip712\n\
  \    description: >-\n      Authenticated/trading operations are authorized by signing EIP-712\n      typed-data with the trader's Ethereum wallet; there is no server-issued\n      API key or OAuth token. Not modeled in the public OpenAPI (public surface\n      only).\n    docs: https://docs.derivadex.io/technical-and-developer/api\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/derivadex/refs/heads/main/authentication/derivadex-authentication.yml
summary_line: none/wallet-signature · 2 schemes
tags:
- Company
- Defi Derivatives
- Cryptocurrency
- Derivatives
- Perpetual Swaps
- Decentralized Exchange
- Trading
- Blockchain
- Market Data
- DeFi
---
