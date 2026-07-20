---
api_key_in: []
api_specs:
- filename: bullet-trading-api-openapi.json
  format: json
  label: Bullet Trading API
  slug: bullet-trading-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bullet/refs/heads/main/openapi/bullet-trading-api-openapi.json
auth_types:
- signature
description: ''
kind: authentication
layout: security
method: searched
name: Bullet Authentication
name_suffix: Authentication
oauth_flows: []
overview: Bullet secures its APIs with signature across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Bullet
provider_slug: bullet
scheme_count: 1
schemes:
- algorithm: Ed25519
  applies_to:
  - POST /tx/submit
  - POST /api/v1/solanaOffchainTx
  - POST /rollup/simulate
  name: ed25519-signed-transaction
  sources:
  - https://tradingapi.bullet.xyz/docs/tx-signing.html
  type: signature
slug: bullet-authentication
source_filename: bullet-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://tradingapi.bullet.xyz/docs/tx-signing.html\ndocs: https://tradingapi.bullet.xyz/docs/account-setup.html\nsummary:\n  types: [signature]\n  model: ed25519 signed transactions (Solana-style)\n  read_access: public (market-data and health endpoints require no credentials)\n  write_access: ed25519-signed transactions submitted to the exchange\nnotes: >-\n  The Bullet Trading API declares no OAuth2 / API-key security schemes in its OpenAPI. Read\n  endpoints (Market-Data, Health, and most Account queries) are open. All write operations\n  (placing/cancelling orders, deposits/withdrawals) are submitted as ed25519-signed\n  transactions: build the call message, wrap in an UnsignedTransaction (call + uniqueness +\n  tx details), sign borsh(unsigned_tx) ++ chain_hash with an ed25519 key, wrap in a\n  SignedTransaction, base64-encode, and POST to /tx/submit (or over WebSocket).\nschemes:\n- name: ed25519-signed-transaction\n\
  \  type: signature\n  algorithm: Ed25519\n  applies_to: [POST /tx/submit, POST /api/v1/solanaOffchainTx, POST /rollup/simulate]\n  sources: [https://tradingapi.bullet.xyz/docs/tx-signing.html]\ndelegate_accounts:\n  supported: true\n  docs: https://docs.bullet.xyz/exchange/help-center/delegate-accounts-and-api.md\n  description: >-\n    A delegate account is a separate ed25519 keypair authorized by the main wallet to sign\n    API/trading transactions, so automated clients never hold the primary wallet key. Delegate\n    wallet addresses are ed25519 addresses; the delegate private key is used to sign submitted\n    transactions.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bullet/refs/heads/main/authentication/bullet-authentication.yml
summary_line: signature · 1 scheme
tags:
- Company
- DeFi
- Solana
- Cryptocurrency
- Derivatives
- Exchange
- Trading
- Perpetuals
- Lending
- Blockchain
---
