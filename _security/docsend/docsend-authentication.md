---
api_key_in: []
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Docsend Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
- refreshToken
overview: DocSend secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, clientCredentials, and refreshToken flow(s).
provider_name: DocSend
provider_slug: docsend
scheme_count: 1
schemes:
- code_challenge_methods:
  - S256
  flows:
  - authorizationUrl: https://docsend.com/oauth/authorize
    flow: authorizationCode
    refreshUrl: https://docsend.com/oauth/token
    scopes:
      mcp:read: Read access via the DocSend MCP server
      mcp:write: Write access via the DocSend MCP server
    tokenUrl: https://docsend.com/oauth/token
  - flow: clientCredentials
    scopes:
      mcp:read: Read access via the DocSend MCP server
      mcp:write: Write access via the DocSend MCP server
    tokenUrl: https://docsend.com/oauth/token
  name: OAuth2
  registration_endpoint: https://docsend.com/oauth/register
  revocation_endpoint: https://docsend.com/oauth/revoke
  sources:
  - well-known/docsend-oauth-authorization-server.json
  token_endpoint_auth_methods:
  - none
  type: oauth2
slug: docsend-authentication
source_filename: docsend-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: >-\n  https://docsend.com/.well-known/oauth-authorization-server (RFC 8414) +\n  WWW-Authenticate challenge on https://mcp.docsend.com/mcp\nsummary:\n  types: [oauth2]\n  oauth2_flows: [authorizationCode, clientCredentials, refreshToken]\n  pkce: S256\n  dynamic_client_registration: true\nschemes:\n- name: OAuth2\n  type: oauth2\n  sources: [well-known/docsend-oauth-authorization-server.json]\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://docsend.com/oauth/authorize\n    tokenUrl: https://docsend.com/oauth/token\n    refreshUrl: https://docsend.com/oauth/token\n    scopes:\n      mcp:read: Read access via the DocSend MCP server\n      mcp:write: Write access via the DocSend MCP server\n  - flow: clientCredentials\n    tokenUrl: https://docsend.com/oauth/token\n    scopes:\n      mcp:read: Read access via the DocSend MCP server\n      mcp:write: Write access via the DocSend MCP server\n  registration_endpoint:\
  \ https://docsend.com/oauth/register\n  revocation_endpoint: https://docsend.com/oauth/revoke\n  code_challenge_methods: [S256]\n  token_endpoint_auth_methods: [none]\nnotes: >-\n  DocSend exposes an OAuth 2.0 authorization server (RFC 8414 discovery) with\n  dynamic client registration (RFC 7591) and mandatory PKCE (S256). It currently\n  gates the hosted MCP server (mcp:read / mcp:write scopes). No general public\n  REST API OpenAPI was found; this profile derives from the published OAuth\n  discovery metadata.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/docsend/refs/heads/main/authentication/docsend-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Enterprise
- Document Sharing
- Sales Enablement
- Analytics
- Data Room
- E-Signature
- MCP
- Dropbox
---
