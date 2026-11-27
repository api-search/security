---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: ClipEmber Authentication
name_suffix: Authentication
oauth_flows: []
overview: ClipEmber declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: ClipEmber
provider_slug: clipember-com
scheme_count: 2
schemes:
- description: Create a key in the app (or via POST /api/v1/keys with a session) and pass it as X-API-Key. The secret is shown once; we store only a hash.
  header: X-API-Key
  in: header
  key_prefix: cf_
  name: ApiKeyAuth
  plan_requirement: Issuing new API keys needs Pro or Agency (https://clipember.com/pricing).
  type: apiKey
- applies_to: MCP server only (https://clipember.com/api/mcp)
  description: OAuth 2.1 + dynamic client registration for chat clients (Claude.ai, ChatGPT, Claude Code); local MCP clients use an X-API-Key header instead.
  docs: https://clipember.com/mcp
  name: McpOAuth
  note: The OAuth flow is documented on the MCP page only; no scopes are published.
  type: oauth2
slug: clipember-com-authentication
source_filename: clipember-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://clipember.com/docs\ndocs: https://clipember.com/docs\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  header: X-API-Key\n  key_prefix: cf_\n  description: 'Create a key in the app (or via POST /api/v1/keys with a session) and pass it as X-API-Key. The secret is shown once; we store only a hash.'\n  plan_requirement: 'Issuing new API keys needs Pro or Agency (https://clipember.com/pricing).'\n- name: McpOAuth\n  type: oauth2\n  applies_to: MCP server only (https://clipember.com/api/mcp)\n  description: 'OAuth 2.1 + dynamic client registration for chat clients (Claude.ai, ChatGPT, Claude Code); local MCP clients use an X-API-Key header instead.'\n  docs: https://clipember.com/mcp\n  note: 'The OAuth flow is documented on the MCP page only; no scopes are published.'\n"
source_yaml_url: https://artifacts.apis.io/clipember-com/authentication/clipember-com-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Video
- Artificial Intelligence
- Video Editing
- Short-Form Video
- Captions
- Social Media
- MCP
---
