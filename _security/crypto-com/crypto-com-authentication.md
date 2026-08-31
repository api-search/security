---
api_key_in:
- body
- header
api_specs:
- filename: crypto-com-account-balance-and-positions-api-openapi.yml
  format: yaml
  label: Crypto.com Account Balance and Positions API
  slug: crypto-com-account-balance-and-positions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crypto-com/refs/heads/main/openapi/crypto-com-account-balance-and-positions-api-openapi.yml
- filename: crypto-com-advanced-order-management-api-openapi.yml
  format: yaml
  label: Crypto.com Advanced Order Management API
  slug: crypto-com-advanced-order-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crypto-com/refs/heads/main/openapi/crypto-com-advanced-order-management-api-openapi.yml
- filename: crypto-com-crypto-wallet-api-openapi.yml
  format: yaml
  label: Crypto.com Crypto Wallet API
  slug: crypto-com-crypto-wallet-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crypto-com/refs/heads/main/openapi/crypto-com-crypto-wallet-api-openapi.yml
- filename: crypto-com-fiat-wallet-api-openapi.yml
  format: yaml
  label: Crypto.com Fiat Wallet API
  slug: crypto-com-fiat-wallet-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crypto-com/refs/heads/main/openapi/crypto-com-fiat-wallet-api-openapi.yml
- filename: crypto-com-otc-rfq-for-taker-api-openapi.yml
  format: yaml
  label: Crypto.com OTC RFQ for Taker API
  slug: crypto-com-otc-rfq-for-taker-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crypto-com/refs/heads/main/openapi/crypto-com-otc-rfq-for-taker-api-openapi.yml
- filename: crypto-com-reference-and-market-data-api-openapi.yml
  format: yaml
  label: Crypto.com Reference and Market Data API
  slug: crypto-com-reference-and-market-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crypto-com/refs/heads/main/openapi/crypto-com-reference-and-market-data-api-openapi.yml
- filename: crypto-com-staking-api-openapi.yml
  format: yaml
  label: Crypto.com Staking API
  slug: crypto-com-staking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crypto-com/refs/heads/main/openapi/crypto-com-staking-api-openapi.yml
- filename: crypto-com-trading-api-openapi.yml
  format: yaml
  label: Crypto.com Trading API
  slug: crypto-com-trading-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crypto-com/refs/heads/main/openapi/crypto-com-trading-api-openapi.yml
- filename: crypto-com-trading-bot-api-api-openapi.yml
  format: yaml
  label: Crypto.com Trading Bot API
  slug: crypto-com-trading-bot-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crypto-com/refs/heads/main/openapi/crypto-com-trading-bot-api-api-openapi.yml
- filename: crypto-com-transaction-history-api-openapi.yml
  format: yaml
  label: Crypto.com Transaction History API
  slug: crypto-com-transaction-history-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crypto-com/refs/heads/main/openapi/crypto-com-transaction-history-api-openapi.yml
auth_types:
- apiKey
- http
- custom-hmac
description: ''
kind: authentication
layout: security
method: searched
name: Crypto Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: Crypto.com secures its APIs with apiKey, http, and custom-hmac across 6 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Crypto.com
provider_slug: crypto-com
scheme_count: 6
schemes:
- algorithm: HMAC-SHA256, hex-encoded
  api: Crypto.com Exchange REST API v1
  in: body
  key_management: Exchange website, User Center -> API. Default permission is read-only; permissions and an optional source-IP allowlist are set in the web UI.
  name: exchange-hmac-signature
  nonce: UTC Unix timestamp in milliseconds; rejected with 40102 INVALID_NONCE when more than 60 seconds from server time
  parameter_string: request params sorted by key ascending, concatenated as key+value with no spaces or delimiters
  parameters:
  - api_key
  - sig
  - nonce
  signing_string: method + id + api_key + parameter_string + nonce
  sources:
  - https://exchange-developer.crypto.com/exchange/v1/docs/api/rest-common-api-reference
  spec_declared: false
  type: custom-hmac
- api: Crypto.com Exchange WebSocket API v1
  in: message
  name: exchange-websocket-session-auth
  note: public/auth is invoked once per session with the same HMAC-SHA256 signature; afterwards user-channel commands need no per-request signature for the life of the session.
  parameters:
  - api_key
  - sig
  - nonce
  sources:
  - https://exchange-developer.crypto.com/exchange/v1/docs/api/websocket-common-api-reference
  spec_declared: false
  type: custom-hmac
- api: Crypto.com Exchange FIX API
  in: fix-message
  name: exchange-fix-logon
  note: Credentials are presented on the FIX Logon (35=A) message over an AWS PrivateLink connection.
  sources:
  - https://exchange-developer.crypto.com/exchange/v1/docs/api/fix-api-key
  spec_declared: false
  type: custom-hmac
- api: Crypto.com Pay API
  header: Authorization
  in: header
  name: pay-secret-key
  note: 'The secret key is the HTTP Basic username with an empty password. Bearer is also accepted for cross-origin calls. Key prefix selects the mode: sk_test_ = test mode, sk_live_ = live mode. HTTPS is mandatory; plain HTTP calls fail.'
  scheme: basic
  sources:
  - https://pay-docs.crypto.com/
  spec_declared: false
  type: http
- api: Crypto.com Developer Platform API
  in: header
  name: developer-platform-api-key
  note: API key issued against a project in the Developer Platform dashboard at developer.crypto.com; supplied by the first-party TypeScript/Python clients via Client.init(api_key).
  sources:
  - https://ai-agent-sdk-docs.crypto.com/crypto.com-developer-platform/developer-platform-dashboard
  spec_declared: false
  type: apiKey
