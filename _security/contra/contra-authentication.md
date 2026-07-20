---
api_key_in:
- header
api_specs:
- filename: contra-openapi-original.json
  format: json
  label: Contra Public API
  slug: contra-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/contra/refs/heads/main/openapi/contra-openapi-original.json
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Contra Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Contra secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Contra
provider_slug: contra
scheme_count: 2
schemes:
- applies_to: Contra Public API (https://contra.com/public-api/*)
  in: header
  name: PublicApiKey
  notes: The @contra/webflow SDK sends the key in both the X-API-Key and Authorization headers. An unauthenticated request returns HTTP 401 {"code":"Unauthorized","message":"Missing or malformed API key"}.
  parameter: X-API-Key
  sources:
  - openapi/contra-openapi-original.json
  type: apiKey
- applies_to: Contra MCP server (https://contra.com/mcp)
  authorization_url: https://contra.com/api/mcp/oauth/authorize
  dynamic_client_registration: true
  issuer: https://contra.com/api
  name: McpOAuth2
  registration_url: https://contra.com/api/mcp/oauth/register
  scheme: OAuth 2.1 authorization_code + PKCE (S256/plain)
  scopes:
  - mcp:tools
  sources:
  - well-known/contra-openid-configuration.json
  - well-known/contra-oauth-protected-resource-mcp.json
  token_url: https://contra.com/api/mcp/oauth/token
  type: oauth2
slug: contra-authentication
source_filename: contra-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: >-\n  github.com/contra/contra-sdk (src/client.ts, contra-open-api.json), live\n  401 from https://contra.com/public-api/*, and the OAuth discovery surface\n  at https://contra.com/.well-known/*\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: PublicApiKey\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  applies_to: Contra Public API (https://contra.com/public-api/*)\n  notes: >-\n    The @contra/webflow SDK sends the key in both the X-API-Key and\n    Authorization headers. An unauthenticated request returns HTTP 401\n    {\"code\":\"Unauthorized\",\"message\":\"Missing or malformed API key\"}.\n  sources:\n  - openapi/contra-openapi-original.json\n- name: McpOAuth2\n  type: oauth2\n  scheme: OAuth 2.1 authorization_code + PKCE (S256/plain)\n  applies_to: Contra MCP server (https://contra.com/mcp)\n  issuer: https://contra.com/api\n  authorization_url:\
  \ https://contra.com/api/mcp/oauth/authorize\n  token_url: https://contra.com/api/mcp/oauth/token\n  registration_url: https://contra.com/api/mcp/oauth/register\n  dynamic_client_registration: true\n  scopes:\n  - mcp:tools\n  sources:\n  - well-known/contra-openid-configuration.json\n  - well-known/contra-oauth-protected-resource-mcp.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/contra/refs/heads/main/authentication/contra-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- Company
- Future Of Work
- Freelance Marketplace
- Talent
- Hiring
- Professional Network
- Model Context Protocol
- Developer API
---
