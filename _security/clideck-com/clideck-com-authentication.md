---
anonymous_access: true
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: CliDeck Authentication
name_suffix: Authentication
oauth_flows: []
overview: CliDeck declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: CliDeck
provider_slug: clideck-com
scheme_count: 3
schemes:
- applies_to: https://mcp.clideck.com/mcp
  description: 'Public CliDeck MCP requires no authentication: "No CliDeck account or access token is required for the public server."'
  name: public-mcp-none
  type: none
- applies_to: https://go.clideck.com/mcp
  description: OAuth 2.0 protected resource per RFC 9728 metadata at https://go.clideck.com/.well-known/oauth-protected-resource (resource_name "WipeGo MCP", authorization_servers https://go.clideck.com, bearer_methods_supported header, scopes_supported mcp.use). Anonymous calls return 401.
  name: wipego-mcp-oauth2
  source: https://go.clideck.com/.well-known/oauth-protected-resource
  type: oauth2
- applies_to: /public/v1/playground/*
  description: 'Server-only upstream headers used by the clideck.com website BFF - "Authorization: Bearer <CLIDECK_MCP_PLAYGROUND_TOKEN>" plus "X-CliDeck-Client-Key" (daily base64url HMAC). Not a public developer credential.'
  name: playground-bff-bearer
  scheme: bearer
  source: https://raw.githubusercontent.com/SmartRoot7/clideck-mcp/main/docs/PLAYGROUND_API.md
  type: http
slug: clideck-com-authentication
source_filename: clideck-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://clideck.com/software/mcp\ndocs: https://clideck.com/software/mcp\nschemes:\n- name: public-mcp-none\n  type: none\n  applies_to: https://mcp.clideck.com/mcp\n  description: 'Public CliDeck MCP requires no authentication: \"No CliDeck account or access token is required for the public server.\"'\n- name: wipego-mcp-oauth2\n  type: oauth2\n  applies_to: https://go.clideck.com/mcp\n  description: OAuth 2.0 protected resource per RFC 9728 metadata at https://go.clideck.com/.well-known/oauth-protected-resource (resource_name \"WipeGo MCP\", authorization_servers https://go.clideck.com, bearer_methods_supported header, scopes_supported mcp.use). Anonymous calls return 401.\n  source: https://go.clideck.com/.well-known/oauth-protected-resource\n- name: playground-bff-bearer\n  type: http\n  scheme: bearer\n  applies_to: /public/v1/playground/*\n  description: 'Server-only upstream headers used by the clideck.com website BFF\
  \ - \"Authorization: Bearer <CLIDECK_MCP_PLAYGROUND_TOKEN>\" plus \"X-CliDeck-Client-Key\" (daily base64url HMAC). Not a public developer credential.'\n  source: https://raw.githubusercontent.com/SmartRoot7/clideck-mcp/main/docs/PLAYGROUND_API.md\nnote: 'The CliDeck API & Integrations offering (clideck.com/software/api) is project-specific; \"Public API access, scopes, webhook delivery, and data schemas are provided by project\". No public REST API authentication is documented.'\n"
source_yaml_url: https://artifacts.apis.io/clideck-com/authentication/clideck-com-authentication.yml
summary_line: 3 schemes
tags:
- Company
- Network Automation
- Terminal
- SSH
- Serial Console
- Out-of-Band Management
- Console Server
- MCP
- Infrastructure
- ITAD
---
