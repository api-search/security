---
anonymous_access: true
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 0
method: searched
name: Digitaltableteur Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: Digitaltableteur declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Digitaltableteur
provider_slug: digitaltableteur-com
scheme_count: 1
schemes:
- applies_to:
  - MCP server /mcp
  - WebMCP
  - /api/chat
  - /api/contact
  - /.well-known/agent-skills/*
  - llms.txt / llms-full.txt
  description: 'Authentication: None for read-only tool calls (MCP server). /api/chat: Authentication: None.'
  name: none
  type: none
slug: digitaltableteur-com-authentication
source_filename: digitaltableteur-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: searched\nsource: https://www.digitaltableteur.com/auth.md\ndocs: https://www.digitaltableteur.com/auth.md\nsummary: All agent surfaces are public and unauthenticated. \"No OAuth provider or API keys are issued for public marketing endpoints at this time.\"\nschemes:\n- name: none\n  type: none\n  applies_to: [MCP server /mcp, WebMCP, /api/chat, /api/contact, /.well-known/agent-skills/*, llms.txt / llms-full.txt]\n  description: \"Authentication: None for read-only tool calls (MCP server). /api/chat: Authentication: None.\"\noauth: false\napi_keys: false\nfuture: If authenticated agent APIs are added in the future, auth.md \"will be updated with issuer URLs, scopes and token endpoints.\"\n"
source_yaml_url: https://artifacts.apis.io/digitaltableteur-com/authentication/digitaltableteur-com-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Design Systems
- DesignOps
- Accessibility
- Artificial Intelligence
- MCP
- Consulting
- Finland
---
