---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: ConnectMachine Authentication
name_suffix: Authentication
oauth_flows: []
overview: ConnectMachine declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: ConnectMachine
provider_slug: connectmachine-ai
scheme_count: 3
schemes:
- description: 'Personal MCP key sent as "Authorization: Bearer YOUR_MCP_KEY" to https://mcp.connectmachine.ai/mcp. Keys are obtained at licenses.connectmachine.ai/mcp/auth (email code or Google); the docs state keys are managed by the backend and do not expire.'
  name: mcpKey
  scheme: bearer
  sources:
  - https://www.connectmachine.ai/docs/mcp/
  - https://www.connectmachine.ai/llms/mcp.md
  type: http
- description: The MCP server supports OAuth 2.0 with dynamic client registration and PKCE; clients sending no Authorization header run the standard MCP OAuth flow.
  name: mcpOAuth
  sources:
  - https://www.connectmachine.ai/docs/mcp/
  type: oauth2
- description: Native Zapier integration - "OAuth uses authorization code with S256 PKCE and automatic refresh." ConnectMachine stores only access-token identifiers and hashed refresh tokens.
  flows:
  - authorizationCode
  name: zapierOAuth
  sources:
  - https://www.connectmachine.ai/docs/#zapier-native
  type: oauth2
slug: connectmachine-ai-authentication
source_filename: connectmachine-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://www.connectmachine.ai/docs/mcp/\ndocs: https://www.connectmachine.ai/docs/\nsummary:\n  note: No public REST OpenAPI is published. Two documented credential paths exist - the MCP server (personal key or OAuth 2.0 with DCR and PKCE) and the native Zapier integration (OAuth authorization code with S256 PKCE and refresh).\nschemes:\n- name: mcpKey\n  type: http\n  scheme: bearer\n  description: 'Personal MCP key sent as \"Authorization: Bearer YOUR_MCP_KEY\" to https://mcp.connectmachine.ai/mcp. Keys are obtained at licenses.connectmachine.ai/mcp/auth (email code or Google); the docs state keys are managed by the backend and do not expire.'\n  sources:\n  - https://www.connectmachine.ai/docs/mcp/\n  - https://www.connectmachine.ai/llms/mcp.md\n- name: mcpOAuth\n  type: oauth2\n  description: The MCP server supports OAuth 2.0 with dynamic client registration and PKCE; clients sending no Authorization header run the standard\
  \ MCP OAuth flow.\n  sources:\n  - https://www.connectmachine.ai/docs/mcp/\n- name: zapierOAuth\n  type: oauth2\n  flows: [authorizationCode]\n  description: Native Zapier integration - \"OAuth uses authorization code with S256 PKCE and automatic refresh.\" ConnectMachine stores only access-token identifiers and hashed refresh tokens.\n  sources:\n  - https://www.connectmachine.ai/docs/#zapier-native\n"
source_yaml_url: https://artifacts.apis.io/connectmachine-ai/authentication/connectmachine-ai-authentication.yml
summary_line: 3 schemes
tags:
- Company
- Digital Business Cards
- Contact Management
- Business Card Scanner
- Networking
- Artificial Intelligence
- MCP
- CRM
---
