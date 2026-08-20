---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Raindrop Authentication
name_suffix: Authentication
oauth_flows: []
overview: Raindrop declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: Raindrop
provider_slug: raindrop
scheme_count: 3
schemes:
- applies_to: https://api.raindrop.ai/v1
  format: Bearer <WRITE_KEY>
  header: Authorization
  in: header
  name: ingest_write_key
  note: Write/ingest key for /events/track, /signals/track, /users/identify.
  scheme: bearer
  type: http
- applies_to: https://query.raindrop.ai/v1
  format: Bearer <QUERY_API_KEY>
  header: Authorization
  in: header
  name: query_api_key
  note: Read-only query key for the Query API.
  scheme: bearer
  type: http
- applies_to: MCP server (OAuth 2.1) and dashboard sign-in.
  authorization_endpoint: https://auth.raindrop.ai/propelauth/oauth/authorize
  grant_types:
  - authorization_code
  issuer: https://auth.raindrop.ai
  name: propelauth_oidc
  openid_configuration: https://auth.raindrop.ai/.well-known/openid-configuration
  pkce:
  - S256
  scopes:
  - openid
  - email
  - profile
  token_endpoint: https://auth.raindrop.ai/propelauth/oauth/token
  type: openIdConnect
  userinfo_endpoint: https://auth.raindrop.ai/propelauth/oauth/userinfo
slug: raindrop-authentication
source_filename: raindrop-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: >-\n  raindrop.ai/docs/sdk/http-api, raindrop.ai/docs/query-api/api-reference,\n  raindrop.ai/docs/mcp/overview, and auth.raindrop.ai OpenID configuration.\nsummary: >-\n  Raindrop's ingest and query APIs authenticate with bearer API keys issued\n  from app.raindrop.ai. The MCP server and dashboard additionally support\n  OAuth 2.1 / OpenID Connect via PropelAuth (auth.raindrop.ai).\nschemes:\n- name: ingest_write_key\n  type: http\n  scheme: bearer\n  in: header\n  header: Authorization\n  format: 'Bearer <WRITE_KEY>'\n  applies_to: https://api.raindrop.ai/v1\n  note: Write/ingest key for /events/track, /signals/track, /users/identify.\n- name: query_api_key\n  type: http\n  scheme: bearer\n  in: header\n  header: Authorization\n  format: 'Bearer <QUERY_API_KEY>'\n  applies_to: https://query.raindrop.ai/v1\n  note: Read-only query key for the Query API.\n- name: propelauth_oidc\n  type: openIdConnect\n  issuer: https://auth.raindrop.ai\n\
  \  openid_configuration: https://auth.raindrop.ai/.well-known/openid-configuration\n  authorization_endpoint: https://auth.raindrop.ai/propelauth/oauth/authorize\n  token_endpoint: https://auth.raindrop.ai/propelauth/oauth/token\n  userinfo_endpoint: https://auth.raindrop.ai/propelauth/oauth/userinfo\n  grant_types: [authorization_code]\n  pkce: [S256]\n  scopes: [openid, email, profile]\n  applies_to: MCP server (OAuth 2.1) and dashboard sign-in.\nproject_scoping:\n  header: X-Raindrop-Project-Id\n  default: Production\n  note: Optional header to target a specific project on ingest and query calls.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/raindrop/refs/heads/main/authentication/raindrop-authentication.yml
summary_line: 3 schemes
tags:
- Company
- Artificial Intelligence
- Agents
- Observability
- Monitoring
- LLMOps
- Developer Tools
- Tracing
---
