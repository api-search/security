---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Pipe Network Authentication
name_suffix: Authentication
oauth_flows: []
overview: Pipe Network declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Pipe Network
provider_slug: pipe-network
scheme_count: 2
schemes:
- bearer_format: JWT
  description: 'Sign In With Solana. Flow: auth_challenge(wallet_pubkey) -> sign returned message -> auth_verify(pubkey, nonce, message, signature_b64) -> JWT access + refresh tokens. SDKs auto-refresh on 401 and retry. auth_refresh() renews; auth_logout() invalidates the session.'
  endpoints:
    challenge: POST /auth/challenge
    identity: GET /user/me
    logout: POST /auth/logout
    refresh: POST /auth/refresh
    verify: POST /auth/verify
  id: siws-bearer
  preferred: true
  scheme: bearer
  type: http
- description: 'Provisioned application-key mode (legacy / compatibility). Every authenticated CDN endpoint takes user_id + user_app_key. Obtained via /createUser and rotated via /rotateAppKey. SDK env: PIPE_API_KEY (holds a user_app_key or a JWT access token) + PIPE_ACCOUNT.'
  id: user-app-key
  in: query
  parameters:
  - user_id
  - user_app_key
  preferred: false
  type: apiKey
slug: pipe-network-authentication
source_filename: pipe-network-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://github.com/PipeNetwork/lib-storage\ndocs: https://github.com/PipeNetwork/docs/blob/main/docs/cdn-api/api-documentation.md\nsummary: >-\n  Pipe Storage supports two auth models. The preferred/current model is SIWS\n  (Sign In With Solana): a wallet signs a server challenge and receives short-\n  lived JWT access + refresh tokens used as bearer credentials. A compatibility\n  model uses a provisioned per-user application key (user_app_key) passed with\n  the user_id. There is no OAuth 2.0 / OpenID Connect layer.\nschemes:\n- id: siws-bearer\n  type: http\n  scheme: bearer\n  bearer_format: JWT\n  preferred: true\n  description: >-\n    Sign In With Solana. Flow: auth_challenge(wallet_pubkey) -> sign returned\n    message -> auth_verify(pubkey, nonce, message, signature_b64) -> JWT access\n    + refresh tokens. SDKs auto-refresh on 401 and retry. auth_refresh() renews;\n    auth_logout() invalidates the session.\n  endpoints:\n\
  \    challenge: POST /auth/challenge\n    verify: POST /auth/verify\n    refresh: POST /auth/refresh\n    logout: POST /auth/logout\n    identity: GET /user/me\n- id: user-app-key\n  type: apiKey\n  in: query\n  preferred: false\n  description: >-\n    Provisioned application-key mode (legacy / compatibility). Every\n    authenticated CDN endpoint takes user_id + user_app_key. Obtained via\n    /createUser and rotated via /rotateAppKey. SDK env: PIPE_API_KEY (holds a\n    user_app_key or a JWT access token) + PIPE_ACCOUNT.\n  parameters:\n  - user_id\n  - user_app_key\nenv_vars:\n- PIPE_API_KEY   # user_app_key or JWT access token\n- PIPE_ACCOUNT   # account id for deterministic URL generation\n- PIPE_BASE_URL  # default https://us-west-01-firestarter.pipenetwork.com\npayments:\n  standard: x402\n  note: SDKs include x402 agent-payment support for machine-to-machine settlement.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pipe-network/refs/heads/main/authentication/pipe-network-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Crypto Web3
- Storage
- Decentralized Storage
- Content Delivery Network
- Solana
- Encryption
- AI Agents
- Web3
---
