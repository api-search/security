---
api_key_in:
- header
auth_types:
- apiKey
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Wisdom Ai Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Wisdom AI secures its APIs with apiKey, http, and oauth2 across 4 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Wisdom AI
provider_slug: wisdom-ai
scheme_count: 4
schemes:
- description: Every WisdomAI user can create and manage their own long-lived API access keys from the API Keys settings page. The access key is a bearer credential exchanged for a short-lived JWT session token via the exchangeAccessToken GraphQL query; the raw access key is a server-side secret and must never reach the browser.
  docs: https://docs.wisdom.ai/settings/api-keys
  name: API access key
  type: apiKey
- description: 'Short-lived JWT session token (issued by Descope) passed as "Authorization: Bearer YOUR_SESSION_TOKEN" on every GraphQL request and in WebSocket subscription connection payloads. Obtained by exchanging an API access key with the exchangeAccessToken query.'
  name: JWT session token (Bearer)
  operations:
  - exchangeAccessToken
  scheme: bearer
  type: http
- description: For embedding scenarios, the backend uses @wisdomai/node to mint a short-lived per-user JWT (via impersonateUser with a Descope management key), which WisdomProvider consumes in the browser and auto-refreshes before expiry.
  name: Embedded user impersonation
  operations:
  - impersonateUser
  scheme: bearer
  type: http
- description: The hosted MCP server authenticates with OAuth 2.1 using Dynamic Client Registration (DCR) and PKCE; clients register automatically with no manual setup. Discovery at /.well-known/oauth-protected-resource and /.well-known/oauth-authorization-server.
  docs: https://docs.wisdom.ai/integrations/mcp-server/MCP-Server
  flows:
  - dynamic_client_registration: true
    flow: authorizationCode
    pkce: true
  name: MCP OAuth 2.1
  type: oauth2
slug: wisdom-ai-authentication
source_filename: wisdom-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://docs.wisdom.ai/integrations/graphql-api/GraphQL-API\ndocs: https://docs.wisdom.ai/settings/api-keys\nsummary:\n  types: [apiKey, http, oauth2]\n  api_key_in: [header]\n  http_scheme: bearer\n  oauth2_flows: [authorizationCode]\n  identity_provider: Descope\nschemes:\n- name: API access key\n  type: apiKey\n  description: >-\n    Every WisdomAI user can create and manage their own long-lived API access\n    keys from the API Keys settings page. The access key is a bearer credential\n    exchanged for a short-lived JWT session token via the exchangeAccessToken\n    GraphQL query; the raw access key is a server-side secret and must never\n    reach the browser.\n  docs: https://docs.wisdom.ai/settings/api-keys\n- name: JWT session token (Bearer)\n  type: http\n  scheme: bearer\n  description: >-\n    Short-lived JWT session token (issued by Descope) passed as\n    \"Authorization: Bearer YOUR_SESSION_TOKEN\" on every GraphQL\
  \ request and in\n    WebSocket subscription connection payloads. Obtained by exchanging an API\n    access key with the exchangeAccessToken query.\n  operations: [exchangeAccessToken]\n- name: Embedded user impersonation\n  type: http\n  scheme: bearer\n  description: >-\n    For embedding scenarios, the backend uses @wisdomai/node to mint a\n    short-lived per-user JWT (via impersonateUser with a Descope management key),\n    which WisdomProvider consumes in the browser and auto-refreshes before expiry.\n  operations: [impersonateUser]\n- name: MCP OAuth 2.1\n  type: oauth2\n  description: >-\n    The hosted MCP server authenticates with OAuth 2.1 using Dynamic Client\n    Registration (DCR) and PKCE; clients register automatically with no manual\n    setup. Discovery at /.well-known/oauth-protected-resource and\n    /.well-known/oauth-authorization-server.\n  flows:\n  - flow: authorizationCode\n    pkce: true\n    dynamic_client_registration: true\n  docs: https://docs.wisdom.ai/integrations/mcp-server/MCP-Server\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wisdom-ai/refs/heads/main/authentication/wisdom-ai-authentication.yml
summary_line: apiKey/http/oauth2 · 4 schemes
tags:
- Company
- AI
- Analytics
- Business Intelligence
- GraphQL
- MCP
- Embedded Analytics
- Agents
- Data
---
