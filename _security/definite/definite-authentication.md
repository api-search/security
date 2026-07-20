---
api_key_in: []
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Definite Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Definite secures its APIs with http and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Definite
provider_slug: definite
scheme_count: 3
schemes:
- format: '{user_id}-{api_key_suffix}'
  header: Authorization
  location: header
  name: apiKeyBearer
  note: 'Primary REST API auth. Send "Authorization: Bearer <API_KEY>". API keys are created/copied from the bottom-left user menu in the Definite app. Used across the v1 REST API, v3 MCP HTTP endpoint, and v4 webhook endpoints.'
  scheme: bearer
  type: http
- flows:
  - authorizationUrl: https://api.definite.app/oauth/authorize
    flow: authorizationCode
    pkce: S256
    scopes:
      mcp: Access the Definite MCP server tools.
    tokenUrl: https://api.definite.app/oauth/token
  name: oauth2Mcp
  note: OAuth 2.1 authorization-code + PKCE flow advertised for MCP clients; refresh_token grant supported; token_endpoint_auth_methods_supported none (public client).
  source: /.well-known/oauth-authorization-server
  type: oauth2
- name: sso
  note: Enterprise SSO via SAML / OIDC (Google Workspace) for app + on-prem sign-in; documented on the security page and on-prem SSO docs.
  type: openIdConnect
slug: definite-authentication
source_filename: definite-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://www.definite.app/docs/definite-api\ndocs:\n- https://www.definite.app/docs/definite-api\n- https://www.definite.app/docs/mcp/mcp\n- https://www.definite.app/security\nsummary:\n  types: [http, oauth2]\n  http_schemes: [bearer]\n  oauth2_flows: [authorizationCode]\n  sso: [SAML, OIDC, Google Workspace]\nschemes:\n- name: apiKeyBearer\n  type: http\n  scheme: bearer\n  location: header\n  header: Authorization\n  format: '{user_id}-{api_key_suffix}'\n  note: >-\n    Primary REST API auth. Send \"Authorization: Bearer <API_KEY>\". API keys are\n    created/copied from the bottom-left user menu in the Definite app. Used\n    across the v1 REST API, v3 MCP HTTP endpoint, and v4 webhook endpoints.\n- name: oauth2Mcp\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.definite.app/oauth/authorize\n    tokenUrl: https://api.definite.app/oauth/token\n    pkce: S256\n    scopes:\n      mcp:\
  \ Access the Definite MCP server tools.\n  source: /.well-known/oauth-authorization-server\n  note: >-\n    OAuth 2.1 authorization-code + PKCE flow advertised for MCP clients;\n    refresh_token grant supported; token_endpoint_auth_methods_supported none\n    (public client).\n- name: sso\n  type: openIdConnect\n  note: >-\n    Enterprise SSO via SAML / OIDC (Google Workspace) for app + on-prem sign-in;\n    documented on the security page and on-prem SSO docs.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/definite/refs/heads/main/authentication/definite-authentication.yml
summary_line: http/oauth2 · 3 schemes
tags:
- Company
- Data
- Analytics
- Business Intelligence
- Data Integration
- Data Warehouse
- Lakehouse
- Semantic Layer
- Artificial Intelligence
- AI Agents
- Model Context Protocol
- ETL
---
