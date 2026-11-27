---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Structura Authentication
name_suffix: Authentication
oauth_flows: []
overview: Structura declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Structura
provider_slug: structura-tools
scheme_count: 1
schemes:
- authorization_url: https://mcp.structura.tools/oauth/authorize
  bearer_methods:
  - header
  evidence:
  - http_status: 200
    url: https://mcp.structura.tools/.well-known/oauth-protected-resource
  - http_status: 200
    url: https://mcp.structura.tools/.well-known/oauth-authorization-server
  - quote: Any other MCP-compliant client (Claude Desktop, MCP Inspector…) that supports OAuth 2.1 (PKCE) discovery will walk you through the same login
    url: https://structura.tools/docs
  flow: authorizationCode
  issuer: https://mcp.structura.tools
  name: mcp-oauth2
  pkce: S256
  registration_url: https://mcp.structura.tools/oauth/register
  scopes:
  - mcp:tools
  - mcp:assistant
  token_endpoint_auth_methods:
  - none
  token_url: https://mcp.structura.tools/oauth/token
  type: oauth2
slug: structura-tools-authentication
source_filename: structura-tools-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: searched\nsource: https://structura.tools/docs\ndocs: https://structura.tools/docs\nsummary: >-\n  The only programmatic surface is the remote MCP server at https://mcp.structura.tools/. MCP clients authenticate with\n  OAuth 2.1 authorization code + PKCE (S256), discovered from the server's RFC 9728 protected-resource metadata and RFC 8414\n  authorization-server metadata, which permit dynamic client registration. The user logs in through the same browser login as the web\n  app (Google/GitHub/Unir), and the bearer token goes in the Authorization header. No API keys are documented.\nschemes:\n- name: mcp-oauth2\n  type: oauth2\n  flow: authorizationCode\n  pkce: S256\n  issuer: https://mcp.structura.tools\n  authorization_url: https://mcp.structura.tools/oauth/authorize\n  token_url: https://mcp.structura.tools/oauth/token\n  registration_url: https://mcp.structura.tools/oauth/register\n  token_endpoint_auth_methods: [none]\n  bearer_methods:\
  \ [header]\n  scopes: [mcp:tools, mcp:assistant]\n  evidence:\n  - url: https://mcp.structura.tools/.well-known/oauth-protected-resource\n    http_status: 200\n  - url: https://mcp.structura.tools/.well-known/oauth-authorization-server\n    http_status: 200\n  - url: https://structura.tools/docs\n    quote: Any other MCP-compliant client (Claude Desktop, MCP Inspector…) that supports OAuth 2.1 (PKCE) discovery will walk you through the same login\nnote: The endpoint URLs come from the published discovery metadata (GET only). None of the authorization, token or registration endpoints was called.\n"
source_yaml_url: https://artifacts.apis.io/structura-tools/authentication/structura-tools-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Code Generation
- Domain Modeling
- UML
- Software Architecture
- Low-Code
- Compliance
- MCP
---
