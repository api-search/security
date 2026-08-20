---
api_key_in: []
api_specs:
- filename: konbiniapi-instagram-api-openapi.yml
  format: yaml
  label: KonbiniAPI Instagram API
  slug: konbiniapi-instagram-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/konbiniapi/refs/heads/main/openapi/konbiniapi-instagram-api-openapi.yml
- filename: konbiniapi-tiktok-api-openapi.yml
  format: yaml
  label: KonbiniAPI TikTok API
  slug: konbiniapi-tiktok-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/konbiniapi/refs/heads/main/openapi/konbiniapi-tiktok-api-openapi.yml
- filename: konbiniapi-x-api-openapi.yml
  format: yaml
  label: KonbiniAPI X API
  slug: konbiniapi-x-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/konbiniapi/refs/heads/main/openapi/konbiniapi-x-api-openapi.yml
- filename: konbiniapi-reddit-api-openapi.yml
  format: yaml
  label: KonbiniAPI Reddit API
  slug: konbiniapi-reddit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/konbiniapi/refs/heads/main/openapi/konbiniapi-reddit-api-openapi.yml
- filename: konbiniapi-linkedin-api-openapi.yml
  format: yaml
  label: KonbiniAPI LinkedIn API
  slug: konbiniapi-linkedin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/konbiniapi/refs/heads/main/openapi/konbiniapi-linkedin-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Konbiniapi Authentication
name_suffix: Authentication
oauth_flows: []
overview: KonbiniAPI secures its APIs with http and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: KonbiniAPI
provider_slug: konbiniapi
scheme_count: 3
schemes:
- applies_to: https://api.konbiniapi.com
  description: 'Send your API key in the Authorization header as a Bearer token.

    Example: `Authorization: Bearer <your-api-key>`'
  format: Bearer knbn_<key>
  global: true
  header: Authorization
  key_prefix: knbn_
  name: apiKey
  note: Declared as the sole global security requirement in the OpenAPI, so every one of the 67 operations requires it. One key per account; rotating the key does not reset the credit balance because credits are tied to the account. Revoked keys are rejected instantly.
  scheme: bearer
  sources:
  - openapi/_original/konbiniapi-openapi.json
  - https://docs.konbiniapi.com/getting-started/authentication
  surface: rest
  type: http
- applies_to: https://mcp.konbiniapi.com
  description: OAuth 2.1 authorization code + PKCE for the hosted MCP server, discoverable through RFC 9728 protected-resource metadata and RFC 8414 authorization-server metadata.
  dynamic_client_registration: true
  flows:
    authorizationCode:
      authorizationUrl: https://app.konbiniapi.com/api/auth/oauth2/authorize
      refreshUrl: https://app.konbiniapi.com/api/auth/oauth2/token
      scopes:
        api_key: Act on the account's KonbiniAPI API key on the user's behalf.
        offline_access: Receive a refresh token and act without the user present.
      tokenUrl: https://app.konbiniapi.com/api/auth/oauth2/token
    clientCredentials:
      tokenUrl: https://app.konbiniapi.com/api/auth/oauth2/token
  id_token_signing_alg: EdDSA
  introspection_endpoint: https://app.konbiniapi.com/api/auth/oauth2/introspect
  issuer: https://app.konbiniapi.com/api/auth
  jwks_uri: https://app.konbiniapi.com/api/auth/jwks
  name: mcpOAuth
  pkce:
  - S256
  registration_endpoint: https://app.konbiniapi.com/api/auth/oauth2/register
  revocation_endpoint: https://app.konbiniapi.com/api/auth/oauth2/revoke
  sources:
  - well-known/konbiniapi-mcp-oauth-protected-resource.json
  - well-known/konbiniapi-mcp-oauth-authorization-server.json
  surface: mcp
  type: oauth2
- applies_to: https://mcp.konbiniapi.com
  description: 'Fallback for MCP clients that support remote servers but not OAuth: send the KonbiniAPI API key as a Bearer token instead of completing the authorization flow.'
  name: mcpBearer
  scheme: bearer
  sources:
  - https://docs.konbiniapi.com/reference/mcp/overview
  surface: mcp
  type: http
