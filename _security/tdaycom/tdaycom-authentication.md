---
api_key_in: []
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Tdaycom Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Tdaycom secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Tdaycom
provider_slug: tdaycom
scheme_count: 1
schemes:
- authorization_endpoint: https://tday.com/api/mcp/oauth/authorize
  authorization_server: https://tday.com
  dynamic_client_registration: true
  flow: authorizationCode
  name: OAuth2
  pkce: S256
  protects:
  - https://tday.com/api/mcp
  public_client: true
  registration_endpoint: https://tday.com/api/mcp/oauth/register
  revocation_endpoint: https://tday.com/api/mcp/oauth/revoke
  scopes:
  - tday
  sources:
  - well-known/tdaycom-oauth-authorization-server.json
  - well-known/tdaycom-oauth-protected-resource.json
  token_endpoint: https://tday.com/api/mcp/oauth/token
  token_endpoint_auth_methods_supported:
  - none
  type: oauth2
slug: tdaycom-authentication
source_filename: tdaycom-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://tday.com/.well-known/oauth-authorization-server\ndocs: https://tday.com/.well-known/oauth-protected-resource\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  api_key_in: []\n  note: >-\n    tday has no published OpenAPI; this profile is derived from its live OAuth 2.1\n    discovery metadata (RFC 8414 authorization-server + RFC 9728 protected-resource).\nschemes:\n- name: OAuth2\n  type: oauth2\n  flow: authorizationCode\n  pkce: S256\n  dynamic_client_registration: true\n  public_client: true\n  token_endpoint_auth_methods_supported:\n  - none\n  authorization_server: https://tday.com\n  authorization_endpoint: https://tday.com/api/mcp/oauth/authorize\n  token_endpoint: https://tday.com/api/mcp/oauth/token\n  registration_endpoint: https://tday.com/api/mcp/oauth/register\n  revocation_endpoint: https://tday.com/api/mcp/oauth/revoke\n  scopes:\n  - tday\n  protects:\n  - https://tday.com/api/mcp\n\
  \  sources:\n  - well-known/tdaycom-oauth-authorization-server.json\n  - well-known/tdaycom-oauth-protected-resource.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tdaycom/refs/heads/main/authentication/tdaycom-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Marketing
- Artificial Intelligence
- Content Generation
- Video
- Social Media
- Developer Tools
- MCP
- Agents
- Y Combinator
---
