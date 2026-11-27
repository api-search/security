---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Corply Authentication
name_suffix: Authentication
oauth_flows: []
overview: Corply declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Corply
provider_slug: corply-dev
scheme_count: 1
schemes:
- bearer_methods:
  - header
  description: MCP clients authenticate through their native OAuth control (e.g. `claude mcp login corply`, `opencode mcp auth corply`); the founder approves sign-in in the browser and the connection is verified with the `whoami` tool. The docs tell OpenCode users not to set an Authorization header manually.
  dynamic_client_registration: https://corply.dev/oauth/register
  flows:
  - authorizationCode
  grant_types:
  - authorization_code
  - refresh_token
  issuer: https://corply.dev
  name: corply-oauth
  pkce: S256
  scopes_published: false
  token_endpoint_auth_methods:
  - none
  type: oauth2
slug: corply-dev-authentication
source_filename: corply-dev-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource:\n- https://corply.dev/.well-known/oauth-protected-resource\n- https://corply.dev/.well-known/oauth-authorization-server\n- https://corply.dev/security\ndocs: https://corply.dev/setup\nnote: Corply publishes no OpenAPI. Auth here applies to the remote MCP server https://corply.dev/mcp and was read from Corply's published OAuth discovery documents (HTTP 200 on 2026-11-04) and docs. No token, registration or login endpoint was called.\nschemes:\n- name: corply-oauth\n  type: oauth2\n  flows:\n  - authorizationCode\n  pkce: S256\n  grant_types: [authorization_code, refresh_token]\n  token_endpoint_auth_methods: [none]\n  dynamic_client_registration: https://corply.dev/oauth/register\n  issuer: https://corply.dev\n  bearer_methods: [header]\n  scopes_published: false\n  description: MCP clients authenticate through their native OAuth control (e.g. `claude mcp login corply`, `opencode mcp auth corply`); the founder approves sign-in\
  \ in the browser and the connection is verified with the `whoami` tool. The docs tell OpenCode users not to set an Authorization header manually.\n"
source_yaml_url: https://artifacts.apis.io/corply-dev/authentication/corply-dev-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Company Formation
- Incorporation
- Delaware C-Corp
- Legal Tech
- AI Agents
- MCP
- Startups
---
