---
anonymous_access: false
api_key_in: []
auth_types: []
description: Vinkius has two credential planes - an application key for the REST API (api.vinkius.com) and connection tokens / OAuth for the MCP Edge (edge.vinkius.com).
kind: authentication
layout: security
mechanism_count: 4
method: searched
name: Vinkius Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: Vinkius declares 4 security scheme(s) across its OpenAPI definitions.
provider_name: Vinkius
provider_slug: vinkius-com
scheme_count: 4
schemes:
- detail: The SDK is initialised with a public application id (vk_app_*) and one secret application key (vk_app_sk_*). The secret is sent only as an Authorization Bearer header over HTTPS and must stay server-side. A leaked key is scoped to a single application; cross-tenant access returns 404.
  environments: Use different App IDs and keys for development, staging and live traffic.
  id: application-key
  key_prefixes:
  - vk_app_
  - vk_app_sk_
  observed: GET https://api.vinkius.com/catalog/mcps without a key returns 401 {"error":"Unauthenticated."}
  scheme: bearer
  surface: https://api.vinkius.com
  type: http
  user_scope: Every user operation is additionally addressed by an externalId in the route (/apps/{app}/users/{externalId}/...); internal ids are prefixed vk_app_user_.
- detail: MCP clients connect to https://edge.vinkius.com/{token}/mcp where the token is a vk_live_* connection token shown once in the Vinkius Cloud console. The runtime token never reaches the Connect SDK - execution is proxied by the API.
  docs: https://vinkius.com/learn/en/tokens
  id: connection-token
  in: path
  key_prefixes:
  - vk_live_
  surface: https://edge.vinkius.com
  type: apiKey
- dynamic_client_registration: https://edge.vinkius.com/oauth/register
  flows:
  - authorization_code
  - refresh_token
  id: edge-oauth
  metadata: well-known/vinkius-com-edge-oauth-authorization-server.json
  pkce: S256
  scopes: scopes/vinkius-com-scopes.yml
  surface: https://edge.vinkius.com
  token_endpoint_auth_methods:
  - none
  - client_secret_post
  type: oauth2
- detail: Console sign-in with Google or GitHub; SSO with SAML or OIDC on the Business plan (pricing page).
  id: console-sso
  surface: https://cloud.vinkius.com
slug: vinkius-com-authentication
source_filename: vinkius-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-20'\nmethod: searched\nsource: https://vinkius.com/learn/en/connect-sdk/authentication, https://github.com/vinkius-labs/ai-connect-sdk/blob/main/SECURITY.md, https://edge.vinkius.com/.well-known/oauth-authorization-server\ndocs: https://vinkius.com/learn/en/connect-sdk/authentication\ndescription: Vinkius has two credential planes - an application key for the REST API (api.vinkius.com) and connection tokens / OAuth for the MCP Edge (edge.vinkius.com).\nschemes:\n- id: application-key\n  surface: https://api.vinkius.com\n  type: http\n  scheme: bearer\n  detail: >-\n    The SDK is initialised with a public application id (vk_app_*) and one secret application key\n    (vk_app_sk_*). The secret is sent only as an Authorization Bearer header over HTTPS and must stay\n    server-side. A leaked key is scoped to a single application; cross-tenant access returns 404.\n  key_prefixes: [vk_app_, vk_app_sk_]\n  user_scope: Every user operation is additionally addressed\
  \ by an externalId in the route (/apps/{app}/users/{externalId}/...); internal ids are prefixed vk_app_user_.\n  environments: Use different App IDs and keys for development, staging and live traffic.\n  observed: GET https://api.vinkius.com/catalog/mcps without a key returns 401 {\"error\":\"Unauthenticated.\"}\n- id: connection-token\n  surface: https://edge.vinkius.com\n  type: apiKey\n  in: path\n  detail: MCP clients connect to https://edge.vinkius.com/{token}/mcp where the token is a vk_live_* connection token shown once in the Vinkius Cloud console. The runtime token never reaches the Connect SDK - execution is proxied by the API.\n  key_prefixes: [vk_live_]\n  docs: https://vinkius.com/learn/en/tokens\n- id: edge-oauth\n  surface: https://edge.vinkius.com\n  type: oauth2\n  flows: [authorization_code, refresh_token]\n  pkce: S256\n  dynamic_client_registration: https://edge.vinkius.com/oauth/register\n  token_endpoint_auth_methods: [none, client_secret_post]\n  scopes: scopes/vinkius-com-scopes.yml\n\
  \  metadata: well-known/vinkius-com-edge-oauth-authorization-server.json\n- id: console-sso\n  surface: https://cloud.vinkius.com\n  detail: Console sign-in with Google or GitHub; SSO with SAML or OIDC on the Business plan (pricing page).\ncredentials_storage: End-user connector credentials are write-only - set through the API and never returned; the SDK reports only which keys are configured.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vinkius-com/refs/heads/main/authentication/vinkius-com-authentication.yml
summary_line: 4 schemes
tags:
- Company
- MCP
- AI Agents
- Integration
- Connectors
- AI Governance
- Developer Tools
- Agent-Native
---
