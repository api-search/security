---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: probed
name: ClerkChat Authentication
name_suffix: Authentication
oauth_flows: []
overview: ClerkChat declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: ClerkChat
provider_slug: clerkchat-co
scheme_count: 1
schemes:
- applies_to: https://mcp.clerkchat.co/mcp
  bearer_methods:
  - header
  dynamic_client_registration: https://mcp.clerkchat.co/oauth/register
  evidence: Authorization server metadata (RFC 8414) and protected resource metadata (RFC 9728) served by mcp.clerkchat.co, HTTP 200.
  flows:
    authorizationCode:
      authorizationUrl: https://mcp.clerkchat.co/oauth/authorize
      refreshUrl: https://mcp.clerkchat.co/oauth/token
      scopes:
      - mcp:read
      - mcp:write
      - offline_access
      tokenUrl: https://mcp.clerkchat.co/oauth/token
  grant_types:
  - authorization_code
  - refresh_token
  name: mcpOAuth
  pkce: S256
  revocation_endpoint: https://mcp.clerkchat.co/oauth/revoke
  token_endpoint_auth_methods:
  - none
  - client_secret_basic
  - client_secret_post
  type: oauth2
slug: clerkchat-co-authentication
source_filename: clerkchat-co-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource:\n- https://mcp.clerkchat.co/.well-known/oauth-protected-resource\n- https://mcp.clerkchat.co/.well-known/oauth-authorization-server\n- https://clerkchat.co/docs/guides/connect-assistant.md\ndocs: https://clerkchat.co/docs/guides/connect-assistant\nsummary: ClerkChat publishes no REST API. Its only programmatic surface is the remote MCP server at https://mcp.clerkchat.co/mcp, protected by OAuth 2.x authorization code with PKCE (S256) and dynamic client registration; bearer tokens are sent in the Authorization header. Docs state users \"select OAuth authentication\" and, in Claude, \"Register automatically\" for the OAuth client, then approve specific workspaces in a browser consent screen. Discovery documents returned HTTP 200 on 2026-11-04; no token, register or authorize endpoint was called.\nschemes:\n- name: mcpOAuth\n  type: oauth2\n  applies_to: https://mcp.clerkchat.co/mcp\n  bearer_methods: [header]\n  flows:\n    authorizationCode:\n\
  \      authorizationUrl: https://mcp.clerkchat.co/oauth/authorize\n      tokenUrl: https://mcp.clerkchat.co/oauth/token\n      refreshUrl: https://mcp.clerkchat.co/oauth/token\n      scopes: [mcp:read, mcp:write, offline_access]\n  pkce: S256\n  dynamic_client_registration: https://mcp.clerkchat.co/oauth/register\n  revocation_endpoint: https://mcp.clerkchat.co/oauth/revoke\n  grant_types: [authorization_code, refresh_token]\n  token_endpoint_auth_methods: [none, client_secret_basic, client_secret_post]\n  evidence: Authorization server metadata (RFC 8414) and protected resource metadata (RFC 9728) served by mcp.clerkchat.co, HTTP 200.\n"
source_yaml_url: https://artifacts.apis.io/clerkchat-co/authentication/clerkchat-co-authentication.yml
summary_line: 1 scheme
tags:
- Company
- AI Agents
- Customer Service
- Chatbots
- Messaging
- WhatsApp
- MCP
- Conversational AI
---