- api: cdcx CLI / MCP server
  name: cdcx-oauth-login
  note: The first-party CLI offers `cdcx auth login --oauth`, a browser-based login that provisions credentials locally. Crypto.com publishes no OAuth authorization-server metadata, no /.well-known/oauth-authorization-server, and no scope reference, so this is not a documented third-party OAuth surface and no scopes/ artifact is emitted.
  sources:
  - https://github.com/crypto-com/crypto-agent-trading/blob/main/crypto-com-exchange/SKILL.md
  spec_declared: false
  type: oauth-device-browser
slug: crypto-com-authentication
source_filename: crypto-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-11'\nmethod: searched\nsource: https://exchange-developer.crypto.com/exchange/v1/docs/api/rest-common-api-reference\ndocs:\n- https://exchange-developer.crypto.com/exchange/v1/docs/api/rest-common-api-reference\n- https://pay-docs.crypto.com/\n- https://ai-agent-sdk-docs.crypto.com/crypto.com-developer-platform/developer-platform-dashboard\nsummary:\n  types:\n  - apiKey\n  - http\n  - custom-hmac\n  api_key_in:\n  - body\n  - header\n  oauth2_flows: []\n  note: No OAuth 2.0 or OpenID Connect surface is published on any Crypto.com API. The Exchange REST OpenAPI\n    declares NO components.securitySchemes at all, even though 85 of its 95 operations document a 401\n    response - the auth contract lives only in prose. See overlays/crypto-com-exchange-overlay.yaml for\n    the scheme API Evangelist would add.\nschemes:\n- name: exchange-hmac-signature\n  api: Crypto.com Exchange REST API v1\n  type: custom-hmac\n  in: body\n  parameters:\n  - api_key\n  - sig\n\
  \  - nonce\n  algorithm: HMAC-SHA256, hex-encoded\n  signing_string: method + id + api_key + parameter_string + nonce\n  parameter_string: request params sorted by key ascending, concatenated as key+value with no spaces or\n    delimiters\n  nonce: UTC Unix timestamp in milliseconds; rejected with 40102 INVALID_NONCE when more than 60 seconds\n    from server time\n  key_management: Exchange website, User Center -> API. Default permission is read-only; permissions and\n    an optional source-IP allowlist are set in the web UI.\n  sources:\n  - https://exchange-developer.crypto.com/exchange/v1/docs/api/rest-common-api-reference\n  spec_declared: false\n- name: exchange-websocket-session-auth\n  api: Crypto.com Exchange WebSocket API v1\n  type: custom-hmac\n  in: message\n  parameters:\n  - api_key\n  - sig\n  - nonce\n  note: public/auth is invoked once per session with the same HMAC-SHA256 signature; afterwards user-channel\n    commands need no per-request signature for the life of the\
  \ session.\n  sources:\n  - https://exchange-developer.crypto.com/exchange/v1/docs/api/websocket-common-api-reference\n  spec_declared: false\n- name: exchange-fix-logon\n  api: Crypto.com Exchange FIX API\n  type: custom-hmac\n  in: fix-message\n  note: Credentials are presented on the FIX Logon (35=A) message over an AWS PrivateLink connection.\n  sources:\n  - https://exchange-developer.crypto.com/exchange/v1/docs/api/fix-api-key\n  spec_declared: false\n- name: pay-secret-key\n  api: Crypto.com Pay API\n  type: http\n  scheme: basic\n  in: header\n  header: Authorization\n  note: 'The secret key is the HTTP Basic username with an empty password. Bearer is also accepted for\n    cross-origin calls. Key prefix selects the mode: sk_test_ = test mode, sk_live_ = live mode. HTTPS\n    is mandatory; plain HTTP calls fail.'\n  sources:\n  - https://pay-docs.crypto.com/\n  spec_declared: false\n- name: developer-platform-api-key\n  api: Crypto.com Developer Platform API\n  type: apiKey\n \
  \ in: header\n  note: API key issued against a project in the Developer Platform dashboard at developer.crypto.com;\n    supplied by the first-party TypeScript/Python clients via Client.init(api_key).\n  sources:\n  - https://ai-agent-sdk-docs.crypto.com/crypto.com-developer-platform/developer-platform-dashboard\n  spec_declared: false\n- name: cdcx-oauth-login\n  api: cdcx CLI / MCP server\n  type: oauth-device-browser\n  note: The first-party CLI offers `cdcx auth login --oauth`, a browser-based login that provisions credentials\n    locally. Crypto.com publishes no OAuth authorization-server metadata, no /.well-known/oauth-authorization-server,\n    and no scope reference, so this is not a documented third-party OAuth surface and no scopes/ artifact\n    is emitted.\n  sources:\n  - https://github.com/crypto-com/crypto-agent-trading/blob/main/crypto-com-exchange/SKILL.md\n  spec_declared: false\ngaps:\n- openapi/crypto-com-exchange-openapi.yml declares no components.securitySchemes\
  \ and no top-level security,\n  so an agent reading only the contract cannot discover how to authenticate.\n- No /.well-known/openid-configuration or /.well-known/oauth-authorization-server on any Crypto.com host\n  (all probed 404 on 2026-08-11).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/crypto-com/refs/heads/main/authentication/crypto-com-authentication.yml
summary_line: apiKey/http/custom-hmac · 6 schemes
tags:
- cryptocurrency
- crypto-exchange
- Trading
- Derivatives
- Market Data
- digital-assets
- Payments
- merchant-payments
- Blockchain
- cronos
- DeFi
- staking
- Fintech
- MCP
- agent-native
---
