---
api_key_in:
- header
auth_types:
- apiKey
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Apstal Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- refreshToken
overview: Apstal secures its APIs with apiKey, http, and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and refreshToken flow(s).
provider_name: Apstal
provider_slug: apstal
scheme_count: 3
schemes:
- applies_to:
  - https://apstal.com/api/mcp
  - https://apstal.com/api/analytics/*
  - https://apstal.com/api/ai/semantic
  format: Bearer apstal_<key>
  in: header
  issuance: Dashboard -> Settings -> API Keys (also Settings -> MCP Server for the MCP key)
  name: apiKeyBearer
  parameter: Authorization
  programmatic_issuance:
  - 'MCP tool: login (email + password) returns an API key'
  - 'MCP tool: generate_api_key (authenticated) mints additional keys'
  sources:
  - https://apstal.com/auth.md
  - https://apstal.com/docs/api
  - https://apstal.com/docs/mcp
  type: apiKey
- bearerFormat: JWT
  description: Supabase session JWT, used by the dashboard and named by the published analytics-query Agent Skill as the credential for POST /api/ai/semantic.
  name: supabaseSession
  scheme: bearer
  sources:
  - https://apstal.com/.well-known/agent-skills/analytics-query/SKILL.md
  - https://apstal.com/docs/api
  type: http
- flows:
  - authorizationUrl: https://apstal.com/api/auth/callback
    flow: authorizationCode
    scopes:
    - read
    - write
    - admin
    tokenUrl: https://apstal.com/api/auth/token
  - flow: refreshToken
  id_token_signing_alg_values_supported:
  - RS256
  jwks_note: The authorization-server metadata advertises a jwks_uri that returns 404. Token signature verification cannot be completed from published material.
  jwks_status: 404
  jwks_uri: https://apstal.com/.well-known/jwks.json
  name: oauth2
  sources:
  - https://apstal.com/.well-known/oauth-authorization-server
  - https://apstal.com/auth.md
  token_endpoint_auth_methods_supported:
  - client_secret_basic
  - client_secret_post
  type: oauth2
slug: apstal-authentication
source_filename: apstal-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://apstal.com/auth.md\ndocs:\n- https://apstal.com/auth.md\n- https://apstal.com/docs/api\n- https://apstal.com/docs/mcp\nprobed:\n- url: https://apstal.com/.well-known/oauth-authorization-server\n  http_status: 200\n- url: https://apstal.com/.well-known/oauth-protected-resource\n  http_status: 200\nnote: >-\n  Apstal publishes no OpenAPI, so this profile is not derived from securitySchemes. It is read\n  from the provider's own agent-facing auth.md, its API reference, and its live RFC 8414 /\n  RFC 9728 discovery documents. Identity is Supabase Auth (GoTrue).\nsummary:\n  types: [apiKey, http, oauth2]\n  api_key_in: [header]\n  api_key_prefix: apstal_\n  oauth2_flows: [authorizationCode, refreshToken]\n  identity_provider: Supabase Auth (GoTrue)\nschemes:\n- name: apiKeyBearer\n  type: apiKey\n  in: header\n  parameter: Authorization\n  format: 'Bearer apstal_<key>'\n  issuance: Dashboard -> Settings -> API Keys (also\
  \ Settings -> MCP Server for the MCP key)\n  programmatic_issuance:\n  - 'MCP tool: login (email + password) returns an API key'\n  - 'MCP tool: generate_api_key (authenticated) mints additional keys'\n  applies_to:\n  - https://apstal.com/api/mcp\n  - https://apstal.com/api/analytics/*\n  - https://apstal.com/api/ai/semantic\n  sources: [https://apstal.com/auth.md, https://apstal.com/docs/api, https://apstal.com/docs/mcp]\n- name: supabaseSession\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: >-\n    Supabase session JWT, used by the dashboard and named by the published analytics-query\n    Agent Skill as the credential for POST /api/ai/semantic.\n  sources: [https://apstal.com/.well-known/agent-skills/analytics-query/SKILL.md, https://apstal.com/docs/api]\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://apstal.com/api/auth/callback\n    tokenUrl: https://apstal.com/api/auth/token\n    scopes: [read, write, admin]\n\
  \  - flow: refreshToken\n  token_endpoint_auth_methods_supported: [client_secret_basic, client_secret_post]\n  id_token_signing_alg_values_supported: [RS256]\n  jwks_uri: https://apstal.com/.well-known/jwks.json\n  jwks_status: 404\n  jwks_note: >-\n    The authorization-server metadata advertises a jwks_uri that returns 404. Token signature\n    verification cannot be completed from published material.\n  sources: [https://apstal.com/.well-known/oauth-authorization-server, https://apstal.com/auth.md]\nprotected_resource:\n  resource: https://apstal.com/api\n  authorization_servers: [https://apstal.com/.well-known/oauth-authorization-server]\n  scopes_supported: [read, write, admin]\n  bearer_methods_supported: [header]\n  source: https://apstal.com/.well-known/oauth-protected-resource\nproject_scoping:\n  note: >-\n    Every read is additionally scoped by Project ID. Write endpoints (/api/v1/m, /api/v1/stream)\n    take projectId in the body rather than a credential; the ingestion layer\
  \ enforces a locked\n    tracker domain and rejects payloads from unauthorized origins with HTTP 403.\n  source: https://apstal.com/docs/privacy\nagent_auth:\n  register_uri: https://apstal.com/auth.md\n  signup: https://apstal.com/app/settings\n  methods:\n  - type: api_key\n    description: Register an account and generate an API key from the dashboard settings\n  skill: https://apstal.com/.well-known/agent-skills/analytics-query/SKILL.md\n  source: https://apstal.com/.well-known/oauth-authorization-server\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apstal/refs/heads/main/authentication/apstal-authentication.yml
summary_line: apiKey/http/oauth2 · 3 schemes
tags:
- Analytics
- Web Analytics
- Privacy
- Session Replay
- Heatmaps
- MCP
- agent-native
- Cookieless
- llms-txt
- BigQuery
- GDPR
- A2A
- Agent Skills
- Bot Detection
- Core Web Vitals
---
