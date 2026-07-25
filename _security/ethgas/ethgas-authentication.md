---
api_key_in: []
auth_types:
- wallet-signature
- http-bearer
description: ''
kind: authentication
layout: security
method: searched
name: Ethgas Authentication
name_suffix: Authentication
oauth_flows: []
overview: ETHGas secures its APIs with wallet-signature and http-bearer across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: ETHGas
provider_slug: ethgas
scheme_count: 2
schemes:
- description: Login is a three-step wallet-signature flow. POST /api/v1/user/login with the wallet address returns an EIP-712 typed message; the client signs it with the wallet key; POST /api/v1/user/login/verify with the signature returns a JWT access token (valid 1 hour).
  login_operations:
  - POST /api/v1/user/login
  - POST /api/v1/user/login/verify
  - POST /api/v1/user/login/refresh
  name: eip712WalletLogin
  standard: EIP-712
  type: wallet-signature
- applies_to: All private REST endpoints (/api/v1/*) and the WebSocket `login` command
  bearerFormat: JWT
  description: 'Private endpoints require Authorization: ''Bearer <accessToken>''. The token is the JWT issued by the login/verify flow and expires after 1 hour; renew via POST /api/v1/user/login/refresh before expiry.'
  name: bearerAuth
  scheme: bearer
  type: http
slug: ethgas-authentication
source_filename: ethgas-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://developers.ethgas.com/ (Authentication section)\ndocs: https://developers.ethgas.com/\nsummary:\n  types: [wallet-signature, http-bearer]\n  api_key_in: []\n  oauth2_flows: []\n  token_format: JWT\n  token_ttl_seconds: 3600\nschemes:\n  - name: eip712WalletLogin\n    type: wallet-signature\n    standard: EIP-712\n    description: >-\n      Login is a three-step wallet-signature flow. POST /api/v1/user/login with\n      the wallet address returns an EIP-712 typed message; the client signs it\n      with the wallet key; POST /api/v1/user/login/verify with the signature\n      returns a JWT access token (valid 1 hour).\n    login_operations:\n      - POST /api/v1/user/login\n      - POST /api/v1/user/login/verify\n      - POST /api/v1/user/login/refresh\n  - name: bearerAuth\n    type: http\n    scheme: bearer\n    bearerFormat: JWT\n    description: >-\n      Private endpoints require Authorization: 'Bearer <accessToken>'.\
  \ The token\n      is the JWT issued by the login/verify flow and expires after 1 hour; renew\n      via POST /api/v1/user/login/refresh before expiry.\n    applies_to: All private REST endpoints (/api/v1/*) and the WebSocket `login` command\npublic_access: >-\n  Public market-data endpoints under /api/v1/p/* and public WebSocket channels\n  require no authentication.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ethgas/refs/heads/main/authentication/ethgas-authentication.yml
summary_line: wallet-signature/http-bearer · 2 schemes
tags:
- Company
- Infrastructure
- Blockchain
- Ethereum
- Trading
- Preconfirmations
- Blockspace
- MEV
- DeFi
- Web3
---
