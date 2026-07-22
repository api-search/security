---
api_key_in: []
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Zeni Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Zeni secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Zeni
provider_slug: zeni
scheme_count: 1
schemes:
- access_model: read-only
  authorization_servers:
  - https://api.zeni.ai/auth
  bearer_methods_supported:
  - header
  name: MCPBearer
  resource: https://api.zeni.ai/zeni-mcp-server/mcp
  scope: company
  sources:
  - https://api.zeni.ai/.well-known/oauth-protected-resource
  type: oauth2
slug: zeni-authentication
source_filename: zeni-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://api.zeni.ai/.well-known/oauth-protected-resource\ndocs: https://www.zeni.ai/product/zeni-mcp\nsummary:\n  types:\n  - oauth2\n  api_key_in: []\n  oauth2_flows:\n  - authorizationCode\n  notes: >-\n    Zeni exposes no public REST OpenAPI. The documented programmatic surface is the\n    hosted Zeni MCP server, which is an OAuth 2.0 protected resource (RFC 9728). The\n    protected-resource metadata advertises the authorization server and bearer-in-header\n    token presentation; access is scoped to the signed-in Zeni company and is read-only.\nschemes:\n- name: MCPBearer\n  type: oauth2\n  resource: https://api.zeni.ai/zeni-mcp-server/mcp\n  authorization_servers:\n  - https://api.zeni.ai/auth\n  bearer_methods_supported:\n  - header\n  access_model: read-only\n  scope: company\n  sources:\n  - https://api.zeni.ai/.well-known/oauth-protected-resource\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zeni/refs/heads/main/authentication/zeni-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Fintech
- Bookkeeping
- Accounting
- Financial Operations
- Startups
- MCP
- AI Agents
---
