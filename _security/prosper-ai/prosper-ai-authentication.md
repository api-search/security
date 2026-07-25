---
api_key_in:
- header
api_specs:
- filename: prosper-ai-api-keys-api-openapi.yml
  format: yaml
  label: Prosper AI API Keys API
  slug: prosper-ai-api-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prosper-ai/refs/heads/main/openapi/prosper-ai-api-keys-api-openapi.yml
- filename: prosper-ai-call-logs-api-openapi.yml
  format: yaml
  label: Prosper AI Call Logs API
  slug: prosper-ai-call-logs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prosper-ai/refs/heads/main/openapi/prosper-ai-call-logs-api-openapi.yml
- filename: prosper-ai-campaigns-api-openapi.yml
  format: yaml
  label: Prosper AI Campaigns API
  slug: prosper-ai-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prosper-ai/refs/heads/main/openapi/prosper-ai-campaigns-api-openapi.yml
- filename: prosper-ai-live-calls-api-openapi.yml
  format: yaml
  label: Prosper AI Live Calls API
  slug: prosper-ai-live-calls-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prosper-ai/refs/heads/main/openapi/prosper-ai-live-calls-api-openapi.yml
- filename: prosper-ai-status-api-openapi.yml
  format: yaml
  label: Prosper AI Status API
  slug: prosper-ai-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prosper-ai/refs/heads/main/openapi/prosper-ai-status-api-openapi.yml
- filename: prosper-ai-targets-api-openapi.yml
  format: yaml
  label: Prosper AI Targets API
  slug: prosper-ai-targets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prosper-ai/refs/heads/main/openapi/prosper-ai-targets-api-openapi.yml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Prosper Ai Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Prosper AI secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Prosper AI
provider_slug: prosper-ai
scheme_count: 2
schemes:
- applies_to: REST API (/api/v1)
  description: API key created in the Prosper platform's API Keys section. Presented on each request. The exact header name is not published in the OpenAPI spec.
  in: header
  name: ApiKey
  source: https://docs.getprosperapp.com/introduction
  type: apiKey
- applies_to: MCP server (/mcp)
  flows:
  - authorizationUrl: https://voice.getprosperapp.com/mcp/authorize
    flow: authorizationCode
    pkce: S256
    registrationUrl: https://voice.getprosperapp.com/mcp/register
    revocationUrl: https://voice.getprosperapp.com/mcp/revoke
    scopes:
      read: Read access to Prosper resources via MCP
    tokenUrl: https://voice.getprosperapp.com/mcp/token
  name: MCP OAuth2
  source: https://voice.getprosperapp.com/.well-known/oauth-authorization-server
  type: oauth2
slug: prosper-ai-authentication
source_filename: prosper-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: >-\n  https://docs.getprosperapp.com/introduction +\n  https://voice.getprosperapp.com/.well-known/oauth-authorization-server\ndocs: https://docs.getprosperapp.com/introduction\nsummary:\n  types: [apiKey, oauth2]\n  api_key_in: [header]\n  oauth2_flows: [authorizationCode]\n  note: >-\n    The REST API (voice.getprosperapp.com/api/v1) authenticates with an API key\n    issued from the Prosper platform (API Keys section). The published OpenAPI\n    declares `security: []` and no securitySchemes, so the key mechanism is\n    documented in prose rather than the spec. The hosted MCP server at /mcp\n    authenticates with OAuth 2.0 (authorization code + PKCE, refresh tokens,\n    Dynamic Client Registration).\nschemes:\n- name: ApiKey\n  type: apiKey\n  in: header\n  applies_to: REST API (/api/v1)\n  description: >-\n    API key created in the Prosper platform's API Keys section. Presented on each\n    request. The exact header\
  \ name is not published in the OpenAPI spec.\n  source: https://docs.getprosperapp.com/introduction\n- name: MCP OAuth2\n  type: oauth2\n  applies_to: MCP server (/mcp)\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://voice.getprosperapp.com/mcp/authorize\n    tokenUrl: https://voice.getprosperapp.com/mcp/token\n    registrationUrl: https://voice.getprosperapp.com/mcp/register\n    revocationUrl: https://voice.getprosperapp.com/mcp/revoke\n    pkce: S256\n    scopes:\n      read: Read access to Prosper resources via MCP\n  source: https://voice.getprosperapp.com/.well-known/oauth-authorization-server\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/prosper-ai/refs/heads/main/authentication/prosper-ai-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- Company
- Healthcare
- Voice AI
- Revenue Cycle Management
- Patient Access
- EHR Integration
- AI Agents
- MCP
---
