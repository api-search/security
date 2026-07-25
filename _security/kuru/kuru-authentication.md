---
api_key_in: []
api_specs:
- filename: kuru-generate-token-api-openapi.yml
  format: yaml
  label: Kuru Generate Token API
  slug: kuru-generate-token-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kuru/refs/heads/main/openapi/kuru-generate-token-api-openapi.yml
- filename: kuru-quote-api-openapi.yml
  format: yaml
  label: Kuru Quote API
  slug: kuru-quote-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kuru/refs/heads/main/openapi/kuru-quote-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Kuru Authentication
name_suffix: Authentication
oauth_flows: []
overview: Kuru declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Kuru
provider_slug: kuru
scheme_count: 2
schemes:
- applied_to:
  - calculateBestPath
  bearer_format: JWT
  description: JWT token obtained from the /api/generate-token endpoint.
  expires: true
  expiry_field: expires_at
  expiry_format: unix-timestamp
  header: Authorization
  id: BearerAuth
  location: header
  mint_endpoint: POST https://ws.kuru.io/api/generate-token
  mint_input: user_address (Ethereum address, ^0x[a-fA-F0-9]{40}$)
  minted_by: generateToken
  rate_limit:
    burst: 1
    rps: 1
  scheme: bearer
  type: http
  value_prefix: 'Bearer '
- applied_to:
  - calculateBestPath
  description: API key for authentication.
  header: X-API-Key
  id: ApiKeyAuth
  location: header
  type: apiKey
slug: kuru-authentication
source_filename: kuru-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: openapi/kuru-flow-openapi.json + https://docs.kuru.io/api-reference/generate-jwt-token\ndocs: https://docs.kuru.io/kuru-flow/flow-overview\napi: Kuru Flow API\nhost: https://ws.kuru.io\nsummary: >-\n  The Kuru Flow API accepts either a short-lived JWT bearer token minted from a\n  user's Ethereum address, or a provisioned API key sent in the X-API-Key\n  header. The token-minting endpoint itself is unauthenticated. There is no\n  OAuth 2.0 or OpenID Connect surface, so no scopes artifact applies.\nschemes:\n  - id: BearerAuth\n    type: http\n    scheme: bearer\n    bearer_format: JWT\n    location: header\n    header: Authorization\n    value_prefix: 'Bearer '\n    description: JWT token obtained from the /api/generate-token endpoint.\n    minted_by: generateToken\n    mint_endpoint: POST https://ws.kuru.io/api/generate-token\n    mint_input: user_address (Ethereum address, ^0x[a-fA-F0-9]{40}$)\n    expires: true\n    expiry_field:\
  \ expires_at\n    expiry_format: unix-timestamp\n    rate_limit:\n      rps: 1\n      burst: 1\n    applied_to:\n      - calculateBestPath\n  - id: ApiKeyAuth\n    type: apiKey\n    location: header\n    header: X-API-Key\n    description: API key for authentication.\n    applied_to:\n      - calculateBestPath\nunauthenticated_operations:\n  - operationId: generateToken\n    path: /api/generate-token\n    method: post\n    note: Token minting is open; the returned JWT is what carries the rate limit.\noauth2: false\nopenid_connect: false\nmutual_tls: false\nscopes: none\nfailure_modes:\n  - status: 401\n    error: unauthorized\n    meaning: Invalid or missing authentication on /api/quote.\n  - status: 429\n    error: too_many_requests\n    meaning: JWT rate limit (1 RPS) exceeded.\nwallet_auth:\n  note: >-\n    End-user product authentication is wallet-based via an embedded Privy\n    wallet; this is a product surface, not an API credential.\n  docs: https://docs.kuru.io/product/wallet\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kuru/refs/heads/main/authentication/kuru-authentication.yml
summary_line: 2 schemes
tags:
- Company
- DeFi
- Decentralized Exchange
- Order Book
- Trading
- Blockchain
- Monad
- Liquidity
- Swaps
- Web3
---
