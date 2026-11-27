---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Council AI Authentication
name_suffix: Authentication
oauth_flows: []
overview: Council AI declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Council AI
provider_slug: council-ai-app
scheme_count: 2
schemes:
- applies_to: config-file MCP clients (Claude Desktop, Claude Code, Cursor, Windsurf)
  docs: https://council-ai.app/mcp
  format: Bearer csa_<token>
  header: Authorization
  in: header
  issued_at: Council Settings -> MCP tokens (https://council-ai.app/settings?tab=mcp)
  name: Personal Access Token
  quote: PATs can be revoked at any time and are scoped to your account only.
  revocable: true
  scheme: bearer
  type: http
- applies_to: connector-style MCP clients (ChatGPT, claude.ai)
  authorization_server: https://mcp.council-ai.app
  docs: https://council-ai.app/mcp
  name: OAuth 2.1
  quote: connector-style clients (ChatGPT, claude.ai) sign in over OAuth 2.1 with one approval click and never handle a token
  scopes:
  - mcp
  scopes_note: Authorization server and the `mcp` scope come from the MCP module's 2026-11-04 probe recorded in apis.yml, not from the docs page.
  type: oauth2
slug: council-ai-app-authentication
source_filename: council-ai-app-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://council-ai.app/mcp\ndocs: https://council-ai.app/mcp\nname: Council AI authentication\nnote: Council AI publishes no REST API or OpenAPI; authentication applies to the hosted MCP server at https://mcp.council-ai.app/mcp (Ultra tier). No securitySchemes exist to derive from.\nschemes:\n- name: Personal Access Token\n  type: http\n  scheme: bearer\n  in: header\n  header: Authorization\n  format: 'Bearer csa_<token>'\n  applies_to: config-file MCP clients (Claude Desktop, Claude Code, Cursor, Windsurf)\n  issued_at: Council Settings -> MCP tokens (https://council-ai.app/settings?tab=mcp)\n  revocable: true\n  quote: \"PATs can be revoked at any time and are scoped to your account only.\"\n  docs: https://council-ai.app/mcp\n- name: OAuth 2.1\n  type: oauth2\n  applies_to: connector-style MCP clients (ChatGPT, claude.ai)\n  quote: \"connector-style clients (ChatGPT, claude.ai) sign in over OAuth 2.1 with one approval click\
  \ and never handle a token\"\n  authorization_server: https://mcp.council-ai.app\n  scopes: [mcp]\n  scopes_note: Authorization server and the `mcp` scope come from the MCP module's 2026-11-04 probe recorded in apis.yml, not from the docs page.\n  docs: https://council-ai.app/mcp\n"
source_yaml_url: https://artifacts.apis.io/council-ai-app/authentication/council-ai-app-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Artificial Intelligence
- LLM
- Multi-Model
- MCP
- RAG
- Code Review
- Consensus
---
