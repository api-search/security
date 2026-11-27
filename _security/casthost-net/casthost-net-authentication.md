---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: probed
name: CastHost Authentication
name_suffix: Authentication
oauth_flows: []
overview: CastHost declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: CastHost
provider_slug: casthost-net
scheme_count: 1
schemes:
- applies_to: https://dashboard.casthost.net/mcp
  authorization_endpoint: https://dashboard.casthost.net/oauth/authorize
  bearer_methods:
  - header
  docs_statement: You approve each connection yourself, and every app only ever sees your own account, never anyone else's.
  dynamic_client_registration: true
  flows:
  - authorization_code
  - refresh_token
  issuer: https://dashboard.casthost.net
  name: casthost-mcp-oauth2
  pkce: S256
  protected_resource_metadata: https://dashboard.casthost.net/.well-known/oauth-protected-resource/mcp
  registration_endpoint: https://dashboard.casthost.net/oauth/register
  revocation_endpoint: https://dashboard.casthost.net/oauth/token/revoke
  scopes: scopes/casthost-net-scopes.yml
  token_endpoint: https://dashboard.casthost.net/oauth/token
  token_endpoint_auth_methods:
  - none
  type: oauth2
slug: casthost-net-authentication
source_filename: casthost-net-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: probed\nsource: https://dashboard.casthost.net/.well-known/oauth-authorization-server\ndocs: https://www.casthost.net/mcp.php\nname: CastHost authentication\nnote: CastHost publishes no REST API or OpenAPI. The only programmatic surface is the beta remote MCP server, protected by OAuth 2.0. Values below come from its RFC 9728 protected-resource metadata and RFC 8414 authorization-server metadata (GET only). Token, registration and authorize endpoints are recorded as published and were NOT called.\nschemes:\n- name: casthost-mcp-oauth2\n  type: oauth2\n  applies_to: https://dashboard.casthost.net/mcp\n  flows:\n  - authorization_code\n  - refresh_token\n  pkce: S256\n  token_endpoint_auth_methods: [none]\n  bearer_methods: [header]\n  issuer: https://dashboard.casthost.net\n  authorization_endpoint: https://dashboard.casthost.net/oauth/authorize\n  token_endpoint: https://dashboard.casthost.net/oauth/token\n  registration_endpoint: https://dashboard.casthost.net/oauth/register\n\
  \  revocation_endpoint: https://dashboard.casthost.net/oauth/token/revoke\n  dynamic_client_registration: true\n  protected_resource_metadata: https://dashboard.casthost.net/.well-known/oauth-protected-resource/mcp\n  scopes: scopes/casthost-net-scopes.yml\n  docs_statement: \"You approve each connection yourself, and every app only ever sees your own account, never anyone else's.\"\n"
source_yaml_url: https://artifacts.apis.io/casthost-net/authentication/casthost-net-authentication.yml
summary_line: 1 scheme
tags:
- Internet Radio
- Hosting
- Shoutcast
- Icecast
- cPanel
---
