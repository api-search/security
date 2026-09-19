---
anonymous_access: false
api_key_in: []
api_specs:
- filename: aeternity-accounts-api-openapi.yml
  format: yaml
  label: Aeternity Accounts API
  slug: aeternity-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aeternity/refs/heads/main/openapi/aeternity-accounts-api-openapi.yml
- filename: aeternity-aex141-api-openapi.yml
  format: yaml
  label: Aeternity Aex141 API
  slug: aeternity-aex141-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aeternity/refs/heads/main/openapi/aeternity-aex141-api-openapi.yml
- filename: aeternity-aex9-api-openapi.yml
  format: yaml
  label: Aeternity Aex9 API
  slug: aeternity-aex9-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aeternity/refs/heads/main/openapi/aeternity-aex9-api-openapi.yml
- filename: aeternity-channels-api-openapi.yml
  format: yaml
  label: Aeternity Channels API
  slug: aeternity-channels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aeternity/refs/heads/main/openapi/aeternity-channels-api-openapi.yml
- filename: aeternity-contracts-api-openapi.yml
  format: yaml
  label: Aeternity Contracts API
  slug: aeternity-contracts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aeternity/refs/heads/main/openapi/aeternity-contracts-api-openapi.yml
- filename: aeternity-dex-api-openapi.yml
  format: yaml
  label: Aeternity Dex API
  slug: aeternity-dex-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aeternity/refs/heads/main/openapi/aeternity-dex-api-openapi.yml
- filename: aeternity-external-api-openapi.yml
  format: yaml
  label: Aeternity External API
  slug: aeternity-external-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aeternity/refs/heads/main/openapi/aeternity-external-api-openapi.yml
- filename: aeternity-hyperchain-api-openapi.yml
  format: yaml
  label: Aeternity Hyperchain API
  slug: aeternity-hyperchain-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aeternity/refs/heads/main/openapi/aeternity-hyperchain-api-openapi.yml
- filename: aeternity-internal-api-openapi.yml
  format: yaml
  label: Aeternity Internal API
  slug: aeternity-internal-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aeternity/refs/heads/main/openapi/aeternity-internal-api-openapi.yml
- filename: aeternity-key-blocks-api-openapi.yml
  format: yaml
  label: Aeternity Key Blocks API
  slug: aeternity-key-blocks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aeternity/refs/heads/main/openapi/aeternity-key-blocks-api-openapi.yml
- filename: aeternity-micro-blocks-api-openapi.yml
  format: yaml
  label: Aeternity Micro Blocks API
  slug: aeternity-micro-blocks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aeternity/refs/heads/main/openapi/aeternity-micro-blocks-api-openapi.yml
- filename: aeternity-names-api-openapi.yml
  format: yaml
  label: Aeternity Names API
  slug: aeternity-names-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aeternity/refs/heads/main/openapi/aeternity-names-api-openapi.yml
- filename: aeternity-oracles-api-openapi.yml
  format: yaml
  label: Aeternity Oracles API
  slug: aeternity-oracles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aeternity/refs/heads/main/openapi/aeternity-oracles-api-openapi.yml
- filename: aeternity-stats-api-openapi.yml
  format: yaml
  label: Aeternity Stats API
  slug: aeternity-stats-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aeternity/refs/heads/main/openapi/aeternity-stats-api-openapi.yml
- filename: aeternity-status-api-openapi.yml
  format: yaml
  label: Aeternity Status API
  slug: aeternity-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aeternity/refs/heads/main/openapi/aeternity-status-api-openapi.yml
- filename: aeternity-transactions-api-openapi.yml
  format: yaml
  label: Aeternity Transactions API
  slug: aeternity-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aeternity/refs/heads/main/openapi/aeternity-transactions-api-openapi.yml
- filename: aeternity-transfers-api-openapi.yml
  format: yaml
  label: Aeternity Transfers API
  slug: aeternity-transfers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aeternity/refs/heads/main/openapi/aeternity-transfers-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 0
