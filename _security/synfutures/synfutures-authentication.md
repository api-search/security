---
api_key_in:
- header
api_specs:
- filename: synfutures-rwa-trading-openapi.yml
  format: yaml
  label: SynFutures RWA Trading API
  slug: synfutures-rwa-trading-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/synfutures/refs/heads/main/openapi/synfutures-rwa-trading-openapi.yml
auth_types:
- apiKey
- hmac
description: ''
kind: authentication
layout: security
method: searched
name: Synfutures Authentication
name_suffix: Authentication
oauth_flows: []
overview: SynFutures secures its APIs with apiKey and hmac across 6 declared security schemes, as derived from its OpenAPI definitions.
provider_name: SynFutures
provider_slug: synfutures
scheme_count: 6
schemes:
- description: Partner API key. Must be active, not expired, and have an IP whitelist configured; a key with an empty/unset whitelist rejects ALL requests with 401.
  in: header
  name: ApiKeyAuth
  parameter: x-api-key
  sources:
  - openapi/synfutures-rwa-trading-openapi.yml
  type: apiKey
- algorithm: HMAC-SHA256
  description: HMAC-SHA256 signature over the canonical request.
  encoding: hex (case-insensitive)
  in: header
  name: ApiSignature
  parameter: x-api-sign
  type: hmac
- description: Unix millisecond timestamp; must be within 45s drift tolerance.
  in: header
  name: ApiTimestamp
  parameter: x-api-ts
  type: apiKey
- description: Unique nonce per key within the 45s window (UUID recommended); replay prevention.
  in: header
  name: ApiNonce
  parameter: x-api-nonce
  type: apiKey
- description: Chain identifier for the request.
  in: header
  name: ApiChainId
  parameter: x-api-chain-id
  type: apiKey
- description: Product type; use "Synfutures".
  in: header
  name: ApiProduct
  parameter: x-api-p
  type: apiKey
slug: synfutures-authentication
source_filename: synfutures-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://docs.synfutures.com/rwa-trading-apis/authentication/headers-and-permissions.md\ndocs: https://docs.synfutures.com/rwa-trading-apis/authentication/signature\nsummary:\n  types: [apiKey, hmac]\n  api_key_in: [header]\n  signed_requests: true\n  scheme: HMAC-SHA256\nschemes:\n  - name: ApiKeyAuth\n    type: apiKey\n    in: header\n    parameter: x-api-key\n    description: Partner API key. Must be active, not expired, and have an IP whitelist configured; a key with an empty/unset whitelist rejects ALL requests with 401.\n    sources: [openapi/synfutures-rwa-trading-openapi.yml]\n  - name: ApiSignature\n    type: hmac\n    in: header\n    parameter: x-api-sign\n    algorithm: HMAC-SHA256\n    encoding: hex (case-insensitive)\n    description: HMAC-SHA256 signature over the canonical request.\n  - name: ApiTimestamp\n    type: apiKey\n    in: header\n    parameter: x-api-ts\n    description: Unix millisecond timestamp; must\
  \ be within 45s drift tolerance.\n  - name: ApiNonce\n    type: apiKey\n    in: header\n    parameter: x-api-nonce\n    description: Unique nonce per key within the 45s window (UUID recommended); replay prevention.\n  - name: ApiChainId\n    type: apiKey\n    in: header\n    parameter: x-api-chain-id\n    description: Chain identifier for the request.\n  - name: ApiProduct\n    type: apiKey\n    in: header\n    parameter: x-api-p\n    description: Product type; use \"Synfutures\".\npermissions:\n  model: key-level access level (not OAuth scopes)\n  levels:\n    - name: READ_ONLY\n      allows: [GET]\n    - name: WRITABLE\n      allows: [GET, POST, DELETE]\nchains:\n  - {name: Base Mainnet, chain_id: 8453}\n  - {name: Ethereum Mainnet, chain_id: 1}\n  - {name: Monad Mainnet, chain_id: 143}\n  - {name: Ethereum Sepolia, chain_id: 11155111}\n  - {name: Monad Testnet, chain_id: 10143}\n  - {name: Base Sepolia, chain_id: 84532}\nnotes:\n  - API keys are issued by the SynFutures team (contact\
  \ via Discord or X); the API is in beta.\n  - One Click Trading (1CT) uses EIP-712 delegated signatures for on-chain actions without per-tx wallet prompts.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/synfutures/refs/heads/main/authentication/synfutures-authentication.yml
summary_line: apiKey/hmac · 6 schemes
tags:
- Company
- Crypto
- DeFi
- Trading
- Derivatives
- Real World Assets
- Blockchain
- API
---
