---
anonymous_access: false
api_key_in: []
api_specs:
- filename: afmr-ai-discovery-api-openapi.yml
  format: yaml
  label: AFMR Discovery API
  slug: afmr-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/afmr-ai/refs/heads/main/openapi/afmr-ai-discovery-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 0
method: searched
name: Afmr Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Agent Failure Mode Registry declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Agent Failure Mode Registry
provider_slug: afmr-ai
scheme_count: 0
schemes: []
slug: afmr-ai-authentication
source_filename: afmr-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: searched\nsource: https://afmr.ai/.well-known/ai-plugin.json (auth.type none) + https://afmr.ai/server.json + https://afmr.ai/.well-known/mcp.json (access public_read_only) + openapi/afmr-ai-discovery-api-openapi.yml (no securitySchemes, no security requirement) + live unauthenticated probes 2026-09-19\ndocs: https://afmr.ai/llms-full.txt\nsummary: >-\n  Every AFMR surface is public and unauthenticated by design. The OpenAPI declares no securitySchemes\n  and no security requirement; ai-plugin.json states auth.type \"none\" and is_user_authenticated\n  false; server.json, mcp.json, afmr.json, agents.json and status.json all declare access\n  \"public_read_only\" for the MCP server and the A2A agent. Live: GET /openapi.json, POST /api/rpc\n  (initialize, tools/list, resources/list, tools/call) and POST /a2a (SendMessage) all returned\n  200 with no credentials.\nschemes: []\nauth_required: false\npublic_read_only: true\noauth2: false\napi_keys:\
  \ false\noauth_discovery:\n  oauth-authorization-server: 404\n  oauth-protected-resource: 404\n  openid-configuration: 404\ncors:\n  access_control_allow_origin: '*'\n  access_control_allow_methods: GET, HEAD, OPTIONS\n  note: The OpenAPI's POST /api/rpc declares a 403 \"Browser Origin is not permitted\" for disallowed browser origins; not observed from a non-browser client.\nwrite_surface: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/afmr-ai/refs/heads/main/authentication/afmr-ai-authentication.yml
summary_line: 0 schemes
tags:
- Company
- AI Agents
- Agent Governance
- Standards
- Reputation
- Failure Modes
- Discovery
- MCP
- A2A
- Machine-Readable Standards
---
