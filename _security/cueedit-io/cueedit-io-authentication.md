---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: CueEditio Authentication
name_suffix: Authentication
oauth_flows: []
overview: CueEditio declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: CueEditio
provider_slug: cueedit-io
scheme_count: 2
schemes:
- applies_to:
  - https://www.cueedit.io/api/v1
  - https://www.cueedit.io/api/mcp/mcp
  description: An agent gets an api_key from an emailed 6-digit code (POST /api/agent/signup, then POST /api/agent/verify). The response has api_key (shown once), mcp_url and connect_url. The same key authorizes the REST API and the MCP connector.
  header: 'Authorization: Bearer <api_key>'
  issuance: email one-time code (self-service, agent-initiated)
  name: CueEditio API key
  scheme: bearer
  type: http
- description: OAuth 2.0 Protected Resource Metadata at https://www.cueedit.io/.well-known/oauth-protected-resource (GET, HTTP 200, 2026-11-04) names resource https://www.cueedit.io/api/mcp/mcp, authorization server https://www.cueedit.io, scopes_supported [mcp], bearer_methods_supported [header]. Used by the Claude / ChatGPT connector. agent.md itself documents Bearer API keys only.
  metadata: https://www.cueedit.io/.well-known/oauth-protected-resource
  name: MCP connector (Claude / ChatGPT)
  scopes:
  - mcp
  type: oauth2
  verified: probed
slug: cueedit-io-authentication
source_filename: cueedit-io-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://www.cueedit.io/agent.md\ndocs: https://www.cueedit.io/agent.md\nschemes:\n- type: http\n  scheme: bearer\n  name: CueEditio API key\n  header: 'Authorization: Bearer <api_key>'\n  applies_to:\n  - https://www.cueedit.io/api/v1\n  - https://www.cueedit.io/api/mcp/mcp\n  description: An agent gets an api_key from an emailed 6-digit code (POST /api/agent/signup, then POST /api/agent/verify). The response has api_key (shown once), mcp_url and connect_url. The same key authorizes\n    the REST API and the MCP connector.\n  issuance: email one-time code (self-service, agent-initiated)\n- type: oauth2\n  name: MCP connector (Claude / ChatGPT)\n  description: OAuth 2.0 Protected Resource Metadata at https://www.cueedit.io/.well-known/oauth-protected-resource (GET, HTTP 200, 2026-11-04) names resource https://www.cueedit.io/api/mcp/mcp, authorization\n    server https://www.cueedit.io, scopes_supported [mcp], bearer_methods_supported\
  \ [header]. Used by the Claude / ChatGPT connector. agent.md itself documents Bearer API keys only.\n  verified: probed\n  scopes:\n  - mcp\n  metadata: https://www.cueedit.io/.well-known/oauth-protected-resource\nnote: Not probed. Under the probe-safety rules no auth, signup or verify endpoint was called.\n"
source_yaml_url: https://artifacts.apis.io/cueedit-io/authentication/cueedit-io-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Video Editing
- Artificial Intelligence
- Social Media
- Scheduling
- Instagram
- Direct Messaging
- Marketing
- MCP
- AI Agents
---
