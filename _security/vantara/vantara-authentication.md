---
api_key_in:
- client-side SDK config
auth_types:
- oauth2
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Vantara Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Milana secures its APIs with oauth2 and apiKey across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Milana
provider_slug: vantara
scheme_count: 2
schemes:
- dynamic_client_registration: true
  flows:
  - authorizationUrl: https://clerk.getmilana.ai/oauth/authorize
    flow: authorizationCode
    pkce: S256
    scopes: 7
    tokenUrl: https://clerk.getmilana.ai/oauth/token
  issuer: https://clerk.getmilana.ai
  name: mcp-oauth
  sources:
  - well-known/vantara-oauth-authorization-server.json
  surface: MCP server (https://app.getmilana.ai/mcp)
  type: oauth2
- credentials:
  - name: productId
    note: Identifies the product being recorded
    prefix: prd_
  - name: clientKey
    note: Publishable client key — documented as safe to include in client-side code
    prefix: key_
  name: sdk-credentials
  obtained_at: https://app.getmilana.ai/settings
  sources:
  - https://docs.getmilana.ai/sdk/init
  - https://docs.getmilana.ai/quickstart/coding-agent
  surface: Browser recording SDK (milana-js)
  type: apiKey
slug: vantara-authentication
source_filename: vantara-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://docs.getmilana.ai/sdk/init + https://app.getmilana.ai/.well-known/oauth-authorization-server\ndocs: https://docs.getmilana.ai/sdk/init\nsummary:\n  types: [oauth2, apiKey]\n  oauth2_flows: [authorizationCode]\n  api_key_in: [client-side SDK config]\nschemes:\n  - name: mcp-oauth\n    type: oauth2\n    surface: MCP server (https://app.getmilana.ai/mcp)\n    issuer: https://clerk.getmilana.ai\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://clerk.getmilana.ai/oauth/authorize\n        tokenUrl: https://clerk.getmilana.ai/oauth/token\n        pkce: S256\n        scopes: 7\n    dynamic_client_registration: true\n    sources: [well-known/vantara-oauth-authorization-server.json]\n  - name: sdk-credentials\n    type: apiKey\n    surface: Browser recording SDK (milana-js)\n    credentials:\n      - name: productId\n        prefix: prd_\n        note: Identifies the product being recorded\n    \
  \  - name: clientKey\n        prefix: key_\n        note: Publishable client key — documented as safe to include in client-side code\n    obtained_at: https://app.getmilana.ai/settings\n    sources:\n      - https://docs.getmilana.ai/sdk/init\n      - https://docs.getmilana.ai/quickstart/coding-agent\nnotes: >-\n  No public REST API is documented; the programmatic surfaces are the browser\n  SDK (product ID + publishable client key) and the hosted MCP server (OAuth\n  2.0 authorization-code with PKCE via Clerk, including RFC 7591 dynamic\n  client registration for MCP clients).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vantara/refs/heads/main/authentication/vantara-authentication.yml
summary_line: oauth2/apiKey · 2 schemes
tags:
- Company
- AI
- Session Replay
- Product Analytics
- Developer Tools
- Agents
- SDK
---
