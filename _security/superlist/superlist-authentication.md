---
api_key_in: []
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Superlist Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Superlist secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Superlist
provider_slug: superlist
scheme_count: 1
schemes:
- bearer_methods_supported:
  - header
  dynamic_client_registration: https://app.superlist.com/oauth/register
  flows:
  - authorizationUrl: https://app.superlist.com/oauth/authorize
    flow: authorizationCode
    pkce: S256
    tokenUrl: https://app.superlist.com/oauth/token
  grant_types_supported:
  - authorization_code
  - refresh_token
  issuer: https://app.superlist.com
  name: OAuth2
  protected_resource: https://app.superlist.com/mcp
  protected_resource_metadata: https://app.superlist.com/.well-known/oauth-protected-resource
  response_types_supported:
  - code
  scopes_advertised: []
  source: https://app.superlist.com/.well-known/oauth-authorization-server
  token_endpoint_auth_methods_supported:
  - none
  - client_secret_basic
  - client_secret_post
  type: oauth2
slug: superlist-authentication
source_filename: superlist-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: >-\n  https://app.superlist.com/.well-known/oauth-authorization-server +\n  https://help.superlist.com/en/articles/658028-superlist-mcp-server\ndocs: https://help.superlist.com/en/articles/658028-superlist-mcp-server\nsummary:\n  types: [oauth2]\n  oauth2_flows: [authorizationCode]\n  api_key_in: []\n  surface: MCP server (https://app.superlist.com/mcp)\n  notes: >-\n    Superlist exposes no traditional REST API key surface. Programmatic access is via the\n    hosted MCP server, authenticated with OAuth 2.0 using PKCE (S256) and dynamic client\n    registration. Bearer tokens are presented in the Authorization header (per RFC 9728\n    protected-resource metadata: bearer_methods_supported = [\"header\"]).\nschemes:\n  - name: OAuth2\n    type: oauth2\n    source: https://app.superlist.com/.well-known/oauth-authorization-server\n    issuer: https://app.superlist.com\n    flows:\n      - flow: authorizationCode\n        authorizationUrl:\
  \ https://app.superlist.com/oauth/authorize\n        tokenUrl: https://app.superlist.com/oauth/token\n        pkce: S256\n    dynamic_client_registration: https://app.superlist.com/oauth/register\n    grant_types_supported: [authorization_code, refresh_token]\n    response_types_supported: [code]\n    token_endpoint_auth_methods_supported: [none, client_secret_basic, client_secret_post]\n    protected_resource: https://app.superlist.com/mcp\n    protected_resource_metadata: https://app.superlist.com/.well-known/oauth-protected-resource\n    bearer_methods_supported: [header]\n    scopes_advertised: []   # authorization-server metadata does not advertise a scopes_supported list\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/superlist/refs/heads/main/authentication/superlist-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Project Management Sector
- Task Management
- Productivity
- To-Do Lists
- Collaboration
- MCP
- Agents
- AI Assistant
---
