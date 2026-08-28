---
api_key_in: []
api_specs:
- filename: maicoin-max-v3-openapi.json
  format: json
  label: MAX Exchange REST API v3
  slug: maicoin-max-rest-v3
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/maicoin/refs/heads/main/openapi/maicoin-max-v3-openapi.json
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Maicoin Authentication
name_suffix: Authentication
oauth_flows: []
overview: MaiCoin declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: MaiCoin
provider_slug: maicoin
scheme_count: 3
schemes:
- algorithm: HMAC-SHA256
  applies_to: MAX Exchange REST API v3 (42 of 54 operations)
  headers:
  - description: The account's Access Key, issued from the API token management page.
    name: X-MAX-ACCESSKEY
  - description: Base64 encoding of the JSON request parameters merged with a `path` field.
    name: X-MAX-PAYLOAD
  - description: Hex HMAC-SHA256 of the payload string, keyed by the account's Secret Key.
    name: X-MAX-SIGNATURE
  - description: Selects a sub-account to operate on. Defaults to the main account, "main".
    name: X-Sub-Account
    required: false
  id: max-hmac
  in: header
  replay_protection:
    max_clock_skew_seconds: 30
    mechanism: nonce
    note: Each nonce may be used only once and must be within 30 seconds of server time. The WebSocket surface returns error 1006 for skew and 1012 for reuse.
    single_use: true
    unit: milliseconds since Unix epoch
  signing:
    parameter_transport: GET appends parameters to the query string; POST/PUT/DELETE send them in the JSON body. The signed payload must match either way.
    steps:
    - Build a parameter object containing `nonce` (Unix epoch milliseconds) plus the request parameters.
    - Merge the request `path` into that object as a `path` field.
    - JSON-serialise the merged object.
    - Base64-encode the JSON string. This is X-MAX-PAYLOAD.
    - HMAC-SHA256 the payload string using the Secret Key; hex-encode the digest. This is X-MAX-SIGNATURE.
  type: apiKey
- action: auth
  algorithm: HMAC-SHA256
  applies_to: MAX Exchange WebSocket API (private channels)
  fields:
  - apiKey
  - nonce
  - signature
  - id
  - filters
  filters:
    available:
    - order
    - trade
    - account
    - trade_update
    - fast_trade_update
    - mwallet_order
    - mwallet_trade
    - mwallet_fast_trade_update
    - mwallet_account
    - ad_ratio
    - borrowing
    default:
    - order
    - trade
    - account
  id: max-websocket-auth
  in: message
  signing:
    note: DIFFERENT FROM REST. The WebSocket signature is the hex HMAC-SHA256 of the NONCE STRING ALONE, keyed by the API secret — not of a base64 payload. A client that reuses the REST signing routine here will fail with error 1007 (authentication failed). This divergence is undocumented as a divergence; it is only visible by reading both pages.
  success_event: authenticated
  type: apiKey
- applies_to: MAX Exchange REST API v3 public endpoints (12 of 54 operations) and all public WebSocket channels
  id: none
  note: 'Public market data — markets, currencies, timestamp, k, depth, trades, tickers, ticker, and the four m-wallet public index/limit/interest endpoints — needs no credentials. Verified live: GET /api/v3/markets returned 200 unauthenticated on 2026-08-25.'
  type: none
