---
api_key_in:
- header
api_specs:
- filename: openapi.json
  format: json
  label: 0xArchive REST API
  slug: 0xarchive-rest-api
  spec_type: OpenAPI
  url: https://0xarchive.io/openapi.json
auth_types:
- apiKey
- oauth2
- siwe
description: ''
kind: authentication
layout: security
method: searched
name: 0Xarchive Authentication
name_suffix: Authentication
oauth_flows: []
overview: 0xArchive secures its APIs with apiKey, oauth2, and siwe across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: 0xArchive
provider_slug: 0xarchive
scheme_count: 4
schemes:
- applies_to:
  - direct REST market-data requests
  - the three language SDKs (key passed to the client constructor)
  - the CLI (reads OXA_API_KEY)
  - the Claude Code agent skill (reads OXARCHIVE_API_KEY)
  declared_in_contract: true
  description: API key for authentication. Get yours at https://0xarchive.io/dashboard
  in: header
  key_prefix: 10
  name: ApiKeyAuth
  parameter: X-API-Key
  sources:
  - openapi/0xarchive-openapi.json
  - https://docs.0xarchive.io/rest-api/authentication
  type: apiKey
- declared_in_contract: false
  declared_in_contract_note: The WebSocket surface is not described by any machine-readable contract, so this scheme exists only in the documentation.
  description: 'The SAME API key as REST, but sent as "Authorization: Bearer <API_KEY>" during the wss://api.0xarchive.io/ws handshake rather than as X-API-Key.'
  in: handshake header
  legacy_form:
    parameter: apiKey (query string)
    status: compatibility-only
    warning: The docs restrict it to private server-side scripts and warn explicitly against browser-facing URLs and logs.
  name: WebSocketBearer
  parameter: Authorization
  scheme: bearer
  sources:
  - https://docs.0xarchive.io/websocket/connection
  - https://0xarchive.io/llms.txt
  type: http
- api_key_required: false
  applies_to:
  - the hosted MCP server at https://mcp.0xarchive.io/mcp
  declared_in_contract: false
  declared_in_contract_note: Not in the OpenAPI, because the MCP server is a separate surface. It IS machine-discoverable though - RFC 8414 metadata at api.0xarchive.io/.well-known/oauth-authorization-server and RFC 9728 metadata at mcp.0xarchive.io/.well-known/oauth-protected-resource.
  detail: scopes/0xarchive-scopes.yml
  dynamic_client_registration: https://auth.0xarchive.io/oauth/register
  flows:
    authorizationCode:
      authorizationUrl: https://auth.0xarchive.io/oauth/authorize
      refreshUrl: https://auth.0xarchive.io/oauth/token
      scopes:
        mcp:market.read: Read market data through the hosted MCP server
      tokenUrl: https://auth.0xarchive.io/oauth/token
  issuer: https://auth.0xarchive.io
  name: HostedMcpOAuth
  pkce: S256 required
  resource: https://mcp.0xarchive.io/mcp
  sources:
  - well-known/0xarchive-oauth-authorization-server.json
  - well-known/0xarchive-oauth-protected-resource.json
  - https://docs.0xarchive.io/mcp-server
  type: oauth2
- declared_in_contract: true
  declared_in_contract_note: These routes appear in the OpenAPI with an empty security array.
  description: Wallet-signed authentication requiring NO API key, used for account bootstrap and key management. POST /v1/auth/web3/challenge issues a single-use SIWE challenge; the client signs it and posts the signed message to /v1/auth/web3/verify. The same signed-message pattern authorises key listing (/v1/web3/keys) and key revocation (/v1/web3/keys/revoke).
  name: SiweWalletAuth
  sources:
  - openapi/0xarchive-openapi.json
  - https://0xarchive.io/llms.txt
  standard: EIP-4361 (Sign-In With Ethereum)
  type: signature
  unauthenticated_routes:
  - POST /v1/auth/web3/challenge
  - POST /v1/auth/web3/verify
  - POST /v1/web3/subscribe