method: derived
name: Aeternity Authentication
name_suffix: Authentication
oauth_flows: []
overview: Aeternity declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Aeternity
provider_slug: aeternity
scheme_count: 0
schemes: []
slug: aeternity-authentication
source_filename: aeternity-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-12'\nmethod: derived\nsource: >-\n  openapi/aeternity-node-openapi.yml, openapi/aeternity-middleware-openapi.yml,\n  well-known/aeternity-oauth-authorization-server.json, well-known/aeternity-oauth-protected-resource.json,\n  live unauthenticated probes of https://mainnet.aeternity.io/v3/status and https://mainnet.aeternity.io/mdw/v3/status (2026-09-12)\nsummary: >-\n  The two blockchain APIs are fully open — no key, no token, no signup. Authority on æternity is carried by\n  the cryptographic signature inside the transaction payload, not by an API credential, so read endpoints\n  need nothing and the single write endpoint (POST /transactions) accepts a transaction the caller has\n  already signed with their own private key. The only credentialed surface in this profile is the remote MCP\n  endpoint on aeternity.com, which is OAuth 2.1 gated.\nsurfaces:\n- name: Aeternity Node API\n  base: https://mainnet.aeternity.io/v3\n  scheme: none\n  security_schemes_declared:\
  \ 0\n  probe:\n    url: https://mainnet.aeternity.io/v3/status\n    http_status: 200\n    authenticated: false\n  detail: >-\n    No securitySchemes and no security requirement in the spec. The internal/debug endpoint family is not\n    protected by a credential either — it is simply not exposed on the public gateway, and returns 403\n    \"Info not enabled\" (GetPeers) where it is disabled. Running your own node is how you get that surface.\n  signing:\n    model: client-side transaction signing\n    detail: >-\n      Write authority = an Ed25519 signature over the serialized transaction, produced by the caller. The\n      node validates the signature and the account nonce; it never holds caller credentials. Obtain the next\n      nonce from GetAccountNextNonce before signing.\n- name: Aeternity Middleware API (REST + GraphQL + WebSocket)\n  base: https://mainnet.aeternity.io/mdw/v3\n  scheme: none\n  security_schemes_declared: 0\n  probe:\n    url: https://mainnet.aeternity.io/mdw/v3/status\n\
  \    http_status: 200\n    authenticated: false\n  detail: >-\n    Read-only index over the chain; no securityScheme declared, CORS wide open\n    (access-control-allow-origin *). GraphQL introspection is enabled and answered anonymously.\n- name: Aeternity MCP Server\n  base: https://aeternity.com/wp-json/mcp/mcp-oauth-server\n  scheme: oauth2\n  flow: authorization_code\n  detail: >-\n    Advertised by RFC 9728 protected-resource metadata and RFC 8414 authorization-server metadata on\n    aeternity.com. Authorization code with PKCE (S256 only), refresh_token supported, bearer token in the\n    Authorization header, a single scope (mcp), token_endpoint_auth_methods_supported \"none\" (public\n    clients), and dynamic registration via client-id metadata documents\n    (client_id_metadata_document_supported: true). An anonymous tools/list returns 401 rest_not_logged_in.\n  endpoints:\n    issuer: https://aeternity.com\n    authorization: https://aeternity.com/oauth/authorize\n    token:\
  \ https://aeternity.com/oauth/token\n    revocation: https://aeternity.com/oauth/revoke\n  probe:\n    url: https://aeternity.com/wp-json/mcp/mcp-oauth-server\n    http_status: 401\n  see: scopes/aeternity-scopes.yml\nno_credential_required: true\nsignup_required: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aeternity/refs/heads/main/authentication/aeternity-authentication.yml
summary_line: 0 schemes
tags:
- Blockchain
- Layer 1
- Smart Contracts
- Cryptocurrency
- Web3
- Distributed Ledger
- Open-Source
- GraphQL
- State Channels
- Oracle
- Naming System
- Developer Tools
---
