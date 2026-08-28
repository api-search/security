---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Moz Authentication
name_suffix: Authentication
oauth_flows: []
overview: Moz declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: Moz
provider_slug: moz
scheme_count: 3
schemes:
- applies_to:
  - https://api.moz.com/jsonrpc
  description: A secret Moz API token issued from the Moz API dashboard. Sent on every POST to the universal JSON-RPC endpoint. Not to be confused with the JSON-RPC "id" field, which is a client-generated request identifier and must be at least 24 characters long.
  id: moz-api-token
  in: header
  issuance:
    dashboard: https://moz.com/api/dashboard
    max_active_tokens: 5
    rotation: Tokens can be deleted after creation; deleting a token immediately breaks any code still using it. Moz documents no automatic expiry or rotation schedule.
    signup_requirement: A separate API subscription is required (distinct from Moz Pro). The free tier requires a valid, non-expired credit card, which is not charged unless the account is upgraded.
  name: x-moz-token
  type: apiKey
- applies_to:
  - https://api.moz.com/mcp/v1/data
  - https://api.moz.com/mcp/v1/local
  authorization_endpoint: https://api.moz.com/oauth/authorize
  authorization_server: https://api.moz.com
  code_challenge_methods_supported:
  - S256
  description: Recommended path for MCP clients. The client walks the user through OAuth sign-in; Moz publishes RFC 8414 authorization-server metadata and RFC 9728 protected-resource metadata per endpoint.
  flow: authorization_code
  grant_types_supported:
  - authorization_code
  id: moz-mcp-oauth
  metadata_documents:
  - well-known/moz-api-oauth-authorization-server.json
  - well-known/moz-api-oauth-protected-resource-mcp-data.json
  - well-known/moz-api-oauth-protected-resource-mcp-local.json
  registration_endpoint: https://api.moz.com/oauth/register
  response_types_supported:
  - code
  scopes_supported:
  - mcp
  token_endpoint: https://api.moz.com/oauth/token
  token_endpoint_auth_methods_supported:
  - none
  type: oauth2
- applies_to:
  - https://api.moz.com/mcp/v1/data
  - https://api.moz.com/mcp/v1/local
  bearer_methods_supported:
  - header
  description: Manual alternative for clients without OAuth support. The bearer value is the same Moz API key used for x-moz-token on the JSON-RPC API; the one token works against both MCP endpoints.
  header: 'Authorization: Bearer <YOUR_MOZ_TOKEN>'
  id: moz-mcp-bearer
  scheme: bearer
  type: http
slug: moz-authentication
source_filename: moz-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: searched\nsource: https://moz.com/api/docs/guides/authentication\ndocs: https://moz.com/api/docs/guides/authentication\nsummary: >-\n  Moz runs two distinct authentication models. The JSON-RPC data API uses a static secret API token\n  in a custom x-moz-token header. The two beta MCP endpoints use OAuth 2.1 (authorization code +\n  PKCE, with dynamic client registration) and also accept the same Moz API token as an HTTP Bearer.\n  There is no OpenID Connect surface: /.well-known/openid-configuration 404s on both hosts.\nschemes:\n- id: moz-api-token\n  type: apiKey\n  in: header\n  name: x-moz-token\n  applies_to:\n  - https://api.moz.com/jsonrpc\n  description: >-\n    A secret Moz API token issued from the Moz API dashboard. Sent on every POST to the universal\n    JSON-RPC endpoint. Not to be confused with the JSON-RPC \"id\" field, which is a client-generated\n    request identifier and must be at least 24 characters long.\n  issuance:\n\
  \    dashboard: https://moz.com/api/dashboard\n    max_active_tokens: 5\n    rotation: >-\n      Tokens can be deleted after creation; deleting a token immediately breaks any code still using\n      it. Moz documents no automatic expiry or rotation schedule.\n    signup_requirement: >-\n      A separate API subscription is required (distinct from Moz Pro). The free tier requires a\n      valid, non-expired credit card, which is not charged unless the account is upgraded.\n- id: moz-mcp-oauth\n  type: oauth2\n  flow: authorization_code\n  applies_to:\n  - https://api.moz.com/mcp/v1/data\n  - https://api.moz.com/mcp/v1/local\n  description: >-\n    Recommended path for MCP clients. The client walks the user through OAuth sign-in; Moz publishes\n    RFC 8414 authorization-server metadata and RFC 9728 protected-resource metadata per endpoint.\n  authorization_server: https://api.moz.com\n  authorization_endpoint: https://api.moz.com/oauth/authorize\n  token_endpoint: https://api.moz.com/oauth/token\n\
  \  registration_endpoint: https://api.moz.com/oauth/register\n  response_types_supported: [code]\n  grant_types_supported: [authorization_code]\n  code_challenge_methods_supported: [S256]\n  token_endpoint_auth_methods_supported: [none]\n  scopes_supported: [mcp]\n  metadata_documents:\n  - well-known/moz-api-oauth-authorization-server.json\n  - well-known/moz-api-oauth-protected-resource-mcp-data.json\n  - well-known/moz-api-oauth-protected-resource-mcp-local.json\n- id: moz-mcp-bearer\n  type: http\n  scheme: bearer\n  applies_to:\n  - https://api.moz.com/mcp/v1/data\n  - https://api.moz.com/mcp/v1/local\n  description: >-\n    Manual alternative for clients without OAuth support. The bearer value is the same Moz API key\n    used for x-moz-token on the JSON-RPC API; the one token works against both MCP endpoints.\n  header: 'Authorization: Bearer <YOUR_MOZ_TOKEN>'\n  bearer_methods_supported: [header]\nmutual_tls: false\nopenid_connect: false\nobservations:\n- >-\n  The MCP endpoints\
  \ return a spec-correct 401 with a WWW-Authenticate Bearer challenge carrying a\n  resource_metadata parameter, which is the RFC 9728 behaviour MCP clients need for automatic OAuth\n  discovery. Probed 2026-08-26.\n- >-\n  token_endpoint_auth_methods_supported is [\"none\"], i.e. public clients with PKCE; combined with an\n  open registration_endpoint this is the standard MCP client-onboarding shape.\n- >-\n  The JSON-RPC API has no OAuth path and no scopes; authorization is entirely plan-based (which\n  methods a token can call is decided by the subscription tier, not by a scope grant).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/moz/refs/heads/main/authentication/moz-authentication.yml
summary_line: 3 schemes
tags:
- SEO
- Search
- Marketing
- Analytics
- Keywords
- Backlinks
- Local Marketing
- Domain Authority
- Link Index
- JSON-RPC
- MCP
- Company
---
