---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: gemini-trust-rest-openapi.yml
  format: yaml
  label: Gemini Crypto Trading REST API
  slug: gemini-crypto-trading-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gemini-trust/refs/heads/main/openapi/gemini-trust-rest-openapi.yml
- filename: gemini-trust-prediction-markets-openapi.yml
  format: yaml
  label: Gemini Prediction Markets REST API
  slug: gemini-prediction-markets-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gemini-trust/refs/heads/main/openapi/gemini-trust-prediction-markets-openapi.yml
- filename: gemini-trust-websocket-asyncapi.yml
  format: yaml
  label: Gemini WebSocket API
  slug: gemini-websocket-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/gemini-trust/refs/heads/main/asyncapi/gemini-trust-websocket-asyncapi.yml
auth_types:
- apiKey
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Gemini Trust Authentication
name_suffix: Authentication
oauth_flows: []
overview: Gemini Trust Company secures its APIs with apiKey, oauth2, and openIdConnect across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Gemini Trust Company
provider_slug: gemini-trust
scheme_count: 3
schemes:
- description: Gemini API key with appropriate permissions
  in: header
  name: apiKey
  parameter: X-GEMINI-APIKEY
  sources:
  - openapi/gemini-trust-prediction-markets-openapi.yml
  - openapi/gemini-trust-rest-openapi.yml
  type: apiKey
- description: Base64-encoded private REST payload. See Gemini private REST authentication.
  in: header
  name: payloadAuth
  parameter: X-GEMINI-PAYLOAD
  sources:
  - openapi/gemini-trust-prediction-markets-openapi.yml
  - openapi/gemini-trust-rest-openapi.yml
  type: apiKey
- description: Hex HMAC-SHA384 signature of the payload using the API secret.
  in: header
  name: signatureAuth
  parameter: X-GEMINI-SIGNATURE
  sources:
  - openapi/gemini-trust-prediction-markets-openapi.yml
  - openapi/gemini-trust-rest-openapi.yml
  type: apiKey
slug: gemini-trust-authentication
source_filename: gemini-trust-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-18'\nmethod: searched\nsource: https://developer.gemini.com/authentication/api-key, https://developer.gemini.com/authentication/oauth, https://api.gemini.com/.well-known/oauth-authorization-server,\n  plus openapi/gemini-trust-rest-openapi.yml and openapi/gemini-trust-prediction-markets-openapi.yml securitySchemes\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  - openIdConnect\n  api_key_in:\n  - header\n  note: The two OpenAPIs declare ONLY the three apiKey header schemes. OAuth 2.0 and the SSO OIDC surface are real\n    and fully documented but are absent from both specs - a machine reading the contract alone would never discover\n    the delegated-access model or its 33 scopes.\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: X-GEMINI-APIKEY\n  description: Gemini API key with appropriate permissions\n  sources:\n  - openapi/gemini-trust-prediction-markets-openapi.yml\n  - openapi/gemini-trust-rest-openapi.yml\n- name: payloadAuth\n\
  \  type: apiKey\n  in: header\n  parameter: X-GEMINI-PAYLOAD\n  description: Base64-encoded private REST payload. See Gemini private REST authentication.\n  sources:\n  - openapi/gemini-trust-prediction-markets-openapi.yml\n  - openapi/gemini-trust-rest-openapi.yml\n- name: signatureAuth\n  type: apiKey\n  in: header\n  parameter: X-GEMINI-SIGNATURE\n  description: Hex HMAC-SHA384 signature of the payload using the API secret.\n  sources:\n  - openapi/gemini-trust-prediction-markets-openapi.yml\n  - openapi/gemini-trust-rest-openapi.yml\ndocs:\n- https://developer.gemini.com/authentication/api-key\n- https://developer.gemini.com/authentication/oauth\n- https://developer.gemini.com/roles\nmodels:\n- name: API key (HMAC-SHA384)\n  primary: true\n  in_spec: true\n  headers:\n  - X-GEMINI-APIKEY\n  - X-GEMINI-PAYLOAD\n  - X-GEMINI-SIGNATURE\n  - 'Content-Length: 0'\n  - 'Content-Type: text/plain'\n  - 'Cache-Control: no-cache'\n  transport_note: 'Unusual and easy to get wrong: private REST\
  \ requests send an EMPTY HTTP body. The JSON payload\n    is base64-encoded into X-GEMINI-PAYLOAD, and X-GEMINI-SIGNATURE is hex(HMAC_SHA384(base64(payload), key=api_secret)).\n    Gemini warns explicitly that generic OpenAPI-generated clients do not implement this signing transport.'\n  key_prefixes:\n    account-: account-scoped key\n    master-: master key spanning sub-accounts; requires an account parameter\n  replay_protection:\n    field: nonce\n    modes:\n    - name: time-based (recommended)\n      rule: Unix epoch seconds, validated within +/- 30 seconds of server time\n    - name: incremental\n      rule: strictly increasing per API session key\n    error: InvalidNonce\n  sessions: Each API key is an independent session with its own nonce sequence; Cancel-on-Disconnect ties open orders\n    to a session heartbeat.\n  provision: https://exchange.gemini.com/settings/api\n- name: OAuth 2.0 authorization code\n  primary: false\n  in_spec: false\n  grants:\n  - authorization_code\n\
  \  - refresh_token\n  pkce: S256; REQUIRED for public clients (SPA, mobile, desktop). Client type is permanent at app creation.\n  client_types:\n  - confidential (client_id + client_secret)\n  - public (client_id only, PKCE)\n  token_lifetime:\n    access_token: 24 hours\n    refresh_token: non-expiring\n  review: Gemini reviews registered applications before production activation; sandbox registration is immediate.\n  scopes: 33 published - see scopes/gemini-trust-scopes.yml\n  revocation:\n  - https://exchange.gemini.com/auth/token/revoke\n  - REST operation revokeOAuthToken (POST /v1/oauth/revokeByToken)\n  metadata: https://api.gemini.com/.well-known/oauth-authorization-server (RFC 8414)\n- name: OpenID Connect (SSO)\n  primary: false\n  in_spec: false\n  scope: Exchange SSO only, not the trading API\n  issuer: https://exchange.gemini.com\n  signing: RS256\n  client_auth: private_key_jwt\n  scopes:\n  - openid\n  - email\n  metadata: https://api.gemini.com/.well-known/openid-configuration\n\
  - name: WebSocket authentication\n  primary: false\n  in_spec: asyncapi\n  methods:\n  - X-GEMINI-APIKEY + X-GEMINI-NONCE + X-GEMINI-PAYLOAD + X-GEMINI-SIGNATURE on the connection upgrade\n  - 'Authorization: Bearer <OAuth token>'\n  docs: https://developer.gemini.com/websocket/authentication\nauthorization:\n  model: role-based access control per API key\n  roles:\n  - Administrator (Master keys only - create and view accounts in the Master Group)\n  - Trader (assigned by default)\n  - Fund Manager\n  - Auditor\n  failure: HTTP 403 with reason MissingRole\n  docs: https://developer.gemini.com/roles\n  ip_allowlist: Group-level IP allowlisting is enforced; a request from an off-list address returns reason RemoteAddressForbidden.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gemini-trust/refs/heads/main/authentication/gemini-trust-authentication.yml
summary_line: apiKey/oauth2/openIdConnect · 3 schemes
tags:
- Company
- Cryptocurrency
- Exchange
- Trading
- Market Data
- Order Management
- Clearing
- Custody
- Financial-Services
- Prediction Markets
- Staking
- Derivatives
- WebSocket
- FIX
---
