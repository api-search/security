---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Clevra Authentication
name_suffix: Authentication
oauth_flows: []
overview: Clevra declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Clevra
provider_slug: clevra-ai
scheme_count: 1
schemes:
- applies_to: https://app.clevra.ai/api/mcp
  client_registration:
  - Client ID Metadata Documents
  - Dynamic Client Registration
  discovery: https://app.clevra.ai/.well-known/oauth-protected-resource/api/mcp
  discovery_standard: RFC 9728 Protected Resource Metadata
  flow: authorization_code
  name: clevra-oauth
  notes: Docs say no API key or pre-shared secret is needed. Every 401 points to the discovery document in its WWW-Authenticate header. Requires a Clevra account with the Org Admin, Manager or Dispatcher role on a Pro, Business or Custom plan (or an active trial).
  pkce: S256
  scopes: []
  summary: OAuth 2.1 authorization code flow with PKCE (S256). The person signs in with their usual Clevra login and approves access; the assistant receives a revocable access token and sends it in the Authorization Bearer header. Tokens in the URL are refused.
  token_placement: 'Authorization: Bearer header'
  type: oauth2
slug: clevra-ai-authentication
source_filename: clevra-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://clevra.ai/mcp\ndocs: https://clevra.ai/mcp\nsummary: The Clevra MCP server (https://app.clevra.ai/api/mcp) uses OAuth 2.1 authorization code with PKCE (S256); the access token is sent as an Authorization Bearer header. No API key. Clevra publishes no REST API.\nschemes:\n- name: clevra-oauth\n  type: oauth2\n  flow: authorization_code\n  pkce: S256\n  token_placement: 'Authorization: Bearer header'\n  applies_to: https://app.clevra.ai/api/mcp\n  discovery: https://app.clevra.ai/.well-known/oauth-protected-resource/api/mcp\n  discovery_standard: RFC 9728 Protected Resource Metadata\n  client_registration: [Client ID Metadata Documents, Dynamic Client Registration]\n  scopes: []\n  summary: OAuth 2.1 authorization code flow with PKCE (S256). The person signs in with their usual Clevra login and approves access; the assistant receives a revocable access token and sends it in the Authorization Bearer header. Tokens in the\
  \ URL are refused.\n  notes: Docs say no API key or pre-shared secret is needed. Every 401 points to the discovery document in its WWW-Authenticate header. Requires a Clevra account with the Org Admin, Manager or Dispatcher role on a Pro, Business or Custom plan (or an active trial).\n"
source_yaml_url: https://artifacts.apis.io/clevra-ai/authentication/clevra-ai-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Field Service Management
- Contractors
- Scheduling
- Invoicing
- Payments
- CRM
- MCP
- AI Assistant
---
