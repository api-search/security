---
api_key_in: []
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Genspark Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Genspark secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Genspark
provider_slug: genspark
scheme_count: 1
schemes:
- dynamic_client_registration: https://www.genspark.ai/api/mcp/oauth/register
  flows:
  - authorizationUrl: https://www.genspark.ai/api/mcp/oauth/authorize
    flow: authorizationCode
    pkce: S256
    refreshUrl: https://www.genspark.ai/api/mcp/oauth/token
    revocationUrl: https://www.genspark.ai/api/mcp/oauth/revoke
    scopes:
      mcp:prompts:read: Read MCP prompts
      mcp:resources:read: Read MCP resources
      mcp:tools:call: Invoke MCP tools
      mcp:tools:read: List available MCP tools
    tokenUrl: https://www.genspark.ai/api/mcp/oauth/token
  grant_types:
  - authorization_code
  - refresh_token
  issuer: https://www.genspark.ai
  name: mcpOAuth
  sources:
  - well-known/genspark-openid-configuration.json
  token_endpoint_auth_methods:
  - none
  - client_secret_post
  type: oauth2
slug: genspark-authentication
source_filename: genspark-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: >-\n  https://www.genspark.ai/.well-known/openid-configuration (OAuth authorization-server\n  metadata for Genspark's hosted MCP server)\ndocs: https://www.genspark.ai/.well-known/openid-configuration\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  api_key_in: []\n  notes: >-\n    Genspark's public programmatic surface is its hosted MCP server, authorized with\n    OAuth 2.1 (authorization_code grant with PKCE S256, plus refresh_token). Dynamic\n    client registration (RFC 7591) is offered at the registration_endpoint, and public\n    clients (token_endpoint_auth_method \"none\") are supported alongside client_secret_post.\nschemes:\n- name: mcpOAuth\n  type: oauth2\n  issuer: https://www.genspark.ai\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://www.genspark.ai/api/mcp/oauth/authorize\n    tokenUrl: https://www.genspark.ai/api/mcp/oauth/token\n    refreshUrl: https://www.genspark.ai/api/mcp/oauth/token\n\
  \    revocationUrl: https://www.genspark.ai/api/mcp/oauth/revoke\n    pkce: S256\n    scopes:\n      mcp:tools:read: List available MCP tools\n      mcp:tools:call: Invoke MCP tools\n      mcp:resources:read: Read MCP resources\n      mcp:prompts:read: Read MCP prompts\n  grant_types:\n  - authorization_code\n  - refresh_token\n  token_endpoint_auth_methods:\n  - none\n  - client_secret_post\n  dynamic_client_registration: https://www.genspark.ai/api/mcp/oauth/register\n  sources:\n  - well-known/genspark-openid-configuration.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/genspark/refs/heads/main/authentication/genspark-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Ai
- Artificial Intelligence
- AI Agents
- MCP
- Model Context Protocol
- Productivity
- Automation
- Search
- Workspace
---
