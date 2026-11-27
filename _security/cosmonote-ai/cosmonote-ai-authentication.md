---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Cosmonote Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cosmonote declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Cosmonote
provider_slug: cosmonote-ai
scheme_count: 2
schemes:
- applies_to: REST API (https://nebula.cosmonote.ai/api/v1)
  header: 'Authorization: Bearer cnk_your_api_key'
  issuance: 'Find your API key in the app: Settings → API keys'
  key_prefix: cnk_
  name: apiKeyBearer
  scheme: bearer
  source: https://cosmonote.ai/en/api/
  type: http
- applies_to: Remote MCP server (https://nebula.cosmonote.ai/mcp)
  authorization_endpoint: https://nebula.cosmonote.ai/oauth/authorize
  bearer_methods_supported:
  - header
  description: The connection uses Streamable HTTP with OAuth 2.0 and PKCE. A Cosmonote sign-in page opens, you paste your API key, and you are connected.
  discovery: https://nebula.cosmonote.ai/.well-known/oauth-authorization-server
  flow: authorizationCode
  grant_types_supported:
  - authorization_code
  - refresh_token
  name: mcpOAuth
  note: Endpoint values read from the two well-known metadata documents (GET, HTTP 200, 2026-11-04); the authorize/token/register endpoints themselves were not called. Access is documented as read-only and user-scoped; no scopes are published.
  pkce: S256
  protected_resource_metadata: https://nebula.cosmonote.ai/.well-known/oauth-protected-resource
  registration_endpoint: https://nebula.cosmonote.ai/oauth/register
  token_endpoint: https://nebula.cosmonote.ai/oauth/token
  token_endpoint_auth_methods_supported:
  - none
  type: oauth2
slug: cosmonote-ai-authentication
source_filename: cosmonote-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://cosmonote.ai/en/api/\ndocs: https://cosmonote.ai/en/api/\ndocs_additional:\n- https://cosmonote.ai/en/mcp/\nschemes:\n- name: apiKeyBearer\n  type: http\n  scheme: bearer\n  applies_to: REST API (https://nebula.cosmonote.ai/api/v1)\n  header: 'Authorization: Bearer cnk_your_api_key'\n  key_prefix: cnk_\n  issuance: 'Find your API key in the app: Settings → API keys'\n  source: https://cosmonote.ai/en/api/\n- name: mcpOAuth\n  type: oauth2\n  flow: authorizationCode\n  pkce: S256\n  applies_to: Remote MCP server (https://nebula.cosmonote.ai/mcp)\n  description: The connection uses Streamable HTTP with OAuth 2.0 and PKCE. A Cosmonote sign-in page opens, you\n    paste your API key, and you are connected.\n  discovery: https://nebula.cosmonote.ai/.well-known/oauth-authorization-server\n  protected_resource_metadata: https://nebula.cosmonote.ai/.well-known/oauth-protected-resource\n  authorization_endpoint: https://nebula.cosmonote.ai/oauth/authorize\n\
  \  token_endpoint: https://nebula.cosmonote.ai/oauth/token\n  registration_endpoint: https://nebula.cosmonote.ai/oauth/register\n  grant_types_supported:\n  - authorization_code\n  - refresh_token\n  token_endpoint_auth_methods_supported:\n  - none\n  bearer_methods_supported:\n  - header\n  note: Endpoint values read from the two well-known metadata documents (GET, HTTP 200, 2026-11-04); the authorize/token/register\n    endpoints themselves were not called. Access is documented as read-only and user-scoped; no scopes are published.\n"
source_yaml_url: https://artifacts.apis.io/cosmonote-ai/authentication/cosmonote-ai-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Artificial Intelligence
- Note Taking
- Transcription
- Meetings
- Summarization
- MCP
- Productivity
---
