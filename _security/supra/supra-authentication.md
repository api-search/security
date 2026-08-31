---
api_key_in: []
api_specs:
- filename: supra-rpc-node-openapi.yml
  format: yaml
  label: Supra RPC Node API
  slug: supra-rpc-node-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/supra/refs/heads/main/openapi/supra-rpc-node-openapi.yml
- filename: supra-rpc-node-openapi.yml
  format: yaml
  label: Supra Automation API
  slug: supra-automation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/supra/refs/heads/main/openapi/supra-rpc-node-openapi.yml
auth_types: []
description: 'Supra runs two authentication regimes side by side. The Layer 1 node RPC is fully public and keyless — no API key, no OAuth, no securityScheme in the OpenAPI at all — because authority on a blockchain comes from the signature inside the transaction payload, not from a credential on the HTTP call. The oracle Price Feeds REST and WebSocket APIs are the opposite: an x-api-key header is mandatory, and the key is issued by hand through a Google Form request, with the surface labelled Early Access.'
kind: authentication
layout: security
method: searched
name: Supra Authentication
name_suffix: Authentication
oauth_flows: []
overview: Supra declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Supra
provider_slug: supra
scheme_count: 2
schemes:
- applies_to: Supra RPC Node API (https://rpc-mainnet.supra.com, https://rpc-testnet.supra.com)
  description: No credential is required for any of the 56 operations. Reads are open. Writes (submit_txn_v3, submit_txn) carry a signed transaction in the request body; the Ed25519 / multi-agent signature inside SignedTransaction is the authorization, and the node verifies it against the sender's on-chain authentication key and sequence number. There is no server-side account to authenticate to.
  evidence:
    openapi_security_schemes: []
    probe: https://rpc-mainnet.supra.com/rpc/v1/transactions/chain_id
    status: 200
  id: none
  in: n/a
  optional_node_operator_auth:
    description: 'Per the OpenAPI description of the WebSocket upgrade operation, "When the node configures websocket_auth_tokens, clients must send Authorization: Bearer <token>. Connection and subscription limits are enforced per token." This is a per-node-operator configuration, not a Supra-issued credential, and the public mainnet endpoint does not require it.'
    mechanism: Authorization Bearer token
    surface: GET /rpc/v4/ws
  type: none
- applies_to: Supra Price Feeds REST API (https://prod-kline-rest.supra.com) and Supra Price Feeds WebSocket API (wss://prod-kline-ws.supra.com)
  description: Static API key sent on every request and on the WebSocket handshake. Missing key returns HTTP 401 with the JSON body {"error":"API key is missing"} — confirmed by probing https://prod-kline-rest.supra.com/latest unauthenticated on 2026-08-29.
  docs: https://docs.supra.com/oracles/apis-real-time-and-historical-data/rest-api
  evidence:
    body: '{"error":"API key is missing"}'
    probe: https://prod-kline-rest.supra.com/latest
    status: 401
  id: price-feeds-api-key
  in: header
  key_issuance: Manual. The docs link a Google Form request ("Please request your key here") rather than a self-serve developer console; there is no signup, dashboard, or key-rotation UI documented.
  name: x-api-key
  signup: https://docs.google.com/forms/d/e/1FAIpQLSfHZr8BHLTY8q_MjbuKZPpdgQS0oGmRIrsn9H-HrieH9eQjFw/viewform
  status: Early Access — the docs state "Supra APIs are currently available in Early Access mode".
  type: apiKey
slug: supra-authentication
source_filename: supra-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-29'\nmethod: searched\nsource: >-\n  https://docs.supra.com/oracles/apis-real-time-and-historical-data/rest-api and\n  https://docs.supra.com/oracles/apis-real-time-and-historical-data/websocket-api for the price feeds key;\n  openapi/supra-rpc-node-openapi.yml (served by rpc-mainnet.supra.com/docs/api.json) for the node API, which\n  declares no components.securitySchemes and no top-level security requirement; verified against a live keyless\n  call to https://rpc-mainnet.supra.com/rpc/v1/transactions/chain_id (HTTP 200, returned \"8\") on 2026-08-29.\ndescription: >-\n  Supra runs two authentication regimes side by side. The Layer 1 node RPC is fully public and keyless — no API\n  key, no OAuth, no securityScheme in the OpenAPI at all — because authority on a blockchain comes from the\n  signature inside the transaction payload, not from a credential on the HTTP call. The oracle Price Feeds REST\n  and WebSocket APIs are the opposite: an x-api-key header\
  \ is mandatory, and the key is issued by hand through a\n  Google Form request, with the surface labelled Early Access.\nschemes:\n- id: none\n  type: none\n  applies_to: Supra RPC Node API (https://rpc-mainnet.supra.com, https://rpc-testnet.supra.com)\n  in: n/a\n  description: >-\n    No credential is required for any of the 56 operations. Reads are open. Writes (submit_txn_v3,\n    submit_txn) carry a signed transaction in the request body; the Ed25519 / multi-agent signature inside\n    SignedTransaction is the authorization, and the node verifies it against the sender's on-chain\n    authentication key and sequence number. There is no server-side account to authenticate to.\n  evidence:\n    probe: https://rpc-mainnet.supra.com/rpc/v1/transactions/chain_id\n    status: 200\n    openapi_security_schemes: []\n  optional_node_operator_auth:\n    surface: GET /rpc/v4/ws\n    mechanism: Authorization Bearer token\n    description: >-\n      Per the OpenAPI description of the WebSocket\
  \ upgrade operation, \"When the node configures\n      websocket_auth_tokens, clients must send Authorization: Bearer <token>. Connection and subscription limits\n      are enforced per token.\" This is a per-node-operator configuration, not a Supra-issued credential, and the\n      public mainnet endpoint does not require it.\n- id: price-feeds-api-key\n  type: apiKey\n  applies_to: >-\n    Supra Price Feeds REST API (https://prod-kline-rest.supra.com) and Supra Price Feeds WebSocket API\n    (wss://prod-kline-ws.supra.com)\n  in: header\n  name: x-api-key\n  description: >-\n    Static API key sent on every request and on the WebSocket handshake. Missing key returns HTTP 401 with the\n    JSON body {\"error\":\"API key is missing\"} — confirmed by probing https://prod-kline-rest.supra.com/latest\n    unauthenticated on 2026-08-29.\n  key_issuance: >-\n    Manual. The docs link a Google Form request (\"Please request your key here\") rather than a self-serve\n    developer console; there\
  \ is no signup, dashboard, or key-rotation UI documented.\n  signup: https://docs.google.com/forms/d/e/1FAIpQLSfHZr8BHLTY8q_MjbuKZPpdgQS0oGmRIrsn9H-HrieH9eQjFw/viewform\n  docs: https://docs.supra.com/oracles/apis-real-time-and-historical-data/rest-api\n  evidence:\n    probe: https://prod-kline-rest.supra.com/latest\n    status: 401\n    body: '{\"error\":\"API key is missing\"}'\n  status: Early Access — the docs state \"Supra APIs are currently available in Early Access mode\".\noauth2: false\nopenid_connect: false\nmutual_tls: false\nnotes:\n- >-\n  No OAuth 2.0 or OpenID Connect anywhere: /.well-known/oauth-authorization-server and\n  /.well-known/openid-configuration return 404 on all five probed hosts (see well-known/supra-well-known.yml),\n  so scopes/ is not applicable for this provider.\n- >-\n  Wallet-level authentication for end users is handled by StarKey, Supra's first-party self-custodial wallet,\n  and is a client-side signing concern rather than an API credential.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/supra/refs/heads/main/authentication/supra-authentication.yml
summary_line: 2 schemes
tags:
- Blockchain
- Layer 1
- Oracles
- Web3
- Market Data
- Smart Contracts
- Verifiable Randomness
- Cross-Chain Bridge
- Automation
- Move
- Cryptocurrency
- DeFi
---
