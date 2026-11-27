---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Чип (Chip AI) Authentication
name_suffix: Authentication
oauth_flows: []
overview: Чип (Chip AI) declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Чип (Chip AI)
provider_slug: chip-ai-digital
scheme_count: 1
schemes:
- evidence: 'claude mcp add --transport http chip https://chip-ai.digital/mcp --header "Authorization: Bearer chip_mcp_YOUR_TOKEN"'
  format: Bearer chip_mcp_YOUR_TOKEN
  header: Authorization
  in: header
  issuance: '@ChipAI_robot → mini app → Chip MCP → issue a token'
  modes:
  - read
  - full
  name: connectionToken
  scheme: bearer
  token_prefix: chip_mcp_
  type: http
slug: chip-ai-digital-authentication
source_filename: chip-ai-digital-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: searched\nsource:\n- https://github.com/zapret-digital/chip-mcp\n- https://chip-ai.digital/mcp\ndocs: https://chip-ai.digital/mcp\nsummary: The MCP server uses a bearer connection token (chip_mcp_…) issued in the\n  Chip Telegram mini-app, sent in the Authorization header. Tokens are issued in read\n  or full mode; read tokens see 11 tools and are refused writes on the call itself.\n  Listing tools needs no token; every call does. Tokens are stored as SHA-256 and\n  shown once.\nschemes:\n- name: connectionToken\n  type: http\n  scheme: bearer\n  in: header\n  header: Authorization\n  format: Bearer chip_mcp_YOUR_TOKEN\n  token_prefix: chip_mcp_\n  issuance: '@ChipAI_robot → mini app → Chip MCP → issue a token'\n  modes:\n  - read\n  - full\n  evidence: 'claude mcp add --transport http chip https://chip-ai.digital/mcp --header\n    \"Authorization: Bearer chip_mcp_YOUR_TOKEN\"'\nunauthenticated:\n- tools/list\n"
source_yaml_url: https://artifacts.apis.io/chip-ai-digital/authentication/chip-ai-digital-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Artificial Intelligence
- AI Assistant
- Chatbots
- Telegram
- MCP
- Agents
- Russian
---
