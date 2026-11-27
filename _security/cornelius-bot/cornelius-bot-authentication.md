---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Cornelius Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cornelius declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Cornelius
provider_slug: cornelius-bot
scheme_count: 1
schemes:
- authorization_server: https://neat-labyrinth-49-staging.authkit.app
  bearer_methods:
  - header
  evidence:
  - quote: Sign-in. OAuth with PKCE, run by WorkOS AuthKit. Claude identifies itself with its published client identity, and every token is bound to the Cornelius server (resource indicators).
    url: https://cornelius.bot/teams
  - http_status: 200
    note: Protected-resource metadata lists authorization_servers ["https://neat-labyrinth-49-staging.authkit.app"] and bearer_methods_supported ["header"]. The AuthKit host name contains "staging".
    url: https://mcp.cornelius.bot/.well-known/oauth-protected-resource
  flow: authorizationCode
  name: oauth2-authkit
  pkce: true
  provider: WorkOS AuthKit
  resource: https://mcp.cornelius.bot/mcp
  resource_indicators: true
  scopes:
  - openid
  - profile
  - email
  - offline_access
  type: oauth2
slug: cornelius-bot-authentication
source_filename: cornelius-bot-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://cornelius.bot/teams\ndocs: https://cornelius.bot/teams\nname: Cornelius authentication\nschemes:\n- name: oauth2-authkit\n  type: oauth2\n  flow: authorizationCode\n  pkce: true\n  authorization_server: https://neat-labyrinth-49-staging.authkit.app\n  provider: WorkOS AuthKit\n  bearer_methods: [header]\n  resource: https://mcp.cornelius.bot/mcp\n  resource_indicators: true\n  scopes: [openid, profile, email, offline_access]\n  evidence:\n  - url: https://cornelius.bot/teams\n    quote: \"Sign-in. OAuth with PKCE, run by WorkOS AuthKit. Claude identifies itself with its published client identity, and every token is bound to the Cornelius server (resource indicators).\"\n  - url: https://mcp.cornelius.bot/.well-known/oauth-protected-resource\n    http_status: 200\n    note: 'Protected-resource metadata lists authorization_servers [\"https://neat-labyrinth-49-staging.authkit.app\"] and bearer_methods_supported [\"header\"\
  ]. The AuthKit host name contains \"staging\".'\napi_keys: false\nnotes: \"Docs state: \\\"No API keys or shared secrets exist, and tokens are never written to logs.\\\" and \\\"The token is verified on each request; the server keeps no session.\\\" No OpenAPI exists, so nothing was derived from a contract.\"\n"
source_yaml_url: https://artifacts.apis.io/cornelius-bot/authentication/cornelius-bot-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Artificial Intelligence
- AI Agents
- Personal Assistant
- MCP
- Knowledge Graph
- Productivity
---
