---
api_key_in: []
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Youart Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Youart secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Youart
provider_slug: youart
scheme_count: 1
schemes:
- applies_to: https://mcp.youart.ai/mcp
  flows:
  - flow: authorizationCode
    notes: Interactive browser OAuth sign-in on first MCP connect; the agent reuses the creator's existing YouArt account, credits, and projects. Discrete /.well-known/oauth-authorization-server and oauth-protected-resource documents were not published at probe time (404).
  name: youart_oauth
  sources:
  - https://youart.ai/mcp
  type: oauth2
slug: youart-authentication
source_filename: youart-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://youart.ai/mcp\ndocs: https://youart.ai/mcp\nsummary:\n  types: [oauth2]\n  oauth2_flows: [authorizationCode]\n  api_key_in: []\n  notes: >-\n    YouArt does not publish a public REST API or API-key program; programmatic\n    access is delivered through its hosted MCP server, which authenticates via\n    OAuth (browser sign-in, no API keys). Unauthenticated JSON-RPC calls to the\n    MCP endpoint return HTTP 200 with {\"error\":\"invalid_token\"}.\nschemes:\n- name: youart_oauth\n  type: oauth2\n  applies_to: https://mcp.youart.ai/mcp\n  flows:\n  - flow: authorizationCode\n    notes: >-\n      Interactive browser OAuth sign-in on first MCP connect; the agent reuses\n      the creator's existing YouArt account, credits, and projects. Discrete\n      /.well-known/oauth-authorization-server and oauth-protected-resource\n      documents were not published at probe time (404).\n  sources: [https://youart.ai/mcp]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/youart/refs/heads/main/authentication/youart-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Artificial Intelligence
- Generative AI
- Image Generation
- Video Generation
- Text to Speech
- Creative Tools
- Model Context Protocol
- AI Agents
- Y Combinator
---
