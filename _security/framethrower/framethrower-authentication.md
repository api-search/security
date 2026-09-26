---
anonymous_access: false
api_key_in: []
api_specs:
- filename: framethrower-openapi.yml
  format: yaml
  label: FrameThrower API
  slug: framethrower-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/framethrower/refs/heads/main/openapi/framethrower-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Framethrower Authentication
name_suffix: Authentication
oauth_flows: []
overview: FrameThrower secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: FrameThrower
provider_slug: framethrower
scheme_count: 2
schemes:
- description: Personal access token, prefix `ft_`. Create one at https://framethrower.ai/settings?tab=api — free accounts included, no plan required.
  header: 'Authorization: Bearer ft_YOUR_TOKEN'
  how_to_get_token: Sign up at https://framethrower.ai/register (free, no card), then create a token at https://framethrower.ai/settings?tab=api
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/framethrower-openapi.yml
  - https://framethrower.ai/api/v1
  surface: REST API (https://framethrower.ai/api/v1)
  token_prefix: ft_
  type: http
- description: OAuth 2.1 for MCP clients per the framethrower-mcp README; metadata served at /.well-known/oauth-authorization-server (RFC 8414) and /.well-known/oauth-protected-resource (RFC 9728).
  flows:
    authorizationCode:
      authorizationUrl: https://framethrower.ai/api/auth/mcp/authorize
      pkce: S256
      tokenUrl: https://framethrower.ai/api/auth/mcp/token
  name: mcpOAuth
  registration_endpoint: https://framethrower.ai/api/auth/mcp/register
  scopes_supported:
  - openid
  - profile
  - email
  - offline_access
  sources:
  - https://framethrower.ai/.well-known/oauth-authorization-server
  - https://github.com/framethrower-ai/framethrower-mcp
  surface: MCP server (https://framethrower.ai/api/mcp)
  type: oauth2
slug: framethrower-authentication
source_filename: framethrower-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-25'\nmethod: searched\nsource:\n- openapi/framethrower-openapi.yml\n- https://framethrower.ai/api/v1\n- https://framethrower.ai/.well-known/oauth-authorization-server\n- https://framethrower.ai/.well-known/oauth-protected-resource\ndocs: https://framethrower.ai/developers\nsummary:\n  types:\n  - http\n  - oauth2\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  surface: REST API (https://framethrower.ai/api/v1)\n  description: Personal access token, prefix `ft_`. Create one at https://framethrower.ai/settings?tab=api — free accounts included, no plan required.\n  header: 'Authorization: Bearer ft_YOUR_TOKEN'\n  token_prefix: ft_\n  how_to_get_token: Sign up at https://framethrower.ai/register (free, no card), then create a token at https://framethrower.ai/settings?tab=api\n  sources:\n  - openapi/framethrower-openapi.yml\n  - https://framethrower.ai/api/v1\n- name: mcpOAuth\n  type: oauth2\n  surface: MCP server (https://framethrower.ai/api/mcp)\n\
  \  flows:\n    authorizationCode:\n      authorizationUrl: https://framethrower.ai/api/auth/mcp/authorize\n      tokenUrl: https://framethrower.ai/api/auth/mcp/token\n      pkce: S256\n  registration_endpoint: https://framethrower.ai/api/auth/mcp/register\n  scopes_supported: [openid, profile, email, offline_access]\n  description: OAuth 2.1 for MCP clients per the framethrower-mcp README; metadata served at /.well-known/oauth-authorization-server (RFC 8414) and /.well-known/oauth-protected-resource (RFC 9728).\n  sources:\n  - https://framethrower.ai/.well-known/oauth-authorization-server\n  - https://github.com/framethrower-ai/framethrower-mcp\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/framethrower/refs/heads/main/authentication/framethrower-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Film
- Cinematography
- Visual Reference
- Image Search
- Media
- Creative Tools
- MCP
- Agent-Native
---
