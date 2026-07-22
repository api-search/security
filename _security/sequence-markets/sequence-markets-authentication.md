---
api_key_in:
- header
auth_types:
- http-bearer
description: ''
kind: authentication
layout: security
method: searched
name: Sequence Markets Authentication
name_suffix: Authentication
oauth_flows: []
overview: Sequence Markets secures its APIs with http-bearer across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Sequence Markets
provider_slug: sequence-markets
scheme_count: 1
schemes:
- description: Sequence-issued API key presented as a Bearer token in the Authorization header on every REST and WebSocket request. seq_live_ keys trade on real venues; seq_test_ keys force every order through the sandbox.
  key_format: seq_live_<key> (production) or seq_test_<key> (sandbox)
  location: 'Authorization: Bearer <key>'
  name: BearerApiKey
  scheme: bearer
  type: http
slug: sequence-markets-authentication
source_filename: sequence-markets-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://docs.sequencemkts.com/api/credentials/\ndocs: https://docs.sequencemkts.com/api/credentials/\nsummary:\n  types:\n  - http-bearer\n  api_key_in:\n  - header\n  bearer_header: Authorization\n  key_prefixes:\n  - seq_live_\n  - seq_test_\n  oauth2_flows: []\nschemes:\n- name: BearerApiKey\n  type: http\n  scheme: bearer\n  location: \"Authorization: Bearer <key>\"\n  key_format: \"seq_live_<key> (production) or seq_test_<key> (sandbox)\"\n  description: >-\n    Sequence-issued API key presented as a Bearer token in the Authorization\n    header on every REST and WebSocket request. seq_live_ keys trade on real\n    venues; seq_test_ keys force every order through the sandbox.\nkey_management:\n  create: POST /v1/api_keys  (body {label, sandbox})\n  list: GET /v1/api_keys\n  rotate: POST /v1/api_keys/{key_id}/rotate\n  revoke: DELETE /v1/api_keys/{key_id}\n  raw_key_note: >-\n    The raw key is returned only once at creation\
  \ time and cannot be retrieved\n    later — store it securely.\nwebsocket_auth:\n  header: \"Authorization: Bearer seq_live_...\"\n  ticket_flow:\n    endpoint: GET /v1/ws/ticket\n    returns: \"{ticket: wst_...}\"\n    connect: \"wss://api.sequencemkts.com/v1/stream?ticket=wst_...\"\n    ttl_seconds: 30\n    single_use: true\n    note: For browser clients that cannot set WebSocket headers.\nvenue_credentials:\n  note: >-\n    Downstream venue credentials are stored separately from the Sequence API\n    key. Guidance: only grant read and trade permissions for CEX API keys —\n    never enable withdrawals.\n  cex:\n    store: GET /v1/credentials  (POST /v1/credentials/{venue})\n    encryption: AES-256-GCM\n    per_venue:\n      kraken/binance/bitget/crypto.com: [api_key, api_secret]\n      coinbase: [api_key, api_secret (EC private key), passphrase (optional)]\n      kalshi: [api_key (UUID), api_secret (RSA private key)]\n      polymarket: [extra_json.signer_private_key]\n  dex:\n    store:\
  \ GET /v1/wallets\n    model: MPC-secured Sequence Wallets for on-chain trading\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sequence-markets/refs/heads/main/authentication/sequence-markets-authentication.yml
summary_line: http-bearer · 1 scheme
tags:
- Company
- Trading
- Cryptocurrency
- Digital Assets
- Execution
- Smart Order Routing
- Prediction Markets
- Algorithmic Trading
- DeFi
- Market Data
- FinTech
- Developer Tools
---
