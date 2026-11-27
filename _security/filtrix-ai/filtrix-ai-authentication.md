---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Filtrix AI Authentication
name_suffix: Authentication
oauth_flows: []
overview: Filtrix AI declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Filtrix AI
provider_slug: filtrix-ai
scheme_count: 1
schemes:
- carried_in: header
  description: 'Filtrix MCP (https://mcp.filtrix.ai/mcp) requires an Authorization: Bearer <MCP_API_KEY> header on every request. Keys are issued from the Filtrix AI account at https://app.filtrix.ai/mcp-keys and reused across the image and video generation skills. Paid credits must be loaded at https://app.filtrix.ai/billing before generation tools return usable responses; missing or invalid keys return 401.'
  header: Authorization
  key_management: https://app.filtrix.ai/mcp-keys
  name: MCP API key
  scheme: bearer
  type: http
slug: filtrix-ai-authentication
source_filename: filtrix-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-07'\nmethod: searched\nsource: https://agent.filtrix.ai/agent-guide.md\ndocs: https://agent.filtrix.ai/agent-guide.md\nname: Filtrix AI authentication\nschemes:\n- type: http\n  scheme: bearer\n  name: MCP API key\n  description: >-\n    Filtrix MCP (https://mcp.filtrix.ai/mcp) requires an Authorization: Bearer\n    <MCP_API_KEY> header on every request. Keys are issued from the Filtrix AI\n    account at https://app.filtrix.ai/mcp-keys and reused across the image\n    and video generation skills. Paid credits must be loaded at\n    https://app.filtrix.ai/billing before generation tools return usable\n    responses; missing or invalid keys return 401.\n  key_management: https://app.filtrix.ai/mcp-keys\n  carried_in: header\n  header: Authorization\nnotes:\n- The provider publishes no OAuth2, OIDC or API-key-in-URL schemes; the only documented\n  auth is the Bearer MCP key described in the agent guide.\n- 401 responses on https://mcp.filtrix.ai/mcp confirm\
  \ the Bearer requirement at\n  the transport (preflight 2026-11-07).\n"
source_yaml_url: https://artifacts.apis.io/filtrix-ai/authentication/filtrix-ai-authentication.yml
summary_line: 1 scheme
tags:
- Artificial Intelligence
- Image Generation
- Video Generation
- Creative Tools
- Marketing
- Advertising
- Image Editing
- MCP
- Generative AI
---
