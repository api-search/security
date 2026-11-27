---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Demiton Authentication
name_suffix: Authentication
oauth_flows: []
overview: Demiton declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Demiton
provider_slug: demiton-io
scheme_count: 2
schemes:
- applies_to:
  - Demiton REST API
  - Ask Demiton MCP server
  description: Organisation-scoped API key created in HQ -> API Keys; "Copy the key immediately. It is only shown once." Keys "carry the same identity and access controls as your platform account."
  format: 'Authorization: Bearer YOUR_API_KEY'
  header: Authorization
  issued_at: HQ -> API Keys
  name: apiKeyBearer
  scheme: bearer
  source: https://docs.demiton.io/access/api/
  type: http
- applies_to:
  - Ask Demiton MCP server
  description: Claude and ChatGPT connect via OAuth (sign in with the Demiton account); "ChatGPT auto-discovers the OAuth endpoints from the server - no manual endpoint configuration required." The mcp-remote path also uses OAuth. Headless or CI access uses an API key as a Bearer token instead.
  endpoint: https://api.demiton.io/mcp
  name: mcpOAuth
  source: https://docs.demiton.io/access/mcp-server/
  type: oauth2
slug: demiton-io-authentication
source_filename: demiton-io-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: searched\nsource: https://docs.demiton.io/access/api/\ndocs: https://docs.demiton.io/access/api/\nnote: No public OpenAPI is published (the Swagger reference at /api/v1/docs on each deployment URL requires authentication), so this profile is read from the docs only.\nschemes:\n- name: apiKeyBearer\n  type: http\n  scheme: bearer\n  applies_to: [Demiton REST API, Ask Demiton MCP server]\n  header: Authorization\n  format: 'Authorization: Bearer YOUR_API_KEY'\n  issued_at: HQ -> API Keys\n  description: Organisation-scoped API key created in HQ -> API Keys; \"Copy the key immediately. It is only shown once.\" Keys \"carry the same identity and access controls as your platform account.\"\n  source: https://docs.demiton.io/access/api/\n- name: mcpOAuth\n  type: oauth2\n  applies_to: [Ask Demiton MCP server]\n  endpoint: https://api.demiton.io/mcp\n  description: Claude and ChatGPT connect via OAuth (sign in with the Demiton account); \"ChatGPT auto-discovers\
  \ the OAuth endpoints from the server - no manual endpoint configuration required.\" The mcp-remote path also uses OAuth. Headless or CI access uses an API key as a Bearer token instead.\n  source: https://docs.demiton.io/access/mcp-server/\nanonymous_access: none (\"Every connection is authenticated - there are no anonymous callers.\")\n"
source_yaml_url: https://artifacts.apis.io/demiton-io/authentication/demiton-io-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Construction
- Civil Engineering
- Project Management
- Compliance
- MCP
- Artificial Intelligence
- Open Contracting
---
