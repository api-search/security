---
api_key_in: []
api_specs:
- filename: orderly-network-openapi-original.yml
  format: yaml
  label: Orderly EVM Trading API
  slug: orderly-evm-trading-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orderly-network/refs/heads/main/openapi/orderly-network-openapi-original.yml
- filename: orderly-network-strategy-vault-openapi-original.yml
  format: yaml
  label: Orderly Strategy Vault API
  slug: orderly-strategy-vault-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orderly-network/refs/heads/main/openapi/orderly-network-strategy-vault-openapi-original.yml
auth_types:
- signature
description: ''
kind: authentication
layout: security
method: searched
name: Orderly Network Authentication
name_suffix: Authentication
oauth_flows: []
overview: Orderly Network secures its APIs with signature across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Orderly Network
provider_slug: orderly-network
scheme_count: 1
schemes:
- algorithm: ed25519
  docs: https://orderly.network/docs/build-on-omnichain/user-flows/wallet-authentication
  encoding: base64url
  headers:
  - orderly-account-id
  - orderly-key
  - orderly-signature
  - orderly-timestamp
  key_format: ed25519:<base58-public-key>
  key_registration: 'Orderly Keys are generated and registered via wallet authentication (EIP-712 wallet signature), or supplied by a frontend such as WOOFi Pro.

    '
  name: OrderlyKeySignature
  signing_string: <timestamp><HTTP-METHOD><path?query><json-body>
  type: signature
  validations:
    checks:
    - signature-verification
    - key-registered-and-not-expired
    timestamp_tolerance_seconds: 300
slug: orderly-network-authentication
source_filename: orderly-network-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://orderly.network/docs/build-on-omnichain/api-authentication\ndocs: https://orderly.network/docs/build-on-omnichain/api-authentication\nnote: >\n  The OpenAPI does not declare formal securitySchemes; authentication is a\n  custom request-signing scheme documented in the auth guide and captured here.\nsummary:\n  types: [signature]\n  scheme: ed25519\n  transport: custom-headers\n  oauth2_flows: []\nschemes:\n  - name: OrderlyKeySignature\n    type: signature\n    algorithm: ed25519\n    encoding: base64url\n    key_format: \"ed25519:<base58-public-key>\"\n    headers:\n      - orderly-account-id   # registered Orderly account identifier\n      - orderly-key          # public key, ed25519:<base58>\n      - orderly-signature    # base64url ed25519 signature of the normalized request\n      - orderly-timestamp    # request time in milliseconds\n    signing_string: \"<timestamp><HTTP-METHOD><path?query><json-body>\"\n   \
  \ validations:\n      timestamp_tolerance_seconds: 300\n      checks: [signature-verification, key-registered-and-not-expired]\n    key_registration: >\n      Orderly Keys are generated and registered via wallet authentication\n      (EIP-712 wallet signature), or supplied by a frontend such as WOOFi Pro.\n    docs: https://orderly.network/docs/build-on-omnichain/user-flows/wallet-authentication\npublic_access:\n  description: >\n    Public market-data endpoints and the Public Info API (POST /v1/public/query)\n    require no authentication.\n  docs: https://orderly.network/docs/build-on-omnichain/public-info-api/overview\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/orderly-network/refs/heads/main/authentication/orderly-network-authentication.yml
summary_line: signature · 1 scheme
tags:
- Company
- Crypto
- DeFi
- Trading
- Perpetual Futures
- Derivatives
- Orderbook
- Web3
- Blockchain
- Liquidity
---
