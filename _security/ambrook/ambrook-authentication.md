---
api_key_in: []
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Ambrook Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Ambrook secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Ambrook
provider_slug: ambrook
scheme_count: 1
schemes:
- flows:
  - authorizationUrl: https://ambrook.com/oauth/mcp/authorize
    flow: authorizationCode
    grantTypes:
    - authorization_code
    - refresh_token
    pkce: S256
    registrationUrl: https://ambrook.com/api/v1/oauth/mcp/register
    scopes:
      export:download: Download exported reports and data
      external_mcp:read: External MCP read access
      mcp:gateway: MCP gateway access
      mcp:readonly_admin: Read-only administrative access via MCP
      mcp:readonly_graphql: Read-only access to the Ambrook GraphQL data surface via MCP
    tokenUrl: https://ambrook.com/api/v1/oauth/mcp/token
  name: OAuth2
  sources:
  - well-known/ambrook-oauth-authorization-server.json
  type: oauth2
slug: ambrook-authentication
source_filename: ambrook-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: searched\nsource: https://ambrook.com/.well-known/oauth-authorization-server\ndocs: https://ambrook.com/.well-known/oauth-authorization-server\nsummary:\n  types: [oauth2]\n  oauth2_flows: [authorizationCode]\n  pkce: [S256]\n  scopes_count: 5\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://ambrook.com/oauth/mcp/authorize\n    tokenUrl: https://ambrook.com/api/v1/oauth/mcp/token\n    registrationUrl: https://ambrook.com/api/v1/oauth/mcp/register\n    pkce: S256\n    grantTypes: [authorization_code, refresh_token]\n    scopes:\n      mcp:readonly_graphql: Read-only access to the Ambrook GraphQL data surface via MCP\n      mcp:gateway: MCP gateway access\n      mcp:readonly_admin: Read-only administrative access via MCP\n      external_mcp:read: External MCP read access\n      export:download: Download exported reports and data\n  sources: [well-known/ambrook-oauth-authorization-server.json]\n\
  notes: >-\n  Auth model is derived from Ambrook's public RFC 8414 OAuth authorization-server\n  metadata (scoped to its MCP surface). Ambrook publishes no OpenAPI, so this is\n  the authoritative public auth profile. Supports dynamic client registration\n  (RFC 7591) and PKCE.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ambrook/refs/heads/main/authentication/ambrook-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Fintech
- Agriculture
- Accounting
- Bookkeeping
- Payments
- Farm Management
- MCP
---
