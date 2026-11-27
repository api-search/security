---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: coret.id Authentication
name_suffix: Authentication
oauth_flows: []
overview: coret.id declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: coret.id
provider_slug: coret-id
scheme_count: 2
schemes:
- description: 'All endpoints except GET /api/v1/SKILL.md and GET /api/v1/share/* require "Authorization: Bearer crt_live_<64_hex_chars>". Workspace admins create API keys in the dashboard; keys carry the prefix crt_live_ (production) or crt_test_ (sandbox) and are scoped (see scopes/).'
  key_prefixes:
  - crt_live_
  - crt_test_
  name: bearerApiKey
  scheme: bearer
  type: http
- authorization_url: https://coret.id/app/oauth/authorize
  description: For clients that cannot send headers (Claude custom connector, Claude Cowork), mcp.coret.id supports OAuth 2.1 authorization code + PKCE with dynamic client registration; the access token returned is a new crt_live_ API key in the chosen workspace.
  discovery:
  - https://mcp.coret.id/.well-known/oauth-protected-resource
  - https://mcp.coret.id/.well-known/oauth-authorization-server
  flow: authorization_code + PKCE (OAuth 2.1)
  name: mcpOAuth
  note: Revocation follows RFC 7009 and always answers 200 with an empty body. Redirects are allowed to claude.ai, claude.com, anthropic.com, cursor.com, grok.com, x.ai, chatgpt.com, vscode.dev and localhost. Documented only; not called by this pipeline.
  registration_url: https://coret.id/api/oauth/register
  revocation_url: https://coret.id/api/oauth/revoke
  token_url: https://coret.id/api/oauth/token
  type: oauth2
slug: coret-id-authentication
source_filename: coret-id-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://coret.id/api/v1/SKILL.md\ndocs: https://coret.id/api/v1/SKILL.md\nschemes:\n- name: bearerApiKey\n  type: http\n  scheme: bearer\n  description: 'All endpoints except GET /api/v1/SKILL.md and GET /api/v1/share/* require \"Authorization: Bearer crt_live_<64_hex_chars>\". Workspace admins create API keys in the dashboard; keys carry the prefix crt_live_ (production) or crt_test_ (sandbox) and are scoped (see scopes/).'\n  key_prefixes: [crt_live_, crt_test_]\n- name: mcpOAuth\n  type: oauth2\n  flow: authorization_code + PKCE (OAuth 2.1)\n  description: For clients that cannot send headers (Claude custom connector, Claude Cowork), mcp.coret.id supports OAuth 2.1 authorization code + PKCE with dynamic client registration; the access token returned is a new crt_live_ API key in the chosen workspace.\n  authorization_url: https://coret.id/app/oauth/authorize\n  token_url: https://coret.id/api/oauth/token\n  registration_url:\
  \ https://coret.id/api/oauth/register\n  revocation_url: https://coret.id/api/oauth/revoke\n  discovery:\n  - https://mcp.coret.id/.well-known/oauth-protected-resource\n  - https://mcp.coret.id/.well-known/oauth-authorization-server\n  note: Revocation follows RFC 7009 and always answers 200 with an empty body. Redirects are allowed to claude.ai, claude.com, anthropic.com, cursor.com, grok.com, x.ai, chatgpt.com, vscode.dev and localhost. Documented only; not called by this pipeline.\n"
source_yaml_url: https://artifacts.apis.io/coret-id/authentication/coret-id-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Mind Mapping
- Collaboration
- Productivity
- AI Agents
- MCP
- Indonesia
---
