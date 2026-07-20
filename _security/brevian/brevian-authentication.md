---
api_key_in: []
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Brevian Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Brevian secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Brevian
provider_slug: brevian
scheme_count: 1
schemes:
- description: OAuth 2.1 authorization-code flow (with PKCE S256) protecting the Brevian hosted MCP server at https://app.brevian.ai/mcp. Supports RFC 7591 dynamic client registration and RFC 7009 token revocation.
  flows:
  - authorizationUrl: https://app.brevian.ai/mcp/authorize
    codeChallengeMethods:
    - S256
    flow: authorizationCode
    registrationUrl: https://app.brevian.ai/mcp/register
    revocationUrl: https://app.brevian.ai/mcp/revoke
    scopes:
      brevian:read: Read access to Brevian revenue-execution context
    tokenEndpointAuthMethods:
    - client_secret_post
    - client_secret_basic
    tokenUrl: https://app.brevian.ai/mcp/token
  name: BrevianMCPOAuth
  sources:
  - well-known/brevian-oauth-authorization-server.json
  type: oauth2
slug: brevian-authentication
source_filename: brevian-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://app.brevian.ai/.well-known/openid-configuration\nsummary:\n  types: [oauth2]\n  oauth2_flows: [authorizationCode]\n  pkce: true\n  dynamic_client_registration: true\nschemes:\n- name: BrevianMCPOAuth\n  type: oauth2\n  description: >-\n    OAuth 2.1 authorization-code flow (with PKCE S256) protecting the Brevian\n    hosted MCP server at https://app.brevian.ai/mcp. Supports RFC 7591 dynamic\n    client registration and RFC 7009 token revocation.\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://app.brevian.ai/mcp/authorize\n    tokenUrl: https://app.brevian.ai/mcp/token\n    registrationUrl: https://app.brevian.ai/mcp/register\n    revocationUrl: https://app.brevian.ai/mcp/revoke\n    codeChallengeMethods: [S256]\n    tokenEndpointAuthMethods: [client_secret_post, client_secret_basic]\n    scopes:\n      brevian:read: Read access to Brevian revenue-execution context\n  sources: [well-known/brevian-oauth-authorization-server.json]\n\
  notes: >-\n  Brevian exposes no public documented REST API; the machine surface is the\n  hosted MCP server, whose auth model is captured here from the published\n  OAuth/OIDC discovery documents. The web app sign-in lives at\n  https://app.brevian.ai/.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/brevian/refs/heads/main/authentication/brevian-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Artificial Intelligence
- Sales
- Revenue Execution
- AI Agents
- CRM
- Model Context Protocol
- Enterprise
---
