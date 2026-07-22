---
api_key_in: []
auth_types:
- oauth2
- http
description: Authentication model for the Virtue AI MCP gateway surface. No public REST OpenAPI is published, so this profile is captured from the documented gateway connection flow rather than derived from a spec. Connecting an agent runtime performs a browser-based OAuth login against the gateway; thereafter each proxied MCP tools/call request carries a Bearer access token.
kind: authentication
layout: security
method: searched
name: Virtue Ai Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Virtue Ai secures its APIs with oauth2 and http across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Virtue Ai
provider_slug: virtue-ai
scheme_count: 2
schemes:
- description: Browser OAuth login initiated by the gateway-connect CLI at setup.
  flow: authorizationCode
  name: gatewayOAuth
  sources:
  - mcp/virtue-ai-mcp.yml
  type: oauth2
- description: Bearer access token sent on each JSON-RPC tools/call to the gateway.
  name: bearerAuth
  scheme: bearer
  sources:
  - mcp/virtue-ai-mcp.yml
  type: http
slug: virtue-ai-authentication
source_filename: virtue-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://www.npmjs.com/package/@virtue-ai/gateway-connect\ndescription: >-\n  Authentication model for the Virtue AI MCP gateway surface. No public REST\n  OpenAPI is published, so this profile is captured from the documented gateway\n  connection flow rather than derived from a spec. Connecting an agent runtime\n  performs a browser-based OAuth login against the gateway; thereafter each\n  proxied MCP tools/call request carries a Bearer access token.\nsummary:\n  types: [oauth2, http]\n  api_key_in: []\n  oauth2_flows: [authorizationCode]\nschemes:\n  - name: gatewayOAuth\n    type: oauth2\n    flow: authorizationCode\n    description: Browser OAuth login initiated by the gateway-connect CLI at setup.\n    sources: [mcp/virtue-ai-mcp.yml]\n  - name: bearerAuth\n    type: http\n    scheme: bearer\n    description: Bearer access token sent on each JSON-RPC tools/call to the gateway.\n    sources: [mcp/virtue-ai-mcp.yml]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/virtue-ai/refs/heads/main/authentication/virtue-ai-authentication.yml
summary_line: oauth2/http · 2 schemes
tags:
- Company
- AI Security
- AI Safety
- LLM Guardrails
- AI Agents
- Red Teaming
- Model Context Protocol
- Agent Security
- Compliance
---
