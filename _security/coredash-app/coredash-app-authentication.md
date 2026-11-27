---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: CoreDash Authentication
name_suffix: Authentication
oauth_flows: []
overview: CoreDash declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: CoreDash
provider_slug: coredash-app
scheme_count: 3
schemes:
- description: Keys start with cdk_ and are scoped to a single project. Created in the app under the project, AI Insights, Connect Your AI; shown once, stored as a SHA-256 hash, revocable; only project owners can manage keys. Used for the JSON-RPC data endpoint, uptime endpoints and the releases (CI/CD) endpoints.
  header: 'Authorization: Bearer cdk_YOUR_API_KEY'
  name: projectKey
  prefix: cdk_
  scheme: bearer
  scope: one project
  type: http
- description: Agency-flagged accounts only; minted at My Account > Agency API tab. Required for /api/agency/projects REST CRUD; also reads data for any owned project by passing project_id to the JSON-RPC tools.
  header: 'Authorization: Bearer cdk_master_YOUR_MASTER_KEY'
  name: masterKey
  prefix: cdk_master_
  scheme: bearer
  scope: every project on the account
  type: http
- authorization_server: https://app.coredash.app
  description: Used by MCP clients (Claude connector, Claude Code browser login). 1-hour access token, 30-day refresh. Read-only - a POST, PATCH or DELETE with an OAuth token gets 403 "This token can only read."
  dynamic_client_registration: true
  evidence:
  - https://app.coredash.app/.well-known/oauth-protected-resource (HTTP 200, scopes_supported [mcp:read])
  - https://app.coredash.app/.well-known/oauth-authorization-server (HTTP 200, grant_types authorization_code+refresh_token, S256, token_endpoint_auth_methods none, registration_endpoint present)
  flow: authorizationCode
  name: mcpOAuth
  pkce: S256
  scopes:
  - mcp:read
  token_prefix: mcp_at_
  type: oauth2
slug: coredash-app-authentication
source_filename: coredash-app-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "name: CoreDash authentication\ngenerated: '2026-11-04'\nmethod: searched\nsource: https://www.coredash.app/api\ndocs: https://www.coredash.app/api\nschemes:\n- name: projectKey\n  type: http\n  scheme: bearer\n  header: 'Authorization: Bearer cdk_YOUR_API_KEY'\n  prefix: cdk_\n  scope: one project\n  description: Keys start with cdk_ and are scoped to a single project. Created in the app under the project, AI Insights, Connect Your AI; shown once, stored as a SHA-256 hash, revocable; only project\n    owners can manage keys. Used for the JSON-RPC data endpoint, uptime endpoints and the releases (CI/CD) endpoints.\n- name: masterKey\n  type: http\n  scheme: bearer\n  header: 'Authorization: Bearer cdk_master_YOUR_MASTER_KEY'\n  prefix: cdk_master_\n  scope: every project on the account\n  description: Agency-flagged accounts only; minted at My Account > Agency API tab. Required for /api/agency/projects REST CRUD; also reads data for any owned project by passing project_id to\
  \ the JSON-RPC\n    tools.\n- name: mcpOAuth\n  type: oauth2\n  flow: authorizationCode\n  pkce: S256\n  token_prefix: mcp_at_\n  authorization_server: https://app.coredash.app\n  scopes:\n  - mcp:read\n  dynamic_client_registration: true\n  description: Used by MCP clients (Claude connector, Claude Code browser login). 1-hour access token, 30-day refresh. Read-only - a POST, PATCH or DELETE with an OAuth token gets 403 \"This token can only\n    read.\"\n  evidence:\n  - https://app.coredash.app/.well-known/oauth-protected-resource (HTTP 200, scopes_supported [mcp:read])\n  - https://app.coredash.app/.well-known/oauth-authorization-server (HTTP 200, grant_types authorization_code+refresh_token, S256, token_endpoint_auth_methods none, registration_endpoint present)\ndocs_pages:\n- https://www.coredash.app/api/agency\n- https://www.coredash.app/api/uptime\n- https://www.coredash.app/core-web-vitals-mcp-server\n"
source_yaml_url: https://artifacts.apis.io/coredash-app/authentication/coredash-app-authentication.yml
summary_line: 3 schemes
tags:
- Company
- Core Web Vitals
- Real User Monitoring
- Web Performance
- Observability
- MCP
- JSON-RPC
- AI Agents
---
