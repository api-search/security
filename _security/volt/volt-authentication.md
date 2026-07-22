---
api_key_in:
- header
auth_types:
- oauth2
- http
description: ''
kind: authentication
layout: security
method: searched
name: Volt Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Volt secures its APIs with oauth2 and http across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Volt
provider_slug: volt
scheme_count: 2
schemes:
- applies_to: mcp.voltchat.com
  description: OAuth-based custom connector supported natively in Claude and ChatGPT — no API key or config file required.
  name: OAuth Custom Connector
  sources:
  - https://voltchat.com/docs/mcp/setup-instructions
  type: oauth2
- applies_to: mcp.voltchat.com
  description: Personal Volt API key sent as an HTTP Bearer token, used with the mcp-remote module for MCP clients without native remote support.
  format: 'Authorization: Bearer YOUR_VOLT_API_KEY'
  in: header
  name: Volt API Key (Bearer)
  parameter: Authorization
  scheme: bearer
  sources:
  - https://voltchat.com/docs/mcp/setup-instructions
  type: http
slug: volt-authentication
source_filename: volt-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://voltchat.com/docs/mcp/setup-instructions\ndocs: https://voltchat.com/docs/mcp/setup-instructions\nnote: >-\n  Volt publishes no public REST API/OpenAPI. Its only programmatic surface is the\n  authenticated remote MCP server (https://mcp.voltchat.com/mcp). Authentication\n  below is derived from the MCP setup docs, not an OpenAPI spec.\nsummary:\n  types: [oauth2, http]\n  api_key_in: [header]\n  oauth2_flows: [authorizationCode]\nschemes:\n- name: OAuth Custom Connector\n  type: oauth2\n  applies_to: mcp.voltchat.com\n  description: >-\n    OAuth-based custom connector supported natively in Claude and ChatGPT — no\n    API key or config file required.\n  sources: [https://voltchat.com/docs/mcp/setup-instructions]\n- name: Volt API Key (Bearer)\n  type: http\n  scheme: bearer\n  in: header\n  parameter: Authorization\n  format: 'Authorization: Bearer YOUR_VOLT_API_KEY'\n  applies_to: mcp.voltchat.com\n  description:\
  \ >-\n    Personal Volt API key sent as an HTTP Bearer token, used with the mcp-remote\n    module for MCP clients without native remote support.\n  sources: [https://voltchat.com/docs/mcp/setup-instructions]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/volt/refs/heads/main/authentication/volt-authentication.yml
summary_line: oauth2/http · 2 schemes
tags:
- Company
- WhatsApp
- Messaging
- Productivity
- MCP
- AI Agents
- Sales
- Communication
---
