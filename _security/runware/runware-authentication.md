---
api_key_in:
- header
- body
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Runware Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode-pkce
overview: Runware secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode-pkce flow(s).
provider_name: Runware
provider_slug: runware
scheme_count: 2
schemes:
- description: API key created in the Runware dashboard. Sent as a Bearer token on HTTP requests, or as an authentication task at the start of a WebSocket session.
  format: Bearer <RUNWARE_API_KEY>
  header: Authorization
  in: header
  name: apiKey
  type: apiKey
  websocket_note: WebSocket connections require an initial authentication task carrying the API key; the socket stays open until 120 seconds of inactivity.
- applies_to: mcp.runware.ai
  description: The hosted MCP server (mcp.runware.ai) authenticates clients with OAuth 2.1 + PKCE; the user supplies their Runware API key through a server-rendered page rather than passing it directly to the MCP client.
  name: mcp-oauth
  scheme: OAuth 2.1 with PKCE
  type: oauth2
slug: runware-authentication
source_filename: runware-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://runware.ai/docs/platform/authentication ; https://runware.ai/docs/platform/mcp\ndocs: https://runware.ai/docs/platform/authentication\nsummary:\n  types: [apiKey, oauth2]\n  api_key_in: [header, body]\n  oauth2_flows: [authorizationCode-pkce]\nschemes:\n- name: apiKey\n  type: apiKey\n  description: >-\n    API key created in the Runware dashboard. Sent as a Bearer token on HTTP\n    requests, or as an authentication task at the start of a WebSocket session.\n  in: header\n  header: Authorization\n  format: Bearer <RUNWARE_API_KEY>\n  websocket_note: >-\n    WebSocket connections require an initial authentication task carrying the API\n    key; the socket stays open until 120 seconds of inactivity.\n- name: mcp-oauth\n  type: oauth2\n  scheme: OAuth 2.1 with PKCE\n  description: >-\n    The hosted MCP server (mcp.runware.ai) authenticates clients with OAuth 2.1\n    + PKCE; the user supplies their Runware API key through\
  \ a server-rendered\n    page rather than passing it directly to the MCP client.\n  applies_to: mcp.runware.ai\nnotes: >-\n  No public OpenAPI is published (the API is a single task-based POST endpoint),\n  so this profile is searched from the documentation rather than derived from a\n  spec. There is no OAuth scope surface on the core inference API — access is\n  key-based — so scopes/ is intentionally omitted.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/runware/refs/heads/main/authentication/runware-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- Company
- Artificial Intelligence
- Machine Learning
- Inference
- Image Generation
- Video Generation
- Audio Generation
- Text Generation
- 3D Generation
- Generative AI
- Models
- Developer Tools
---
