---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Makerme Authentication
name_suffix: Authentication
oauth_flows: []
overview: Maker.me declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Maker.me
provider_slug: makerme
scheme_count: 2
schemes:
- authorization_endpoint: https://ai.maker.co/oauth/authorize
  bearer_methods:
  - header
  flow: authorization_code
  grant_types:
  - authorization_code
  - refresh_token
  id: oauth2_mcp
  issuer: https://ai.maker.co
  pkce: S256
  registration_endpoint: https://ai.maker.co/oauth/register
  resource: https://ai.maker.co/mcp
  revocation_endpoint: https://ai.maker.co/oauth/revoke
  scopes:
  - maker:read
  - maker:publish
  token_endpoint: https://ai.maker.co/oauth/token
  token_endpoint_auth_methods:
  - none
  type: oauth2
- authorization_endpoint: https://api.maker.co/nav_admin_mcp/authorize
  flow: authorization_code + client_credentials
  grant_types:
  - authorization_code
  - client_credentials
  id: oauth2_nav_admin
  issuer: https://api.maker.co
  note: secondary admin MCP authorization server exposed at api.maker.co
  pkce: S256
  token_endpoint: https://api.maker.co/nav_admin_mcp/token
  token_endpoint_auth_methods:
  - client_secret_post
  - client_secret_basic
  type: oauth2
slug: makerme-authentication
source_filename: makerme-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: >-\n  ai.maker.co and api.maker.co OAuth well-known metadata + docs.maker.co MCP\n  documentation (2026-07-20)\nsummary: >-\n  Maker's programmatic surface (the hosted MCP server) is protected by OAuth 2.0.\n  There is no documented public REST API or API-key scheme; access is delegated\n  through the OAuth authorization-code flow with PKCE, and the MCP endpoint is an\n  RFC 9728 protected resource requiring a bearer token.\nschemes:\n- id: oauth2_mcp\n  type: oauth2\n  flow: authorization_code\n  pkce: S256\n  issuer: https://ai.maker.co\n  authorization_endpoint: https://ai.maker.co/oauth/authorize\n  token_endpoint: https://ai.maker.co/oauth/token\n  registration_endpoint: https://ai.maker.co/oauth/register\n  revocation_endpoint: https://ai.maker.co/oauth/revoke\n  token_endpoint_auth_methods:\n  - none\n  grant_types:\n  - authorization_code\n  - refresh_token\n  scopes:\n  - maker:read\n  - maker:publish\n  bearer_methods:\n\
  \  - header\n  resource: https://ai.maker.co/mcp\n- id: oauth2_nav_admin\n  type: oauth2\n  flow: authorization_code + client_credentials\n  pkce: S256\n  issuer: https://api.maker.co\n  authorization_endpoint: https://api.maker.co/nav_admin_mcp/authorize\n  token_endpoint: https://api.maker.co/nav_admin_mcp/token\n  token_endpoint_auth_methods:\n  - client_secret_post\n  - client_secret_basic\n  grant_types:\n  - authorization_code\n  - client_credentials\n  note: secondary admin MCP authorization server exposed at api.maker.co\ndocs: https://docs.maker.co/features/use-maker-from-your-ai-assistant\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/makerme/refs/heads/main/authentication/makerme-authentication.yml
summary_line: 2 schemes
tags:
- Company
- AI
- Website Builder
- No-Code
- Content Generation
- Design
- Ecommerce
- MCP
- Agents
---
