---
api_key_in:
- header
auth_types:
- oauth2
- apiKey
- http
description: ''
kind: authentication
layout: security
method: searched
name: Supplier Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Supplier secures its APIs with oauth2, apiKey, and http across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Supplier
provider_slug: supplier
scheme_count: 3
schemes:
- authorizationUrl: https://supplier.io/authorize
  flow: authorizationCode
  name: OAuth2
  pkce: S256
  registrationUrl: https://supplier.io/register
  scopes:
  - mcp:full
  sources:
  - well-known/supplier-oauth-authorization-server.json
  tokenUrl: https://supplier.io/token
  type: oauth2
- in: header
  name: ApiKey
  parameter: X-Royal-MCP-API-Key
  sources:
  - live probe of supplier.io/wp-json/royal-mcp/v1
  type: apiKey
- in: header
  name: Bearer
  parameter: Authorization
  scheme: bearer
  sources:
  - well-known/supplier-oauth-protected-resource.json
  type: http
slug: supplier-authentication
source_filename: supplier-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://supplier.io/.well-known/oauth-authorization-server + /.well-known/oauth-protected-resource\nscope: MCP server (supplier.io/wp-json/royal-mcp/v1) — no other public API is documented\nsummary:\n  types: [oauth2, apiKey, http]\n  api_key_in: [header]\n  oauth2_flows: [authorizationCode]\nschemes:\n- name: OAuth2\n  type: oauth2\n  flow: authorizationCode\n  authorizationUrl: https://supplier.io/authorize\n  tokenUrl: https://supplier.io/token\n  registrationUrl: https://supplier.io/register\n  pkce: S256\n  scopes: [mcp:full]\n  sources: ['well-known/supplier-oauth-authorization-server.json']\n- name: ApiKey\n  type: apiKey\n  in: header\n  parameter: X-Royal-MCP-API-Key\n  sources: ['live probe of supplier.io/wp-json/royal-mcp/v1']\n- name: Bearer\n  type: http\n  scheme: bearer\n  in: header\n  parameter: Authorization\n  sources: ['well-known/supplier-oauth-protected-resource.json']\nnotes: >-\n  Authentication model\
  \ reflects the published Royal MCP server surface only. Supplier.io's\n  core procurement application (explorer.supplier.io) is a session/login web app with no\n  documented public developer API.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/supplier/refs/heads/main/authentication/supplier-authentication.yml
summary_line: oauth2/apiKey/http · 3 schemes
tags:
- Company
- Procurement
- Supply Chain
- Supplier Diversity
- Spend Analytics
- Sourcing
- ESG
- Sustainability
- MCP
---