slug: konbiniapi-authentication
source_filename: konbiniapi-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.konbiniapi.com/getting-started/authentication
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://docs.konbiniapi.com/getting-started/authentication\nsources:\n  - https://docs.konbiniapi.com/getting-started/authentication\n  - https://docs.konbiniapi.com/reference/mcp/overview\n  - https://mcp.konbiniapi.com/.well-known/oauth-protected-resource\n  - https://mcp.konbiniapi.com/.well-known/oauth-authorization-server\n  - openapi/_original/konbiniapi-openapi.json\nnote: >-\n  KonbiniAPI runs two distinct authentication surfaces. The REST API takes a single static Bearer\n  API key and nothing else. The hosted MCP server takes OAuth 2.1, and accepts the same Bearer API\n  key as a fallback for clients that cannot do the browser flow. The OpenAPI declares only the\n  first, so a spec-only read of this provider understates its auth posture.\nsummary:\n  types:\n    - http\n    - oauth2\n  surfaces: 2\nschemes:\n  - name: apiKey\n    type: http\n    scheme: bearer\n    surface: rest\n    applies_to: https://api.konbiniapi.com\n\
  \    header: Authorization\n    format: 'Bearer knbn_<key>'\n    key_prefix: knbn_\n    description: |-\n      Send your API key in the Authorization header as a Bearer token.\n      Example: `Authorization: Bearer <your-api-key>`\n    global: true\n    note: >-\n      Declared as the sole global security requirement in the OpenAPI, so every one of the 67\n      operations requires it. One key per account; rotating the key does not reset the credit\n      balance because credits are tied to the account. Revoked keys are rejected instantly.\n    sources:\n      - openapi/_original/konbiniapi-openapi.json\n      - https://docs.konbiniapi.com/getting-started/authentication\n  - name: mcpOAuth\n    type: oauth2\n    surface: mcp\n    applies_to: https://mcp.konbiniapi.com\n    flows:\n      authorizationCode:\n        authorizationUrl: https://app.konbiniapi.com/api/auth/oauth2/authorize\n        tokenUrl: https://app.konbiniapi.com/api/auth/oauth2/token\n        refreshUrl: https://app.konbiniapi.com/api/auth/oauth2/token\n\
  \        scopes:\n          api_key: Act on the account's KonbiniAPI API key on the user's behalf.\n          offline_access: Receive a refresh token and act without the user present.\n      clientCredentials:\n        tokenUrl: https://app.konbiniapi.com/api/auth/oauth2/token\n    issuer: https://app.konbiniapi.com/api/auth\n    jwks_uri: https://app.konbiniapi.com/api/auth/jwks\n    registration_endpoint: https://app.konbiniapi.com/api/auth/oauth2/register\n    introspection_endpoint: https://app.konbiniapi.com/api/auth/oauth2/introspect\n    revocation_endpoint: https://app.konbiniapi.com/api/auth/oauth2/revoke\n    pkce: ['S256']\n    dynamic_client_registration: true\n    id_token_signing_alg: EdDSA\n    description: >-\n      OAuth 2.1 authorization code + PKCE for the hosted MCP server, discoverable through RFC 9728\n      protected-resource metadata and RFC 8414 authorization-server metadata.\n    sources:\n      - well-known/konbiniapi-mcp-oauth-protected-resource.json\n     \
  \ - well-known/konbiniapi-mcp-oauth-authorization-server.json\n  - name: mcpBearer\n    type: http\n    scheme: bearer\n    surface: mcp\n    applies_to: https://mcp.konbiniapi.com\n    description: >-\n      Fallback for MCP clients that support remote servers but not OAuth: send the KonbiniAPI API\n      key as a Bearer token instead of completing the authorization flow.\n    sources:\n      - https://docs.konbiniapi.com/reference/mcp/overview\nidentity_providers:\n  - Email and password\n  - Google\n  - GitHub\nscopes: scopes/konbiniapi-scopes.yml\nfailure_modes:\n  - status: 401\n    code: missing_api_key\n    meaning: Authorization header absent or malformed.\n  - status: 401\n    code: invalid_api_key\n    meaning: Key not recognised or revoked.\n  - status: 403\n    code: api_key_disabled\n    meaning: Key exists but is disabled.\n  - status: 403\n    code: api_key_expired\n    meaning: Key exists but is expired.\nobserved:\n  - url: https://api.konbiniapi.com/v1/openapi.json\n\
  \    http_status: 401\n    note: unauthenticated request returns missing_api_key, confirming the key is enforced at the edge\n  - url: https://mcp.konbiniapi.com/\n    http_status: 401\n    note: 'anonymous MCP tools/list returns {\"code\":-32000,\"message\":\"Unauthorized\"}'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/konbiniapi/refs/heads/main/authentication/konbiniapi-authentication.yml
summary_line: http/oauth2 · 3 schemes
tags:
- Social-Media
- Instagram
- TikTok
- X
- Reddit
- LinkedIn
- ActivityStreams 2.0
- Scraping
- Data Extraction
- Public Data
- Influencer Marketing
- Social Listening
- Creator Tools
- MCP
- Agent Skills
- Agents
---
