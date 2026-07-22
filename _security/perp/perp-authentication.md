---
api_key_in:
- header
auth_types:
- apiKey
- hmac
description: ''
kind: authentication
layout: security
method: searched
name: Perp Authentication
name_suffix: Authentication
oauth_flows: []
overview: Perp secures its APIs with apiKey and hmac across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Perp
provider_slug: perp
scheme_count: 3
schemes:
- credentials:
    api_key:
      format: perp_live_<48 hex> (live) or perp_test_<...> (testnet)
      header: X-API-Key
    api_secret:
      format: 32 random bytes (64 hex chars)
      note: never retransmitted after creation
    signature:
      format: HMAC-SHA256 over the request pre-image (hex)
      header: X-Signature
    timestamp:
      drift_tolerance: +/- 5 seconds; clock must be NTP-synced
      format: Unix time in milliseconds
      header: X-Timestamp
  errors:
  - MM_1001_INVALID_API_KEY
  - MM_1002_KEY_REVOKED
  - MM_1005_INVALID_SIGNATURE
  - MM_1006_SIGNATURE_EXPIRED
  - MM_1008_NOT_AUTHENTICATED
  in: header
  name: hmac-api-key
  scheme: hmac-sha256
  sources:
  - docs/market-maker-api
  type: apiKey
  websocket:
    note: WebSocket connections authenticate with an AUTHENTICATE command carrying the same X-API-Key / X-Timestamp / X-Signature fields.
- name: eip712-order-signature
  note: Individual orders carry an EIP-712 signature produced by the trader's wallet; the signer must be authorized for the API key. Bad or mismatched signatures return MM_2010_INVALID_ORDER_SIGNATURE / MM_2011_WALLET_MISMATCH.
  scheme: eip712-wallet-signature
  sources:
  - docs/market-maker-api
  type: mutualTLS
- name: curie-subgraph-public
  note: The Curie (v2) GraphQL subgraph is public and unauthenticated on The Graph hosted service (now sunset; see lifecycle).
  scheme: none
  sources:
  - apis.yml
  type: apiKey
slug: perp-authentication
source_filename: perp-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://perp.com/docs/market-maker-api\ndocs: https://perp.com/docs/market-maker-api\nsummary:\n  types: [apiKey, hmac]\n  api_key_in: [header]\n  oauth2_flows: []\n  note: >-\n    The perp.com V1 Market Maker API uses HMAC-SHA256 request signing with an\n    API key + secret pair. There is no OAuth surface. The public Curie (v2)\n    GraphQL subgraph on The Graph requires no authentication. Order placement\n    additionally requires an on-chain EIP-712 wallet signature over the order\n    payload.\nschemes:\n  - name: hmac-api-key\n    type: apiKey\n    scheme: hmac-sha256\n    in: header\n    credentials:\n      api_key:\n        header: X-API-Key\n        format: 'perp_live_<48 hex> (live) or perp_test_<...> (testnet)'\n      api_secret:\n        format: 32 random bytes (64 hex chars)\n        note: never retransmitted after creation\n      timestamp:\n        header: X-Timestamp\n        format: Unix time in milliseconds\n\
  \        drift_tolerance: '+/- 5 seconds; clock must be NTP-synced'\n      signature:\n        header: X-Signature\n        format: HMAC-SHA256 over the request pre-image (hex)\n    websocket:\n      note: >-\n        WebSocket connections authenticate with an AUTHENTICATE command carrying\n        the same X-API-Key / X-Timestamp / X-Signature fields.\n    errors:\n      - MM_1001_INVALID_API_KEY\n      - MM_1002_KEY_REVOKED\n      - MM_1005_INVALID_SIGNATURE\n      - MM_1006_SIGNATURE_EXPIRED\n      - MM_1008_NOT_AUTHENTICATED\n    sources: [docs/market-maker-api]\n  - name: eip712-order-signature\n    type: mutualTLS\n    scheme: eip712-wallet-signature\n    note: >-\n      Individual orders carry an EIP-712 signature produced by the trader's\n      wallet; the signer must be authorized for the API key. Bad or mismatched\n      signatures return MM_2010_INVALID_ORDER_SIGNATURE / MM_2011_WALLET_MISMATCH.\n    sources: [docs/market-maker-api]\n  - name: curie-subgraph-public\n    type:\
  \ apiKey\n    scheme: none\n    note: >-\n      The Curie (v2) GraphQL subgraph is public and unauthenticated on The Graph\n      hosted service (now sunset; see lifecycle).\n    sources: [apis.yml]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/perp/refs/heads/main/authentication/perp-authentication.yml
summary_line: apiKey/hmac · 3 schemes
tags:
- Company
- Crypto Web3
- DeFi
- Derivatives
- Perpetual Futures
- Prediction Markets
- Optimism
- GraphQL
- Blockchain
- SDK
---
