---
api_key_in: []
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Woodstock Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Woodstock secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Woodstock
provider_slug: woodstock
scheme_count: 1
schemes:
- bearer_methods:
  - header
  code_challenge_methods:
  - S256
  description: OAuth 2.0 authorization server protecting the hosted MCP endpoint at https://mcp.app.woodstock.co/mcp (RFC 8414 metadata published; RFC 9728 protected-resource metadata at /.well-known/oauth-protected-resource/mcp).
  flows:
  - authorizationUrl: https://mcp.app.woodstock.co/authorize
    flow: authorizationCode
    refreshUrl: https://mcp.app.woodstock.co/token
    scopes: {}
    tokenUrl: https://mcp.app.woodstock.co/token
  grant_types:
  - authorization_code
  - refresh_token
  name: WoodstockMCPOAuth
  registration_endpoint: https://mcp.app.woodstock.co/register
  revocation_endpoint: https://mcp.app.woodstock.co/revoke
  scopes_supported: []
  sources:
  - well-known/woodstock-mcp-oauth-authorization-server.json
  - well-known/woodstock-mcp-oauth-protected-resource.json
  token_endpoint_auth_methods:
  - client_secret_post
  - client_secret_basic
  type: oauth2
slug: woodstock-authentication
source_filename: woodstock-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://mcp.app.woodstock.co/.well-known/oauth-authorization-server\ndocs: https://woodstock.co/ja/mcp/installation/getting-started\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  pkce: required (S256)\n  dynamic_client_registration: true\n  end_user_factor: passkey (WebAuthn) registered in the Woodstock mobile app;\n    no API keys issued\nschemes:\n- name: WoodstockMCPOAuth\n  type: oauth2\n  description: OAuth 2.0 authorization server protecting the hosted MCP endpoint\n    at https://mcp.app.woodstock.co/mcp (RFC 8414 metadata published; RFC 9728\n    protected-resource metadata at /.well-known/oauth-protected-resource/mcp).\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://mcp.app.woodstock.co/authorize\n    tokenUrl: https://mcp.app.woodstock.co/token\n    refreshUrl: https://mcp.app.woodstock.co/token\n    scopes: {}\n  registration_endpoint: https://mcp.app.woodstock.co/register\n\
  \  revocation_endpoint: https://mcp.app.woodstock.co/revoke\n  code_challenge_methods:\n  - S256\n  token_endpoint_auth_methods:\n  - client_secret_post\n  - client_secret_basic\n  grant_types:\n  - authorization_code\n  - refresh_token\n  scopes_supported: []\n  bearer_methods:\n  - header\n  sources:\n  - well-known/woodstock-mcp-oauth-authorization-server.json\n  - well-known/woodstock-mcp-oauth-protected-resource.json\nnotes: Woodstock publishes no public REST API; the OAuth surface exists to\n  authorize MCP clients. End users authenticate with the passkey they registered\n  in the Woodstock app during account opening (MyNumber Card KYC required).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/woodstock/refs/heads/main/authentication/woodstock-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Investing
- Stock Trading
- Brokerage
- FinTech
- Japan
- MCP
- AI Agents
---