slug: 0xarchive-authentication
source_filename: 0xarchive-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-01'\nmethod: searched\ndocs: https://docs.0xarchive.io/authentication\nsource: >-\n  Derived from openapi/0xarchive-openapi.json components.securitySchemes by\n  0-working/derive-authentication.py, then upgraded from the provider's own credential map at\n  https://docs.0xarchive.io/authentication (HTTP 200, fetched 2026-09-01), the RFC 8414\n  authorization-server metadata, and the wallet-auth routes in the contract.\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  - siwe\n  api_key_in:\n  - header\n  note: >-\n    The OpenAPI declares exactly ONE security scheme (ApiKeyAuth / X-API-Key), which is why the\n    derived baseline showed a single apiKey scheme. That baseline is accurate but incomplete as a\n    picture of how a caller actually authenticates: 0xArchive runs THREE distinct credential\n    models across four surfaces, and only one of them appears in the REST contract. This file\n    records all three, and flags which are contract-declared and which\
  \ are documentation-only.\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  key_prefix: 0xa_\n  description: API key for authentication. Get yours at https://0xarchive.io/dashboard\n  declared_in_contract: true\n  applies_to:\n  - direct REST market-data requests\n  - the three language SDKs (key passed to the client constructor)\n  - the CLI (reads OXA_API_KEY)\n  - the Claude Code agent skill (reads OXARCHIVE_API_KEY)\n  sources:\n  - openapi/0xarchive-openapi.json\n  - https://docs.0xarchive.io/rest-api/authentication\n- name: WebSocketBearer\n  type: http\n  scheme: bearer\n  in: handshake header\n  parameter: Authorization\n  description: >-\n    The SAME API key as REST, but sent as \"Authorization: Bearer <API_KEY>\" during the\n    wss://api.0xarchive.io/ws handshake rather than as X-API-Key.\n  declared_in_contract: false\n  declared_in_contract_note: >-\n    The WebSocket surface is not described by any machine-readable contract, so this scheme\n\
  \    exists only in the documentation.\n  legacy_form:\n    parameter: apiKey (query string)\n    status: compatibility-only\n    warning: >-\n      The docs restrict it to private server-side scripts and warn explicitly against\n      browser-facing URLs and logs.\n  sources:\n  - https://docs.0xarchive.io/websocket/connection\n  - https://0xarchive.io/llms.txt\n- name: HostedMcpOAuth\n  type: oauth2\n  flows:\n    authorizationCode:\n      authorizationUrl: https://auth.0xarchive.io/oauth/authorize\n      tokenUrl: https://auth.0xarchive.io/oauth/token\n      refreshUrl: https://auth.0xarchive.io/oauth/token\n      scopes:\n        mcp:market.read: Read market data through the hosted MCP server\n  pkce: S256 required\n  dynamic_client_registration: https://auth.0xarchive.io/oauth/register\n  issuer: https://auth.0xarchive.io\n  resource: https://mcp.0xarchive.io/mcp\n  declared_in_contract: false\n  declared_in_contract_note: >-\n    Not in the OpenAPI, because the MCP server is a separate\
  \ surface. It IS machine-discoverable\n    though - RFC 8414 metadata at api.0xarchive.io/.well-known/oauth-authorization-server and\n    RFC 9728 metadata at mcp.0xarchive.io/.well-known/oauth-protected-resource.\n  applies_to:\n  - the hosted MCP server at https://mcp.0xarchive.io/mcp\n  api_key_required: false\n  detail: scopes/0xarchive-scopes.yml\n  sources:\n  - well-known/0xarchive-oauth-authorization-server.json\n  - well-known/0xarchive-oauth-protected-resource.json\n  - https://docs.0xarchive.io/mcp-server\n- name: SiweWalletAuth\n  type: signature\n  standard: EIP-4361 (Sign-In With Ethereum)\n  description: >-\n    Wallet-signed authentication requiring NO API key, used for account bootstrap and key\n    management. POST /v1/auth/web3/challenge issues a single-use SIWE challenge; the client signs\n    it and posts the signed message to /v1/auth/web3/verify. The same signed-message pattern\n    authorises key listing (/v1/web3/keys) and key revocation (/v1/web3/keys/revoke).\n\
  \  declared_in_contract: true\n  declared_in_contract_note: These routes appear in the OpenAPI with an empty security array.\n  unauthenticated_routes:\n  - POST /v1/auth/web3/challenge\n  - POST /v1/auth/web3/verify\n  - POST /v1/web3/subscribe\n  sources:\n  - openapi/0xarchive-openapi.json\n  - https://0xarchive.io/llms.txt\ncredential_map:\n  note: >-\n    Transcribed from the provider's own \"Credential map\" table. Worth reading closely for the\n    env-var split, which is a real integration trap - the CLI reads OXA_API_KEY while the SDKs\n    and the agent skill read OXARCHIVE_API_KEY.\n  rows:\n  - surface: REST\n    credential: OXARCHIVE_API_KEY from the runtime environment, sent as X-API-Key\n  - surface: WebSocket\n    credential: the same API key, supplied during connection setup as a Bearer token\n  - surface: SDKs\n    credential: the key passed to the client constructor\n  - surface: CLI\n    credential: OXA_API_KEY\n  - surface: Agent skill\n    credential: OXARCHIVE_API_KEY\
  \ through the host environment or secret store\n  - surface: Hosted MCP server\n    credential: client-managed OAuth; no 0xArchive API key\n  - surface: Browser applications\n    credential: call your own backend - the docs say never expose a 0xArchive key to users\nkey_lifecycle:\n  create: https://0xarchive.io/dashboard\n  create_alternative: >-\n    A wallet can obtain an account and key with no dashboard visit at all, via the x402 path -\n    POST /v1/web3/subscribe settles a USDC payment on Base and issues the key on settlement.\n  storage_guidance: >-\n    Load from an environment variable or secret manager; never in checked-in code, notebooks,\n    prompts, logs, screenshots or public issue text.\n  rotation: >-\n    Replace keys when a workflow, machine, environment or teammate no longer needs access. The\n    docs recommend a separate key per environment (local, CI, staging, production, agent tooling)\n    so that a leaked development key cannot expose a production workflow.\n\
  \  revocation:\n    operation: web3RevokeKey\n    path: POST /v1/web3/keys/revoke\n    auth: SIWE signed message + key_id\n    reversible: false\n    note: No un-revoke path is documented. See the reversibility block in conventions/.\n  key_limits_by_tier:\n    Free: 1\n    Build: 10\n    Pro: 100\n    Scale: 200\n    Enterprise: 200\nunauthenticated_surface:\n- url: https://api.0xarchive.io/health\n  operation: healthCheck\n  http_status: 200\n  note: The only unauthenticated route on the API host; every other path returns 401, not 404.\n- url: https://0xarchive.io/.well-known/data-samples.json\n  note: Fixed public Parquet samples with checksums and reconstruction proofs. No account, no key.\n- url: https://0xarchive.io/.well-known/data-coverage.json\n  note: Public coverage manifest.\n- url: https://api.0xarchive.io/.well-known/oauth-authorization-server\n  note: Deliberately exempted from the API host's blanket 401 so an MCP client can discover the AS.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/0xarchive/refs/heads/main/authentication/0xarchive-authentication.yml
summary_line: apiKey/oauth2/siwe · 4 schemes
tags:
- market data
- historical data
- crypto
- DeFi
- perpetuals
- derivatives
- order book
- Hyperliquid
- Lighter
- HIP-3
- HIP-4
- prediction markets
- WebSocket
- streaming
- historical replay
- Parquet
- bulk data
- MCP
- agent-native
- x402
- OpenAPI
- REST
---
