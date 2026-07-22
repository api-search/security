---
api_key_in: []
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Rindler Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Rindler secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Rindler
provider_slug: rindler
scheme_count: 1
schemes:
- authorizationUrl: https://mcp.rindler.ai/auth/authorize
  code_challenge_methods_supported:
  - S256
  grant_types_supported:
  - authorization_code
  - refresh_token
  issuer: https://mcp.rindler.ai
  name: OAuth2
  registrationUrl: https://mcp.rindler.ai/auth/register-client
  response_types_supported:
  - code
  scheme: authorization_code + PKCE
  sources:
  - well-known/rindler-mcp-oauth-authorization-server.json
  tokenUrl: https://mcp.rindler.ai/auth/token
  token_endpoint_auth_methods_supported:
  - none
  type: oauth2
slug: rindler-authentication
source_filename: rindler-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://rindler.ai/docs/quickstart\ndocs: https://rindler.ai/docs/auth\nsummary:\n  types: [oauth2]\n  api_key: false\n  oauth2_flows: [authorizationCode]\n  pkce: S256\n  dynamic_client_registration: true\n  client_secret: false\nschemes:\n  - name: OAuth2\n    type: oauth2\n    scheme: authorization_code + PKCE\n    sources: [well-known/rindler-mcp-oauth-authorization-server.json]\n    issuer: https://mcp.rindler.ai\n    authorizationUrl: https://mcp.rindler.ai/auth/authorize\n    tokenUrl: https://mcp.rindler.ai/auth/token\n    registrationUrl: https://mcp.rindler.ai/auth/register-client\n    code_challenge_methods_supported: [S256]\n    grant_types_supported: [authorization_code, refresh_token]\n    response_types_supported: [code]\n    token_endpoint_auth_methods_supported: [none]\nnotes: >-\n  Rindler authenticates agents over OAuth 2.0 with PKCE. On first tool call the\n  runtime opens a browser authorization link; the\
  \ user approves and tokens\n  refresh automatically. There is no API key to paste. The MCP server also\n  supports RFC 7591 dynamic client registration (register-client) and RFC 9728\n  protected-resource metadata. Separately, each mapped site session\n  authenticates to the target portal the way the user's own team does\n  (site-side credentials), handled server-side.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rindler/refs/heads/main/authentication/rindler-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- MCP
- Model Context Protocol
- AI Agents
- Web Automation
- Browser Automation
- Structured Data
- Website to API
- Agent Tools
- Y Combinator
---
