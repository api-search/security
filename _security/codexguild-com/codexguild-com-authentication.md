---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: CodexGuild Authentication
name_suffix: Authentication
oauth_flows: []
overview: CodexGuild declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: CodexGuild
provider_slug: codexguild-com
scheme_count: 3
schemes:
- description: 'Agent key sent as "Authorization: Bearer cgk_..." — preferred because every MCP client supports it. Used by coding agents, scripts and MCP clients, including the remote MCP endpoint.'
  format: cgk_<prefix>_<secret>
  header: Authorization
  in: header
  lifetime: until revoked
  name: agentKeyBearer
  preferred: true
  scheme: bearer
  type: http
- description: Alternative header carrying the same agent key.
  format: cgk_<prefix>_<secret>
  header: x-codexguild-key
  in: header
  name: agentKeyHeader
  type: apiKey
- bearerFormat: JWT
  description: Session token (JWT access + refresh) used only by the web dashboard; access 15 min, refresh 30 days. Account and agent management (/auth/*, /agents, /me/*, /billing/*) require it; an agent key on those endpoints gets 403 USER_SESSION_REQUIRED.
  name: dashboardSession
  scheme: bearer
  type: http
slug: codexguild-com-authentication
source_filename: codexguild-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://codexguild.com/docs/authentication\ndocs: https://codexguild.com/docs/authentication\nschemes:\n- name: agentKeyBearer\n  type: http\n  scheme: bearer\n  in: header\n  header: Authorization\n  format: cgk_<prefix>_<secret>\n  lifetime: until revoked\n  preferred: true\n  description: 'Agent key sent as \"Authorization: Bearer cgk_...\" — preferred because every MCP client supports it. Used by coding agents, scripts and MCP clients, including the remote MCP endpoint.'\n- name: agentKeyHeader\n  type: apiKey\n  in: header\n  header: x-codexguild-key\n  format: cgk_<prefix>_<secret>\n  description: 'Alternative header carrying the same agent key.'\n- name: dashboardSession\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: 'Session token (JWT access + refresh) used only by the web dashboard; access 15 min, refresh 30 days. Account and agent management (/auth/*, /agents, /me/*, /billing/*) require it;\
  \ an agent key on those endpoints gets 403 USER_SESSION_REQUIRED.'\npublic_endpoints: 'Some endpoints are public (no key), e.g. GET /setup, GET /start-here.md, GET /mcp-servers, GET /models, POST /lint/instructions, GET /health.'\nkey_storage: 'Only a SHA-256 hash of the key plus its short prefix is stored; the key cannot be shown again.'\nrotation: 'Dashboard → Agents → the agent → Revoke; the key stops working on the next request. Create a new agent and update CODEXGUILD_API_KEY.'\nguidance: 'One key per agent (per harness or machine); all agents on an account share one quota. Never put the key in a URL or query string.'\nerrors:\n- status: 401\n  code: UNAUTHORIZED\n  meaning: 'key missing, malformed or revoked'\n- status: 403\n  code: FORBIDDEN\n  meaning: 'key valid but action not allowed; USER_SESSION_REQUIRED when an agent key calls a dashboard-only endpoint'\n"
source_yaml_url: https://artifacts.apis.io/codexguild-com/authentication/codexguild-com-authentication.yml
summary_line: 3 schemes
tags:
- Company
- AI Coding Agents
- Agent Security
- MCP
- Software Supply Chain
- Package Security
- Developer Tools
- Agent Skills
---
