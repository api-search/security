---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: cymetica-com-eventtrader-public-api-openapi.yml
  format: yaml
  label: EventTrader Public API
  slug: eventtrader-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cymetica-com/refs/heads/main/openapi/cymetica-com-eventtrader-public-api-openapi.yml
auth_types:
- apiKey
- http
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 4
method: searched
name: Cymetica Com Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Cymetica secures its APIs with apiKey, http, and oauth2 across 4 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Cymetica
provider_slug: cymetica-com
scheme_count: 4
schemes:
- in: header
  issuance:
  - POST /auth/api-key (JWT or email+password bootstrap) -> api_key + api_secret
  - POST /api/v1/api-keys (session JWT only) -> named key with permissions {read, trade, withdraw}
  - POST /mcp/v1/register (no auth) -> mcp_ key, trust_level recognized
  key_prefixes:
    agent: mcp_
    user: evt_
  name: ApiKeyAuth
  parameter: X-API-Key
  permissions:
  - read
  - trade
  - withdraw (registered agent keys only; user keys and OAuth tokens cannot withdraw)
  sources:
  - openapi/cymetica-com-eventtrader-public-api-openapi.yml
  storage: SHA-256 hashed; plaintext shown once
  type: apiKey
- bearerFormat: JWT
  description: Account session JWT (from /auth/login). Key-management routes accept only this — never an API key.
  issuance:
  - POST /auth/login (email/password) -> access_token + refresh_token
  - POST /auth/register
  - SIWE wallet sign-in (EventTrader.from_wallet in the Python SDK)
  name: BearerJWT
  scheme: bearer
  sources:
  - openapi/cymetica-com-eventtrader-public-api-openapi.yml
  type: http
- discovery:
    authorization_server_metadata: well-known/cymetica-com-oauth-authorization-server.json
    grant_types:
    - authorization_code
    - refresh_token
    pkce: S256
    protected_resource_metadata: well-known/cymetica-com-oauth-protected-resource.json
    registration_endpoint: https://cymetica.com/oauth/register
    revocation_endpoint: https://cymetica.com/oauth/revoke
    token_endpoint_auth_methods:
    - none
    - client_secret_post
    - client_secret_basic
    userinfo_endpoint: https://cymetica.com/oauth/userinfo
  flows:
  - authorizationUrl: https://cymetica.com/oauth/authorize
    flow: authorizationCode
    scopes: 3
    tokenUrl: https://cymetica.com/oauth/token
  name: OAuth2
  note: OAuth bearer tokens work on the REST API (/api/v1/*); the /mcp/v1 JSON-RPC endpoint uses X-API-Key (mcp.json authentication.oauth.note).
  sources:
  - openapi/cymetica-com-eventtrader-public-api-openapi.yml
  type: oauth2
- description: POST /auth/api-key returns an api_secret "for HMAC-signed integrations" (docs); the signing scheme is not documented in the spec or the docs.
  name: HMAC (api_secret)
  sources:
  - https://cymetica.com/api-docs
  - https://cymetica.com/getting-started
  status: mentioned-not-specified
  type: custom
slug: cymetica-com-authentication
source_filename: cymetica-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: searched\nsource: openapi/cymetica-com-eventtrader-public-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - authorizationCode\n  docs_upgrade: 'Three documented ways in: (1) register + POST /auth/api-key under a JWT, (2) one-call bootstrap\n    POST /auth/api-key with email+password, (3) POST /mcp/v1/register for an instant mcp_ agent key. Plus OAuth\n    2.0 authorization-code with PKCE S256 (RFC 8414 + RFC 9728 discovery, RFC 7591 registration) whose tokens work\n    on REST but not on /mcp/v1, and SIWE wallet sign-in via the Python SDK. A 401 carries WWW-Authenticate: Bearer\n    and {\"detail\": \"Authentication required. Provide Bearer token or X-API-Key header.\"}.'\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  sources:\n  - openapi/cymetica-com-eventtrader-public-api-openapi.yml\n  key_prefixes:\n    user: evt_\n    agent: mcp_\n\
  \  issuance:\n  - POST /auth/api-key (JWT or email+password bootstrap) -> api_key + api_secret\n  - POST /api/v1/api-keys (session JWT only) -> named key with permissions {read, trade, withdraw}\n  - POST /mcp/v1/register (no auth) -> mcp_ key, trust_level recognized\n  permissions:\n  - read\n  - trade\n  - withdraw (registered agent keys only; user keys and OAuth tokens cannot withdraw)\n  storage: SHA-256 hashed; plaintext shown once\n- name: BearerJWT\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: Account session JWT (from /auth/login). Key-management routes accept only this — never an API key.\n  sources:\n  - openapi/cymetica-com-eventtrader-public-api-openapi.yml\n  issuance:\n  - POST /auth/login (email/password) -> access_token + refresh_token\n  - POST /auth/register\n  - SIWE wallet sign-in (EventTrader.from_wallet in the Python SDK)\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://cymetica.com/oauth/authorize\n\
  \    tokenUrl: https://cymetica.com/oauth/token\n    scopes: 3\n  sources:\n  - openapi/cymetica-com-eventtrader-public-api-openapi.yml\n  discovery:\n    authorization_server_metadata: well-known/cymetica-com-oauth-authorization-server.json\n    protected_resource_metadata: well-known/cymetica-com-oauth-protected-resource.json\n    registration_endpoint: https://cymetica.com/oauth/register\n    revocation_endpoint: https://cymetica.com/oauth/revoke\n    userinfo_endpoint: https://cymetica.com/oauth/userinfo\n    pkce: S256\n    grant_types:\n    - authorization_code\n    - refresh_token\n    token_endpoint_auth_methods:\n    - none\n    - client_secret_post\n    - client_secret_basic\n  note: OAuth bearer tokens work on the REST API (/api/v1/*); the /mcp/v1 JSON-RPC endpoint uses X-API-Key (mcp.json\n    authentication.oauth.note).\n- name: HMAC (api_secret)\n  type: custom\n  status: mentioned-not-specified\n  description: POST /auth/api-key returns an api_secret \"for HMAC-signed integrations\"\
  \ (docs); the signing scheme\n    is not documented in the spec or the docs.\n  sources:\n  - https://cymetica.com/api-docs\n  - https://cymetica.com/getting-started\ndocs: https://cymetica.com/api-docs#authentication\nsources_searched:\n- https://cymetica.com/api-docs (Authentication, API Key Management)\n- https://cymetica.com/getting-started\n- https://cymetica.com/sdk (Authentication)\n- https://cymetica.com/.well-known/oauth-authorization-server\n- https://cymetica.com/.well-known/oauth-protected-resource\n- https://cymetica.com/.well-known/mcp.json\n- live 401 probe of GET /api/v1/portfolio/positions\nmcp:\n  endpoint: https://cymetica.com/mcp/v1\n  anonymous_access: 57 public tools with no credentials\n  header: X-API-Key\n  trust_tiers:\n  - unknown\n  - recognized\n  - trusted\n  - allied\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cymetica-com/refs/heads/main/authentication/cymetica-com-authentication.yml
summary_line: apiKey/http/oauth2 · 4 schemes
tags:
- Prediction Markets
- Cryptocurrency Exchange
- Trading
- AI Agents
- MCP
- agent-native
- Blockchain
- DeFi
- Financial-Services
- Market Data
---
