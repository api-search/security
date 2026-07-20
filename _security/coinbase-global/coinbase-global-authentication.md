---
api_key_in:
- header
auth_types:
- apiKey
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Coinbase Global Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Coinbase Global secures its APIs with apiKey, http, and oauth2 across 4 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Coinbase Global
provider_slug: coinbase-global
scheme_count: 4
schemes:
- bearerFormat: JWT
  description: Coinbase Developer Platform API v2 / Advanced Trade authenticate server requests with a short-lived JWT signed by the project's API key (Ed25519 or EC key pair). See JWT Authentication docs.
  docs: https://docs.cdp.coinbase.com/get-started/authentication/jwt-authentication
  name: CDP JWT Bearer
  products:
  - CDP API v2
  - Advanced Trade API
  scheme: bearer
  type: http
- description: Non-custodial wallet write operations additionally require a wallet secret configured in the CDP portal.
  docs: https://docs.cdp.coinbase.com/get-started/authentication/security-best-practices
  in: header
  name: Wallet Secret
  products:
  - CDP Wallets
  type: apiKey
- description: The legacy Coinbase App / Sign in with Coinbase (API v2) supports API key + secret with an HMAC request signature (CB-ACCESS-KEY / CB-ACCESS-SIGN).
  in: header
  name: Coinbase App API Key (HMAC)
  products:
  - Coinbase App API v2
  type: apiKey
- description: Sign in with Coinbase (Coinbase App API) supports OAuth2 authorization code flow for delegated end-user access.
  flows:
    authorizationCode:
      authorizationUrl: https://login.coinbase.com/oauth2/auth
      tokenUrl: https://login.coinbase.com/oauth2/token
  name: OAuth2
  products:
  - Coinbase App API v2
  - Sign in with Coinbase
  type: oauth2
slug: coinbase-global-authentication
source_filename: coinbase-global-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://docs.cdp.coinbase.com/get-started/authentication/overview\ndocs: https://docs.cdp.coinbase.com/get-started/authentication/overview\nsummary:\n  types: [apiKey, http, oauth2]\n  api_key_in: [header]\n  oauth2_flows: [authorizationCode]\nschemes:\n  - name: CDP JWT Bearer\n    type: http\n    scheme: bearer\n    bearerFormat: JWT\n    description: >-\n      Coinbase Developer Platform API v2 / Advanced Trade authenticate server\n      requests with a short-lived JWT signed by the project's API key\n      (Ed25519 or EC key pair). See JWT Authentication docs.\n    docs: https://docs.cdp.coinbase.com/get-started/authentication/jwt-authentication\n    products: [CDP API v2, Advanced Trade API]\n  - name: Wallet Secret\n    type: apiKey\n    in: header\n    description: >-\n      Non-custodial wallet write operations additionally require a wallet\n      secret configured in the CDP portal.\n    docs: https://docs.cdp.coinbase.com/get-started/authentication/security-best-practices\n\
  \    products: [CDP Wallets]\n  - name: Coinbase App API Key (HMAC)\n    type: apiKey\n    in: header\n    description: >-\n      The legacy Coinbase App / Sign in with Coinbase (API v2) supports API key\n      + secret with an HMAC request signature (CB-ACCESS-KEY / CB-ACCESS-SIGN).\n    products: [Coinbase App API v2]\n  - name: OAuth2\n    type: oauth2\n    description: >-\n      Sign in with Coinbase (Coinbase App API) supports OAuth2 authorization\n      code flow for delegated end-user access.\n    flows:\n      authorizationCode:\n        authorizationUrl: https://login.coinbase.com/oauth2/auth\n        tokenUrl: https://login.coinbase.com/oauth2/token\n    products: [Coinbase App API v2, Sign in with Coinbase]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/coinbase-global/refs/heads/main/authentication/coinbase-global-authentication.yml
summary_line: apiKey/http/oauth2 · 4 schemes
tags:
- Company
- Cryptocurrency
- Blockchain
- Payments
- Wallets
- Trading
- Onchain
- Web3
- Financial Services
- Developer Platform
- AI Agents
- Stablecoins
---
