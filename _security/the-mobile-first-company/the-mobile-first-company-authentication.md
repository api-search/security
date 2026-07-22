---
api_key_in:
- header
api_specs:
- filename: the-mobile-first-company-allo-openapi.json
  format: json
  label: Allo API
  slug: allo-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/the-mobile-first-company/refs/heads/main/openapi/the-mobile-first-company-allo-openapi.json
auth_types:
- apiKey
- oauth2
description: 'Every Allo API request requires authentication in the Authorization header. The primary method is a scoped API key (Settings > API) sent as `Authorization: Api-Key ak_live_<key>`. OAuth 2.0 is additionally supported for OAuth clients and the hosted MCP server (authorization server api.withallo.com). API access is not available on trial plans.'
kind: authentication
layout: security
method: searched
name: The Mobile First Company Authentication
name_suffix: Authentication
oauth_flows: []
overview: The Mobile First Company secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: The Mobile First Company
provider_slug: the-mobile-first-company
scheme_count: 2
schemes:
- description: Scoped API key. Live keys use the ak_live_ prefix. Keys are scoped to a single team, can be revoked at any time, and carry one or more of the scopes in scopes/the-mobile-first-company-scopes.yml. Per-endpoint scope requirements are documented in the authentication guide's scope-to-endpoint mapping.
  format: Api-Key ak_live_<key>
  in: header
  name: ApiKeyAuth
  parameter: Authorization
  sources:
  - openapi/the-mobile-first-company-allo-openapi.json
  - https://help.withallo.com/en/v2/api-reference/guides/authentication
  type: apiKey
- authorization_endpoint: https://api.withallo.com/v1/oauth/authorize
  description: OAuth 2.0 (RFC 8414 metadata at well-known/the-mobile-first-company-oauth-authorization-server.json). Used by the Claude Connector and other OAuth clients; the hosted MCP server is an OAuth protected resource against this authorization server.
  flows:
  - authorization_code (PKCE S256)
  - client_credentials
  - refresh_token
  name: OAuth2
  revocation_endpoint: https://api.withallo.com/v1/oauth/revoke
  sources:
  - well-known/the-mobile-first-company-oauth-authorization-server.json
  - https://www.withallo.com/mcp
  token_endpoint: https://api.withallo.com/v1/oauth/token
  type: oauth2
slug: the-mobile-first-company-authentication
source_filename: the-mobile-first-company-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\ndocs: https://help.withallo.com/en/v2/api-reference/guides/authentication\nsource: >-\n  openapi/the-mobile-first-company-allo-openapi.json securitySchemes +\n  Allo authentication guide + OAuth authorization-server metadata\napi: Allo API\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - header\nprimary: api_key\ndescription: >-\n  Every Allo API request requires authentication in the Authorization header.\n  The primary method is a scoped API key (Settings > API) sent as\n  `Authorization: Api-Key ak_live_<key>`. OAuth 2.0 is additionally supported\n  for OAuth clients and the hosted MCP server (authorization server\n  api.withallo.com). API access is not available on trial plans.\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  format: 'Api-Key ak_live_<key>'\n  description: >-\n    Scoped API key. Live keys use the ak_live_ prefix. Keys are scoped to a\n    single team, can\
  \ be revoked at any time, and carry one or more of the scopes\n    in scopes/the-mobile-first-company-scopes.yml. Per-endpoint scope\n    requirements are documented in the authentication guide's scope-to-endpoint\n    mapping.\n  sources:\n  - openapi/the-mobile-first-company-allo-openapi.json\n  - https://help.withallo.com/en/v2/api-reference/guides/authentication\n- name: OAuth2\n  type: oauth2\n  flows:\n  - authorization_code (PKCE S256)\n  - client_credentials\n  - refresh_token\n  authorization_endpoint: https://api.withallo.com/v1/oauth/authorize\n  token_endpoint: https://api.withallo.com/v1/oauth/token\n  revocation_endpoint: https://api.withallo.com/v1/oauth/revoke\n  description: >-\n    OAuth 2.0 (RFC 8414 metadata at\n    well-known/the-mobile-first-company-oauth-authorization-server.json). Used by\n    the Claude Connector and other OAuth clients; the hosted MCP server is an\n    OAuth protected resource against this authorization server.\n  sources:\n  - well-known/the-mobile-first-company-oauth-authorization-server.json\n\
  \  - https://www.withallo.com/mcp\nspec_scheme_aliases:\n  note: >-\n    The spec also exposes scope-specific apiKey scheme aliases, all sent in the\n    Authorization header and differing only by the scope the key must carry.\n  aliases:\n  - name: CallsAuth\n    scope: CONVERSATIONS_READ\n  - name: ContactsAuth\n    scope: CONTACTS_READ\n  - name: ContactsWriteAuth\n    scope: CONTACTS_READ_WRITE\n  - name: SmsAuth\n    scope: SMS_SEND\nerrors:\n  invalid_key:\n    status: 401\n    code: API_KEY_INVALID\n  insufficient_scope:\n    status: 403\n    code: API_KEY_INSUFFICIENT_SCOPE\n  trial_not_allowed:\n    status: 403\n    code: API_KEY_TRIAL_NOT_ALLOWED\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/the-mobile-first-company/refs/heads/main/authentication/the-mobile-first-company-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- Company
- Communication
- Telephony
- Voice
- SMS
- CRM
- Artificial Intelligence
- MCP
- Webhooks
- Small Business
---
