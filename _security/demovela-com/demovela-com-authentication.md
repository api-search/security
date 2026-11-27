---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Demovela Authentication
name_suffix: Authentication
oauth_flows: []
overview: Demovela declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Demovela
provider_slug: demovela-com
scheme_count: 2
schemes:
- api_keys: false
  applies_to: https://demovela.com/v1
  description: 'Verbatim (n8n README): "Credentials use dynamic registration, OAuth authorization code flow, PKCE, expiring access tokens, and refresh tokens. The API resource is `https://demovela.com/v1`; REST tokens are separate from MCP tokens."'
  dynamic_client_registration: true
  flows:
  - authorizationCode
  name: Demovela OAuth2 (REST API)
  pkce: true
  refresh_tokens: true
  resource: https://demovela.com/v1
  type: oauth2
- applies_to: https://mcp.demovela.com/mcp
  description: Browser-based OAuth sign-in and consent; the npm bridge uses pinned mcp-remote for OAuth, PKCE and local token storage.
  flows:
  - authorizationCode
  name: Demovela OAuth2 (MCP server)
  pkce: true
  scopes:
  - profile:read
  - videos:read
  - drafts:write
  source: https://github.com/demovela/mcp-server
  type: oauth2
slug: demovela-com-authentication
source_filename: demovela-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "name: Demovela authentication\ngenerated: '2026-11-05'\nmethod: searched\nsource: https://demovela.com/integrations/n8n/\ndocs: https://github.com/demovela/n8n-nodes-demovela#authentication\nschemes:\n- name: Demovela OAuth2 (REST API)\n  type: oauth2\n  applies_to: https://demovela.com/v1\n  flows: [authorizationCode]\n  pkce: true\n  dynamic_client_registration: true\n  refresh_tokens: true\n  resource: https://demovela.com/v1\n  description: 'Verbatim (n8n README): \"Credentials use dynamic registration, OAuth authorization code flow, PKCE, expiring access tokens, and refresh tokens. The API resource is `https://demovela.com/v1`; REST tokens are separate from MCP tokens.\"'\n  api_keys: false\n- name: Demovela OAuth2 (MCP server)\n  type: oauth2\n  applies_to: https://mcp.demovela.com/mcp\n  flows: [authorizationCode]\n  pkce: true\n  scopes: [profile:read, videos:read, drafts:write]\n  source: https://github.com/demovela/mcp-server\n  description: Browser-based OAuth sign-in\
  \ and consent; the npm bridge uses pinned mcp-remote for OAuth, PKCE and local token storage.\nrevocation: Connected apps can be reviewed and revoked at https://demovela.com/oauth/n8n/connections (REST/n8n) and https://demovela.com/oauth/mcp/connections (MCP).\nnote: The docs state \"OAuth sign-in, no API keys\". No OpenAPI is published, so this is read from docs rather than derived from securitySchemes. Authentication endpoints were not called.\n"
source_yaml_url: https://artifacts.apis.io/demovela-com/authentication/demovela-com-authentication.yml
summary_line: 2 schemes
tags:
- Company
- AI Video
- Product Demos
- Marketing Video
- Video Generation
- MCP
- n8n
- Software-as-a-Service
---
