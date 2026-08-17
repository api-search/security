---
api_key_in:
- header
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Adverity Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Adverity secures its APIs with apiKey and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Adverity
provider_slug: adverity
scheme_count: 3
schemes:
- description: API keys generated programmatically via POST https://{{INSTANCE}}/api/auth/token/ (username + password, application/x-www-form-urlencoded). The response returns {username, token, expires_in} with expires_in null — the token does not expire and is only rotated when the account password is deliberately changed (profile settings, password reset, or an administrator reset). Adverity recommends a dedicated service account for long-lived integrations. These keys inherit the user's permissions and CANNOT call the user-management endpoints.
  format: Token {{KEY}}
  in: header
  name: ManagementApiToken
  parameter: Authorization
  sources:
  - docs
  type: apiKey
- description: API keys generated in the Adverity UI (Administration > Management API keys). Assigned to a single workspace and valid for that workspace and its children. Maximum 5 keys per workspace; creation requires Administrator permissions in the root workspace. Keys do not expire, are shown exactly once at creation, carry per-resource scopes set to No access / Read-only / Write, and are the only keys that may call user-management endpoints.
  format: Bearer {{KEY}}
  in: header
  name: ManagementApiBearer
  parameter: Authorization
  scopes_ref: scopes/adverity-scopes.yml
  sources:
  - docs
  type: apiKey
- authorizationUrl: https://mcp.eu.adverity.com/authorize
  description: Guards the remote MCP endpoint https://mcp.eu.adverity.com/mcp. The MCP client registers dynamically and runs an authorization-code flow; at Adverity's sign-in page the user supplies their Instance URL and MAPI key, so the agent's effective authority is exactly that key's scopes. Since release 2026.30 the server introspects the underlying API key on token refresh, so a revoked or rotated key invalidates the agent session immediately.
  flow: authorizationCode
  grant_types:
  - authorization_code
  - refresh_token
  name: AdverityMcpOAuth
  pkce: S256
  probed: '2026-08-13'
  registrationUrl: https://mcp.eu.adverity.com/register
  scopes_supported: []
  sources:
  - https://mcp.eu.adverity.com/.well-known/oauth-authorization-server
  - https://docs.adverity.com/guides/mcp/mcp-setup.html
  tokenUrl: https://mcp.eu.adverity.com/token
  token_endpoint_auth_methods:
  - client_secret_post
  - client_secret_basic
  type: oauth2
slug: adverity-authentication
source_filename: adverity-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://docs.adverity.com/guides/management-api/authorizing-to-management-api.html\ndocs: https://docs.adverity.com/guides/management-api/authorizing-to-management-api.html\nsummary:\n  types: [apiKey, oauth2]\n  api_key_in: [header]\n  oauth2_flows: [authorizationCode]\n  note: >-\n    The Adverity Management API uses long-lived API-key (token) authentication in the\n    Authorization header — there is no OAuth2 on the Management API itself. OAuth2 appears in\n    two other places: the remote MCP server runs its own OAuth 2.0 authorization server\n    (authorization code + refresh, PKCE S256, dynamic client registration) in front of the\n    same MAPI key, and OAuth is used downstream when Adverity authorizes to connected data\n    sources (Google Ads, Facebook Ads, LinkedIn Ads) on the customer's behalf.\nschemes:\n- name: ManagementApiToken\n  type: apiKey\n  in: header\n  parameter: Authorization\n  format: 'Token {{KEY}}'\n\
  \  description: >-\n    API keys generated programmatically via POST https://{{INSTANCE}}/api/auth/token/\n    (username + password, application/x-www-form-urlencoded). The response returns\n    {username, token, expires_in} with expires_in null — the token does not expire and is\n    only rotated when the account password is deliberately changed (profile settings,\n    password reset, or an administrator reset). Adverity recommends a dedicated service\n    account for long-lived integrations. These keys inherit the user's permissions and\n    CANNOT call the user-management endpoints.\n  sources: [docs]\n- name: ManagementApiBearer\n  type: apiKey\n  in: header\n  parameter: Authorization\n  format: 'Bearer {{KEY}}'\n  description: >-\n    API keys generated in the Adverity UI (Administration > Management API keys). Assigned\n    to a single workspace and valid for that workspace and its children. Maximum 5 keys per\n    workspace; creation requires Administrator permissions in the root\
  \ workspace. Keys do\n    not expire, are shown exactly once at creation, carry per-resource scopes set to No\n    access / Read-only / Write, and are the only keys that may call user-management\n    endpoints.\n  scopes_ref: scopes/adverity-scopes.yml\n  sources: [docs]\n- name: AdverityMcpOAuth\n  type: oauth2\n  flow: authorizationCode\n  authorizationUrl: https://mcp.eu.adverity.com/authorize\n  tokenUrl: https://mcp.eu.adverity.com/token\n  registrationUrl: https://mcp.eu.adverity.com/register\n  pkce: S256\n  grant_types: [authorization_code, refresh_token]\n  token_endpoint_auth_methods: [client_secret_post, client_secret_basic]\n  description: >-\n    Guards the remote MCP endpoint https://mcp.eu.adverity.com/mcp. The MCP client registers\n    dynamically and runs an authorization-code flow; at Adverity's sign-in page the user\n    supplies their Instance URL and MAPI key, so the agent's effective authority is exactly\n    that key's scopes. Since release 2026.30 the server introspects\
  \ the underlying API key\n    on token refresh, so a revoked or rotated key invalidates the agent session immediately.\n  scopes_supported: []\n  sources: [https://mcp.eu.adverity.com/.well-known/oauth-authorization-server, https://docs.adverity.com/guides/mcp/mcp-setup.html]\n  probed: '2026-08-13'\nkey_lifecycle:\n  create_programmatic: POST /api/auth/token/\n  create_ui: Administration > Management API keys (max 5 per workspace)\n  rotate: POST /api/v1/auth/keys/current/rotate/\n  introspect: GET /api/v1/auth/keys/introspect/\n  introspect_note: >-\n    Added 2026.30; unauthenticated route, IP-rate-limited. Returns active status and key\n    details so a caller can verify key validity before use.\n  revoke: Administration > Management API keys\n  expiry: none\n  displayed_once: true\ndownstream_oauth:\n  note: >-\n    Adverity holds OAuth credentials for the customer's connected marketing platforms\n    (authorizations). Those are managed through /api/connection-types/{type_id}/connections/\n\
  \    and the manage_authorization MCP tool, including account-level collection permissions and\n    a grant-all flag. Updating permissions is a full replacement.\nrelated:\n- scopes/adverity-scopes.yml\n- conventions/adverity-conventions.yml\n- mcp/adverity-mcp.yml\n- well-known/adverity-oauth-authorization-server.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/adverity/refs/heads/main/authentication/adverity-authentication.yml
summary_line: apiKey/oauth2 · 3 schemes
tags:
- Company
- Data Analytics
- Marketing Analytics
- Data Integration
- ETL
- Business Intelligence
- Marketing Intelligence
- MCP
---
