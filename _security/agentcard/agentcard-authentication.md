---
api_key_in: []
api_specs:
- filename: agentcard-openapi-original.json
  format: json
  label: Agentcard v2 API
  slug: agentcard-v2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agentcard/refs/heads/main/openapi/agentcard-openapi-original.json
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Agentcard Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
- authorizationCode
overview: Agentcard secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials and authorizationCode flow(s).
provider_name: Agentcard
provider_slug: agentcard
scheme_count: 2
schemes:
- description: 'Platform access token for the REST v2 API. Mint it via POST /api/v2/oauth/token by exchanging client_id + client_secret (OAuth2 client credentials, RFC 6749 §4.4). Send as Authorization: Bearer <token>. Tokens live one hour; no refresh token on this grant — re-mint.'
  name: platformToken
  scheme: bearer
  sources:
  - openapi/agentcard-openapi-original.json
  type: http
- authorization_endpoint: https://mcp.agentcard.sh/authorize
  authorization_server: https://mcp.agentcard.sh
  description: '"Connect with Agentcard" — OAuth 2.1 + PKCE for end-user authorization to the hosted MCP server. Confidential clients get an acs_ secret; public (PKCE-only) clients omit it. Discoverable via /.well-known/oauth-authorization-server and /.well-known/oauth-protected-resource.'
  flow: authorizationCode
  name: connectWithAgentcard
  pkce: required
  refresh: rotating
  registration_endpoint: https://mcp.agentcard.sh/register
  resource: https://mcp.agentcard.sh/mcp
  revocation_endpoint: https://mcp.agentcard.sh/revoke
  sources:
  - https://mcp.agentcard.sh/.well-known/oauth-authorization-server
  - https://docs.agentcard.sh/companies/authentication/oauth
  token_endpoint: https://mcp.agentcard.sh/token
  type: oauth2
slug: agentcard-authentication
source_filename: agentcard-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: searched\nsource: openapi/agentcard-openapi-original.json + https://docs.agentcard.sh/companies/authentication/oauth + https://mcp.agentcard.sh/.well-known/oauth-authorization-server\ndocs: https://docs.agentcard.sh/companies/api/user-authentication\nsummary:\n  types: [http, oauth2]\n  http_schemes: [bearer]\n  oauth2_flows: [clientCredentials, authorizationCode]\nschemes:\n- name: platformToken\n  type: http\n  scheme: bearer\n  description: >-\n    Platform access token for the REST v2 API. Mint it via POST /api/v2/oauth/token by\n    exchanging client_id + client_secret (OAuth2 client credentials, RFC 6749 §4.4). Send as\n    Authorization: Bearer <token>. Tokens live one hour; no refresh token on this grant — re-mint.\n  sources: [openapi/agentcard-openapi-original.json]\n- name: connectWithAgentcard\n  type: oauth2\n  flow: authorizationCode\n  pkce: required   # S256, enforced for every client including confidential\n  authorization_server:\
  \ https://mcp.agentcard.sh\n  authorization_endpoint: https://mcp.agentcard.sh/authorize\n  token_endpoint: https://mcp.agentcard.sh/token\n  registration_endpoint: https://mcp.agentcard.sh/register\n  revocation_endpoint: https://mcp.agentcard.sh/revoke\n  resource: https://mcp.agentcard.sh/mcp   # audience-bound, sent on /authorize and /token\n  refresh: rotating   # refresh tokens rotate on every refresh — persist the new one\n  description: >-\n    \"Connect with Agentcard\" — OAuth 2.1 + PKCE for end-user authorization to the hosted MCP\n    server. Confidential clients get an acs_ secret; public (PKCE-only) clients omit it.\n    Discoverable via /.well-known/oauth-authorization-server and /.well-known/oauth-protected-resource.\n  sources: [https://mcp.agentcard.sh/.well-known/oauth-authorization-server, https://docs.agentcard.sh/companies/authentication/oauth]\nnotes: >-\n  The REST spec declares only the platformToken bearer scheme; the OAuth 2.1 + PKCE end-user\n  flow is documented\
  \ in the Companies auth docs and the MCP authorization-server metadata.\n  A headless phone-authentication path exists for messaging agents with no browser moment.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/agentcard/refs/heads/main/authentication/agentcard-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Company
- Payments
- Virtual Cards
- Card Issuing
- AI Agents
- Agentic Commerce
- MCP
- Fintech
- Wallet
- Visa
---
