---
api_key_in:
- header
api_specs:
- filename: debank-pro-openapi.yml
  format: yaml
  label: DeBank OpenAPI
  slug: debank-openapi
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/debank/refs/heads/main/openapi/debank-pro-openapi.yml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Debank Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: DeBank secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: DeBank
provider_slug: debank
scheme_count: 2
schemes:
- applies_to: https://pro-openapi.debank.com
  description: 'Prepaid, unit-metered access key issued from the DeBank Cloud dashboard. Applied globally — the spec sets security: [{accessKey: []}] at the root, so all 42 operations require it.'
  expiry: null
  in: header
  issued_at: https://cloud.debank.com/
  name: accessKey
  parameter: AccessKey
  rotation_policy: null
  scopes: []
  sources:
  - openapi/debank-pro-openapi.yml
  type: apiKey
- applies_to: https://api.connect.debank.com
  artifact: scopes/debank-scopes.yml
  client_authentication: client_secret_basic
  flows:
  - authorizationUrl: https://debank.com/connect
    flow: authorizationCode
    scopes:
      user:base:read: User base info
      user:chain:read: User on-chain portfolio data
      user:social:read: User social info
    tokenUrl: https://api.connect.debank.com/oauth/token
  name: DeBank Connect
  pkce: false
  refresh_token: true
  sources:
  - https://docs.cloud.debank.com/en/debank-connect/integration
  state_recommended: true
  token_type: Bearer
  type: oauth2
slug: debank-authentication
source_filename: debank-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: searched\nsource: openapi/debank-pro-openapi.yml\ndocs: https://docs.cloud.debank.com/en/readme/open-api\nnote: Two independent auth surfaces. The DeBank Cloud Pro API is api-key only (AccessKey header, no scopes, no expiry,\n  no rotation policy published). DeBank Connect is a separate OAuth 2.0 authorization-code service on api.connect.debank.com\n  that is NOT described by the published Swagger, so it was searched from the integration guide rather than derived.\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: accessKey\n  type: apiKey\n  in: header\n  parameter: AccessKey\n  applies_to: https://pro-openapi.debank.com\n  sources:\n  - openapi/debank-pro-openapi.yml\n  issued_at: https://cloud.debank.com/\n  description: 'Prepaid, unit-metered access key issued from the DeBank Cloud dashboard. Applied globally — the\n    spec sets security: [{accessKey: []}] at\
  \ the root, so all 42 operations require it.'\n  expiry: null\n  rotation_policy: null\n  scopes: []\n- name: DeBank Connect\n  type: oauth2\n  applies_to: https://api.connect.debank.com\n  sources:\n  - https://docs.cloud.debank.com/en/debank-connect/integration\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://debank.com/connect\n    tokenUrl: https://api.connect.debank.com/oauth/token\n    scopes:\n      user:base:read: User base info\n      user:chain:read: User on-chain portfolio data\n      user:social:read: User social info\n  client_authentication: client_secret_basic\n  token_type: Bearer\n  refresh_token: true\n  pkce: false\n  state_recommended: true\n  artifact: scopes/debank-scopes.yml\ngaps:\n- No /.well-known/oauth-authorization-server or /.well-known/openid-configuration on any host (404, probed 2026-08-12).\n- No key rotation, expiry or revocation policy published for the AccessKey.\n- No PKCE support documented for the public-client case.\n- The 401/403\
  \ responses are documented on the error-code page but absent from the machine-readable contract.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/debank/refs/heads/main/authentication/debank-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- Web3
- DeFi
- Blockchain
- Crypto
- Portfolio Tracking
- On-Chain Data
- Wallets
- token-data
- NFT
- Ethereum
- Authentication
- Market Data
---
