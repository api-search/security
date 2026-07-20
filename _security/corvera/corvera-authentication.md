---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Corvera Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Corvera secures its APIs with oauth2 and openIdConnect across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Corvera
provider_slug: corvera
scheme_count: 1
schemes:
- client_id_metadata_document_supported: true
  dynamic_client_registration: true
  flows:
    authorizationCode:
      authorizationUrl: https://mcp.corvera.ai/authorize
      registrationUrl: https://mcp.corvera.ai/register
      scopes:
        email: User email address
        openid: OpenID Connect authentication
        profile: Basic user profile
        user:org:read: Read the user's organization/workspace context
      tokenUrl: https://mcp.corvera.ai/token
  grant_types:
  - authorization_code
  - refresh_token
  name: OAuth2
  pkce: S256
  sources:
  - well-known/corvera-oauth-authorization-server.json
  token_endpoint_auth_methods:
  - client_secret_post
  - client_secret_basic
  type: oauth2
slug: corvera-authentication
source_filename: corvera-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://mcp.corvera.ai/.well-known/oauth-authorization-server\ndocs: https://docs.corvera.ai/quickstart\nsummary:\n  types: [oauth2, openIdConnect]\n  oauth2_flows: [authorizationCode]\n  api_key_in: []\n  interface: mcp\nschemes:\n  - name: OAuth2\n    type: oauth2\n    flows:\n      authorizationCode:\n        authorizationUrl: https://mcp.corvera.ai/authorize\n        tokenUrl: https://mcp.corvera.ai/token\n        registrationUrl: https://mcp.corvera.ai/register\n        scopes:\n          openid: OpenID Connect authentication\n          email: User email address\n          profile: Basic user profile\n          user:org:read: Read the user's organization/workspace context\n    pkce: S256\n    grant_types: [authorization_code, refresh_token]\n    token_endpoint_auth_methods: [client_secret_post, client_secret_basic]\n    dynamic_client_registration: true\n    client_id_metadata_document_supported: true\n    sources: [well-known/corvera-oauth-authorization-server.json]\n\
  flow:\n  description: >-\n    Corvera authenticates over its hosted MCP server. On first connect the AI\n    tool opens a Corvera sign-in popup; the user authorizes the OAuth connection\n    to link the tool to their workspace data. Dynamic client registration and\n    PKCE (S256) are supported, so MCP clients can register automatically. After\n    authorization, callable tools are gated by the account's connected\n    integrations and role-based dataset access controls.\n  verify_step: \"Run list_my_integrations to confirm the connection.\"\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/corvera/refs/heads/main/authentication/corvera-authentication.yml
summary_line: oauth2/openIdConnect · 1 scheme
tags:
- Company
- MCP
- Model Context Protocol
- CPG
- Consumer Packaged Goods
- Retail
- Data
- Context Layer
- AI Agents
- Analytics
- Y Combinator
---
