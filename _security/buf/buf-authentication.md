---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Buf Authentication
name_suffix: Authentication
oauth_flows: []
overview: Buf declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: Buf
provider_slug: buf
scheme_count: 3
schemes:
- anonymous_access: Public modules on the public BSR are readable without credentials. Private instances typically require authentication for every call regardless of repository visibility.
  applies_to: Every BSR RPC over Connect, gRPC and gRPC-Web, on buf.build and on private instances. Also accepted by the MCP server for headless/CI use.
  bot_identity: Bot users are a private-instance feature only; they are not offered on the public buf.build. Instance admins create them so headless tokens survive staff changes.
  env_var: BUF_TOKEN
  expiry: user-chosen at creation time
  format: Bearer <BUF_TOKEN>
  header: Authorization
  id: bsr_bearer_token
  in: header
  issuance:
  - '`buf registry login` opens a browser flow, prompts for an expiration, and writes the token to $HOME/.netrc (%HOME%/_netrc on Windows).'
  - Created by hand in account settings (Create New Token → pick expiration → add a note).
  multi_host: BUF_TOKEN accepts a comma-separated list of <token>@<hostname> entries so one machine can hold credentials for the public BSR and a private instance at once; the CLI matches the remote hostname to the right token.
  precedence:
  - BUF_TOKEN environment variable
  - $HOME/.netrc
  revocation: Delete the token by name in account settings; revocation is immediate.
  scheme: bearer
  type: http
- applies_to: https://buf.build/mcp
  authorization_endpoint: https://buf.build/oauth2/authorize
  challenge_observed: 'Anonymous POST to the MCP endpoint returns 401 with WWW-Authenticate: Bearer resource_metadata="https://buf.build/.well-known/oauth-protected-resource/mcp", scope="mcp"'
  client_authentication: none (public clients)
  dynamic_client_registration: true
  flow: authorization_code
  grant_types:
  - authorization_code
  - refresh_token
  id: bsr_mcp_oauth2
  issuer: https://buf.build
  note: The token the flow mints is an ordinary BSR API token and appears in account settings under the client's consent-screen name, which is also how it is revoked.
  pkce: required (S256)
  registration_endpoint: https://buf.build/oauth2/register
  resource_metadata: https://buf.build/.well-known/oauth-protected-resource/mcp
  scopes:
  - mcp
  token_endpoint: https://buf.build/oauth2/token
  type: oauth2
- applies_to: Human sign-in to buf.build (/login, /signup) — not an API credential.
  discovery: https://login.buf.build/.well-known/openid-configuration
  enterprise: Pro and Enterprise instances support custom SSO with SAML and OIDC, plus SCIM for server admin and bulk user management.
  id: end_user_sso
  issuer: https://login.buf.build/
  type: openIdConnect
slug: buf-authentication
source_filename: buf-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-13'\nmethod: searched\nsource: https://buf.build/docs/bsr/authentication/\ndocs:\n  - https://buf.build/docs/bsr/authentication/\n  - https://buf.build/docs/bsr/apis/api-access/\n  - https://buf.build/docs/bsr/apis/mcp/\nderived_from:\n  - well-known/buf-oauth-authorization-server.json\n  - well-known/buf-oauth-protected-resource-mcp.json\nsummary: >-\n  The Buf Schema Registry authenticates API calls with a user-scoped bearer token. There is\n  no API-key header, no HMAC signing, and no mTLS. A second, separate OAuth2 authorization\n  server exists purely to issue those same tokens to MCP clients.\nschemes:\n  - id: bsr_bearer_token\n    type: http\n    scheme: bearer\n    in: header\n    header: Authorization\n    format: 'Bearer <BUF_TOKEN>'\n    applies_to: >-\n      Every BSR RPC over Connect, gRPC and gRPC-Web, on buf.build and on private\n      instances. Also accepted by the MCP server for headless/CI use.\n    issuance:\n      - '`buf registry login`\
  \ opens a browser flow, prompts for an expiration, and writes the token to $HOME/.netrc (%HOME%/_netrc on Windows).'\n      - 'Created by hand in account settings (Create New Token → pick expiration → add a note).'\n    expiry: user-chosen at creation time\n    revocation: 'Delete the token by name in account settings; revocation is immediate.'\n    env_var: BUF_TOKEN\n    multi_host: >-\n      BUF_TOKEN accepts a comma-separated list of <token>@<hostname> entries so one machine\n      can hold credentials for the public BSR and a private instance at once; the CLI\n      matches the remote hostname to the right token.\n    precedence:\n      - BUF_TOKEN environment variable\n      - $HOME/.netrc\n    anonymous_access: >-\n      Public modules on the public BSR are readable without credentials. Private instances\n      typically require authentication for every call regardless of repository visibility.\n    bot_identity: >-\n      Bot users are a private-instance feature only; they are\
  \ not offered on the public\n      buf.build. Instance admins create them so headless tokens survive staff changes.\n  - id: bsr_mcp_oauth2\n    type: oauth2\n    flow: authorization_code\n    pkce: required (S256)\n    issuer: https://buf.build\n    authorization_endpoint: https://buf.build/oauth2/authorize\n    token_endpoint: https://buf.build/oauth2/token\n    registration_endpoint: https://buf.build/oauth2/register\n    dynamic_client_registration: true\n    client_authentication: none (public clients)\n    grant_types: [authorization_code, refresh_token]\n    scopes: [mcp]\n    applies_to: https://buf.build/mcp\n    resource_metadata: https://buf.build/.well-known/oauth-protected-resource/mcp\n    challenge_observed: >-\n      Anonymous POST to the MCP endpoint returns 401 with\n      WWW-Authenticate: Bearer resource_metadata=\"https://buf.build/.well-known/oauth-protected-resource/mcp\", scope=\"mcp\"\n    note: >-\n      The token the flow mints is an ordinary BSR API token and\
  \ appears in account settings\n      under the client's consent-screen name, which is also how it is revoked.\n  - id: end_user_sso\n    type: openIdConnect\n    issuer: https://login.buf.build/\n    discovery: https://login.buf.build/.well-known/openid-configuration\n    applies_to: 'Human sign-in to buf.build (/login, /signup) — not an API credential.'\n    enterprise: >-\n      Pro and Enterprise instances support custom SSO with SAML and OIDC, plus SCIM for\n      server admin and bulk user management.\nci:\n  pattern: 'Store the token in the CI secret store and expose it as BUF_TOKEN; the Buf CLI reads it on every command.'\n  netrc_fallback: 'echo \"${BUF_TOKEN}\" | buf registry login --token-stdin'\n  documented_providers: [GitHub Actions, Travis CI, CircleCI]\ngaps:\n  - 'No per-token scoping on BSR API tokens: a token carries the full access of the user or bot user it belongs to, including writes. The only scope in the system is \"mcp\", and it gates the MCP transport, not the\
  \ operations behind it.'\n  - 'No OpenID Connect discovery document on the API host itself; api.buf.build/.well-known/openid-configuration is a 404.'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/buf/refs/heads/main/authentication/buf-authentication.yml
summary_line: 3 schemes
tags:
- Code Generation
- gRPC
- Kafka
- Open Source
- Protocol Buffers
- Schema Registry
- SDK
- Streaming
---
