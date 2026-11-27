---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: CodeMouse Authentication
name_suffix: Authentication
oauth_flows: []
overview: CodeMouse declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: CodeMouse
provider_slug: codemouse-ai
scheme_count: 1
schemes:
- applies_to: https://codemouse.ai/api/mcp
  description: OAuth 2.1 authorization code flow with PKCE (S256), public clients (token_endpoint_auth_methods_supported none), sign in with GitHub.
  dynamic_client_registration: https://codemouse.ai/api/oauth/register
  flows:
    authorizationCode:
      authorizationUrl: https://codemouse.ai/oauth/authorize
      refreshUrl: https://codemouse.ai/api/oauth/token
      scopes:
      - mcp
      - read
      - write
      tokenUrl: https://codemouse.ai/api/oauth/token
  grant_types:
  - authorization_code
  - refresh_token
  metadata_status: 200
  metadata_url: https://codemouse.ai/.well-known/oauth-authorization-server
  name: oauth2
  pkce: S256
  revocation_endpoint: https://codemouse.ai/api/oauth/revoke
  type: oauth2
slug: codemouse-ai-authentication
source_filename: codemouse-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "name: CodeMouse authentication\ngenerated: '2026-11-04'\nmethod: searched\nsource: https://codemouse.ai/mcp\ndocs: https://codemouse.ai/mcp\nnote: CodeMouse publishes no REST/OpenAPI contract; its only programmatic surface is the remote MCP server at https://codemouse.ai/api/mcp. The docs state \"Authentication uses OAuth 2.1 (PKCE)\"; users sign in with GitHub. Endpoint details below were read from the provider's published RFC 8414 metadata document (GET https://codemouse.ai/.well-known/oauth-authorization-server, HTTP 200, 2026-11-04). No token, registration or authorize endpoint was called. /.well-known/oauth-protected-resource returned 404.\nschemes:\n- name: oauth2\n  type: oauth2\n  applies_to: https://codemouse.ai/api/mcp\n  description: OAuth 2.1 authorization code flow with PKCE (S256), public clients (token_endpoint_auth_methods_supported none), sign in with GitHub.\n  flows:\n    authorizationCode:\n      authorizationUrl: https://codemouse.ai/oauth/authorize\n \
  \     tokenUrl: https://codemouse.ai/api/oauth/token\n      refreshUrl: https://codemouse.ai/api/oauth/token\n      scopes: [mcp, read, write]\n  pkce: S256\n  dynamic_client_registration: https://codemouse.ai/api/oauth/register\n  revocation_endpoint: https://codemouse.ai/api/oauth/revoke\n  grant_types: [authorization_code, refresh_token]\n  metadata_url: https://codemouse.ai/.well-known/oauth-authorization-server\n  metadata_status: 200\nother_credentials:\n- name: Customer AI provider keys (BYOK)\n  description: The service requires customers to supply their own Anthropic, OpenAI, Google or OpenRouter API key, \"encrypted at rest using AES-256-GCM\" (Terms). These are credentials CodeMouse uses outbound, not credentials for calling CodeMouse; the MCP page states \"CodeMouse never sees your AI provider keys\" in the connector.\n  source: https://codemouse.ai/terms\n"
source_yaml_url: https://artifacts.apis.io/codemouse-ai/authentication/codemouse-ai-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Code Review
- Artificial Intelligence
- GitHub
- Pull Requests
- Developer Tools
- LLM
---
