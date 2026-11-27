---
anonymous_access: false
api_key_in: []
api_specs:
- filename: nflmcp-com-openapi-generated.yml
  format: yaml
  label: NFL MCP API
  slug: nflmcp-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nflmcp-com/openapi/_ae-authored/nflmcp-com-openapi-generated.yml
auth_types: []
description: Authentication methods for NFL MCP as documented on the authentication page.
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: NFL MCP Authentication
name_suffix: Authentication
oauth_flows: []
overview: NFL MCP declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: NFL MCP
provider_slug: nflmcp-com
scheme_count: 2
schemes:
- evidence: 'Send it as a bearer token on every request: Authorization header Authorization: Bearer YOUR_API_KEY'
  header: Authorization
  how_to_obtain: Create a key in the dashboard — the raw value is shown once at creation, so store it somewhere safe.
  location: header
  name: API key
  type: http-bearer
- evidence: OAuth 2.1 is the recommended path for clients that support remote MCP servers, such as Claude and ChatGPT.
  how_to_obtain: Dynamic client registration lets a compatible client register itself with the authorization server without asking you to configure a client ID or secret. The server advertises its authorization server at /.well-known/oauth-protected-resource/mcp and a compliant client discovers and completes the flow for you.
  name: OAuth 2.1
  type: oauth2
slug: nflmcp-com-authentication
source_filename: nflmcp-com-authentication.yml
source_heading: Authentication Profile
source_url: https://nflmcp.com/docs/authentication
source_yaml: "generated: '2026-11-19'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://nflmcp.com/docs/authentication\nsources:\n- https://nflmcp.com/docs/authentication\n- https://nflmcp.com/docs/claude\n- https://nflmcp.com/docs/chatgpt\ndescription: Authentication methods for NFL MCP as documented on the authentication page.\nschemes:\n- type: http-bearer\n  name: API key\n  evidence: 'Send it as a bearer token on every request: Authorization header Authorization: Bearer YOUR_API_KEY'\n  location: header\n  header: Authorization\n  how_to_obtain: Create a key in the dashboard — the raw value is shown once at creation, so store it somewhere safe.\n- type: oauth2\n  name: OAuth 2.1\n  evidence: OAuth 2.1 is the recommended path for clients that support remote MCP servers, such as Claude and ChatGPT.\n  how_to_obtain: Dynamic client registration lets a compatible client register itself with the authorization server without asking you to configure\n    a client\
  \ ID or secret. The server advertises its authorization server at /.well-known/oauth-protected-resource/mcp and a compliant client\n    discovers and completes the flow for you.\ndocs: https://nflmcp.com/docs/authentication\n"
source_yaml_url: https://artifacts.apis.io/nflmcp-com/authentication/nflmcp-com-authentication.yml
summary_line: 2 schemes
tags:
- Artificial Intelligence
- Sports
- Analytics
- Fantasy Football
- Betting
- Data
---
