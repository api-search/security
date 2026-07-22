---
api_key_in: []
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Reltio Authentication
name_suffix: Authentication
oauth_flows:
- password
- clientCredentials
- authorizationCode
overview: Reltio secures its APIs with oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the password, clientCredentials, and authorizationCode flow(s).
provider_name: Reltio
provider_slug: reltio
scheme_count: 2
schemes:
- description: 'Reltio REST APIs are authorized with OAuth 2.0 bearer access tokens. Tokens are obtained from the Reltio auth service; the token is passed as an Authorization: Bearer <access_token> header on every API request.'
  flows:
  - description: Resource-owner password grant (username/password) — common for user-context REST access
    flow: password
  - description: Client credentials grant — used by the open-source MCP Server (Developer Edition) and server-to-server integrations
    flow: clientCredentials
  name: ReltioOAuth2
  token_endpoint: https://auth.reltio.com/oauth/token
  type: oauth2
- authorization_endpoint: https://login.reltio.com
  description: OAuth 2.0 server fronting the Reltio AgentFlow MCP / AI Tools surface, with OpenID-style dynamic client registration and PKCE.
  flows:
  - description: Authorization code with PKCE (S256); client_secret_basic token auth
    flow: authorizationCode
  issuer: https://dev.reltio.com/ai/tools
  name: ReltioAIToolsOAuth2
  registration_endpoint: https://dev.reltio.com/ai/tools/register
  source: dev.reltio.com/.well-known/oauth-authorization-server
  token_endpoint: https://login.reltio.com/token
  type: oauth2
slug: reltio-authentication
source_filename: reltio-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://docs.reltio.com/en/developer-resources\ndocs: https://docs.reltio.com/en/developer-resources\nnotes: >-\n  No public OpenAPI is available for the Reltio REST API (tenant-scoped,\n  auth-gated), so this profile is searched from the developer docs and the\n  live OAuth authorization-server discovery document rather than derived.\nsummary:\n  types: [oauth2]\n  api_key_in: []\n  oauth2_flows: [password, clientCredentials, authorizationCode]\nschemes:\n- name: ReltioOAuth2\n  type: oauth2\n  description: >-\n    Reltio REST APIs are authorized with OAuth 2.0 bearer access tokens.\n    Tokens are obtained from the Reltio auth service; the token is passed as\n    an Authorization: Bearer <access_token> header on every API request.\n  token_endpoint: https://auth.reltio.com/oauth/token\n  flows:\n  - flow: password\n    description: Resource-owner password grant (username/password) — common for user-context REST access\n \
  \ - flow: clientCredentials\n    description: Client credentials grant — used by the open-source MCP Server (Developer Edition) and server-to-server integrations\n- name: ReltioAIToolsOAuth2\n  type: oauth2\n  description: >-\n    OAuth 2.0 server fronting the Reltio AgentFlow MCP / AI Tools surface, with\n    OpenID-style dynamic client registration and PKCE.\n  source: dev.reltio.com/.well-known/oauth-authorization-server\n  issuer: https://dev.reltio.com/ai/tools\n  authorization_endpoint: https://login.reltio.com\n  token_endpoint: https://login.reltio.com/token\n  registration_endpoint: https://dev.reltio.com/ai/tools/register\n  flows:\n  - flow: authorizationCode\n    description: Authorization code with PKCE (S256); client_secret_basic token auth\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/reltio/refs/heads/main/authentication/reltio-authentication.yml
summary_line: oauth2 · 2 schemes
tags:
- Company
- Data Analytics
- Master Data Management
- MDM
- Entity Resolution
- Data Quality
- Data Integration
- AI Agents
- MCP
- SAP
---