slug: maicoin-authentication
source_filename: maicoin-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-25'\nmethod: searched\nsource: https://max-api.maicoin.com/api/doc/external/v3 (info.description, \"身分驗證\" section) + https://maicoin.github.io/max-websocket-docs/authentication.md\ndocs: https://campaign.maicoin.com/en/api-document\nnote: >-\n  DERIVATION FAILED, SEARCH SUCCEEDED. The published contract is Swagger 2.0 and declares NO\n  securityDefinitions block at all, so derive-authentication.py produced zero profiles. The three\n  auth headers are instead declared as ordinary per-operation header PARAMETERS on all 42 private\n  operations (X-MAX-ACCESSKEY / X-MAX-PAYLOAD / X-MAX-SIGNATURE), which no scorer or code generator\n  will read as a security scheme. The model below is transcribed from MaiCoin's own prose docs.\n  This is a concrete, cheap fix for MaiCoin: declaring one apiKey securityDefinition and a global\n  `security` block would make the same auth machine-readable without changing a single endpoint.\nschemes:\n- id: max-hmac\n  type: apiKey\n\
  \  in: header\n  applies_to: MAX Exchange REST API v3 (42 of 54 operations)\n  headers:\n  - name: X-MAX-ACCESSKEY\n    description: The account's Access Key, issued from the API token management page.\n  - name: X-MAX-PAYLOAD\n    description: Base64 encoding of the JSON request parameters merged with a `path` field.\n  - name: X-MAX-SIGNATURE\n    description: Hex HMAC-SHA256 of the payload string, keyed by the account's Secret Key.\n  - name: X-Sub-Account\n    required: false\n    description: Selects a sub-account to operate on. Defaults to the main account, \"main\".\n  algorithm: HMAC-SHA256\n  signing:\n    steps:\n    - Build a parameter object containing `nonce` (Unix epoch milliseconds) plus the request parameters.\n    - Merge the request `path` into that object as a `path` field.\n    - JSON-serialise the merged object.\n    - Base64-encode the JSON string. This is X-MAX-PAYLOAD.\n    - HMAC-SHA256 the payload string using the Secret Key; hex-encode the digest. This is X-MAX-SIGNATURE.\n\
  \    parameter_transport: GET appends parameters to the query string; POST/PUT/DELETE send them in the JSON body. The signed payload must match either way.\n  replay_protection:\n    mechanism: nonce\n    unit: milliseconds since Unix epoch\n    max_clock_skew_seconds: 30\n    single_use: true\n    note: 'Each nonce may be used only once and must be within 30 seconds of server time. The WebSocket surface returns error 1006 for skew and 1012 for reuse.'\n- id: max-websocket-auth\n  type: apiKey\n  in: message\n  applies_to: MAX Exchange WebSocket API (private channels)\n  action: auth\n  fields:\n  - apiKey\n  - nonce\n  - signature\n  - id\n  - filters\n  algorithm: HMAC-SHA256\n  signing:\n    note: >-\n      DIFFERENT FROM REST. The WebSocket signature is the hex HMAC-SHA256 of the NONCE STRING ALONE,\n      keyed by the API secret — not of a base64 payload. A client that reuses the REST signing routine\n      here will fail with error 1007 (authentication failed). This divergence is\
  \ undocumented as a\n      divergence; it is only visible by reading both pages.\n  success_event: authenticated\n  filters:\n    default: [order, trade, account]\n    available: [order, trade, account, trade_update, fast_trade_update, mwallet_order, mwallet_trade, mwallet_fast_trade_update, mwallet_account, ad_ratio, borrowing]\n- id: none\n  type: none\n  applies_to: MAX Exchange REST API v3 public endpoints (12 of 54 operations) and all public WebSocket channels\n  note: 'Public market data — markets, currencies, timestamp, k, depth, trades, tickers, ticker, and the four m-wallet public index/limit/interest endpoints — needs no credentials. Verified live: GET /api/v3/markets returned 200 unauthenticated on 2026-08-25.'\ncredential_issuance:\n  url: https://max.maicoin.com/api_tokens\n  prerequisites:\n  - A registered MAX account (https://max.maicoin.com/signup)\n  - Completed identity verification\n  permissions_model: >-\n    Tokens carry per-scope read permissions selected at creation\
  \ time. The WebSocket docs name\n    \"read permission for Order / Trade\" and \"read permission for Account & Personal Information\"\n    as separate grants. MaiCoin publishes no enumerated machine-readable permission list, so\n    scopes/ is intentionally absent — this is key auth, not OAuth.\noauth2: false\nopenid_connect: false\nmutual_tls: false\nsecurity_guidance:\n  published:\n  - Do not share API keys.\n  - Rotate API keys periodically.\n  - Configure an IP allow-list for additional security.\n  source: MAX V3 API reference, \"安全指南\" section\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/maicoin/refs/heads/main/authentication/maicoin-authentication.yml
summary_line: 3 schemes
tags:
- Company
- Cryptocurrency
- Digital Assets
- Exchange
- Trading
- Financial Services
- Market Data
- Blockchain
- Taiwan
- WebSocket
---
