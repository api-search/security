---
api_key_in: []
api_specs:
- filename: gte-openapi-original.yml
  format: yaml
  label: GTE API
  slug: gte-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gte/refs/heads/main/openapi/gte-openapi-original.yml
auth_types:
- signature
description: ''
kind: authentication
layout: security
method: searched
name: Gte Authentication
name_suffix: Authentication
oauth_flows: []
overview: GTE secures its APIs with signature across 0 declared security schemes, as derived from its OpenAPI definitions.
provider_name: GTE
provider_slug: gte
scheme_count: 0
schemes: []
slug: gte-authentication
source_filename: gte-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://docs.gte.xyz/openapi.yaml\ndocs: https://docs.gte.xyz\nsummary:\n  types: [signature]\n  api_key_in: []\n  oauth2_flows: []\nmodel: evm-wallet-signature\nnotes: >-\n  GTE is a non-custodial decentralized exchange on MegaETH. The OpenAPI declares no\n  securitySchemes (apiKey / http / oauth2 / openIdConnect / mutualTLS): all read\n  endpoints (tokens, markets, candles, trades, book, user portfolio/orders) are\n  public and unauthenticated, keyed only by the EVM wallet address in the path\n  (e.g. /users/{user_address}/portfolio). Write access is via POST /exchange, which\n  accepts a signed EVM transaction body — authorization is cryptographic (the user\n  signs the order/trade transaction with their wallet key), not an API key or OAuth\n  token. The GTE Python SDK (packages/gte-packages.yml) constructs and signs the\n  transaction body.\nschemes: []\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gte/refs/heads/main/authentication/gte-authentication.yml
summary_line: signature · 0 schemes
tags:
- Company
- Crypto Defi
- Decentralized Exchange
- Trading
- Market Data
- Order Book
- Perpetuals
- MegaETH
- Blockchain
---
