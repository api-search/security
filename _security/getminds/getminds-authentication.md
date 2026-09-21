---
anonymous_access: false
api_key_in: []
api_specs:
- filename: getminds-openapi.json
  format: json
  label: Minds Public API
  slug: minds-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/getminds/refs/heads/main/openapi/getminds-openapi.json
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Getminds Authentication
name_suffix: Authentication
oauth_flows: []
overview: Minds secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Minds
provider_slug: getminds
scheme_count: 2
schemes:
- bearerFormat: API Key
  description: 'Personal API key sent as `Authorization: Bearer minds_…`. Keys are prefixed `minds_`, created at https://getminds.ai/settings/api-keys, shown once at creation, and never returned again. `GET /api/v1/auth/me` verifies a key. A missing/invalid/revoked key returns a generic 401 (the API deliberately does not distinguish among them).'
  docs: https://getminds.ai/docs/api/authentication
  header: Authorization
  key_prefix: minds_
  name: ApiKeyAuth
  scheme: bearer
  sources:
  - openapi/getminds-openapi.json
  - https://getminds.ai/docs/api/authentication
  surface: rest
  type: http
- authorization_endpoint: https://getminds.ai/oauth/authorize
  description: RFC 9728 protected-resource metadata is served at /.well-known/oauth-protected-resource; the authorization server metadata (RFC 8414) and OpenID configuration are served on the same host. Public client (token_endpoint_auth_method none) with PKCE and dynamic client registration. The MCP server also accepts a Minds API key in place of OAuth.
  docs: https://getminds.ai/mcp/setup
  dynamic_client_registration: true
  flow: authorization_code
  name: MCP OAuth2
  pkce: S256
  protected_resource: https://getminds.ai/mcp
  registration_endpoint: https://getminds.ai/oauth/register
  revocation_endpoint: https://getminds.ai/oauth/revoke
  scopes:
  - sparks:read
  - sparks:write
  - sparks:chat
  - flows:read
  - flows:write
  sources:
  - well-known/getminds-oauth-authorization-server.json
  - well-known/getminds-oauth-protected-resource.json
  - well-known/getminds-openid-configuration.json
  surface: mcp
  token_endpoint: https://getminds.ai/oauth/token
  token_endpoint_auth_methods:
  - none
  type: oauth2
slug: getminds-authentication
source_filename: getminds-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-20'\nmethod: searched\nsource: https://getminds.ai/docs/api/authentication\nsummary:\n  types:\n  - http\n  - oauth2\n  note: >-\n    REST v1 API uses a personal API key sent as a bearer token. The MCP server\n    (https://getminds.ai/mcp) is a separate protected resource that uses OAuth 2.0\n    (or the same API key). The OpenAPI document itself is intentionally public.\nschemes:\n- name: ApiKeyAuth\n  surface: rest\n  type: http\n  scheme: bearer\n  bearerFormat: API Key\n  key_prefix: minds_\n  header: Authorization\n  description: >-\n    Personal API key sent as `Authorization: Bearer minds_…`. Keys are prefixed\n    `minds_`, created at https://getminds.ai/settings/api-keys, shown once at\n    creation, and never returned again. `GET /api/v1/auth/me` verifies a key.\n    A missing/invalid/revoked key returns a generic 401 (the API deliberately\n    does not distinguish among them).\n  docs: https://getminds.ai/docs/api/authentication\n  sources:\n\
  \  - openapi/getminds-openapi.json\n  - https://getminds.ai/docs/api/authentication\n- name: MCP OAuth2\n  surface: mcp\n  type: oauth2\n  flow: authorization_code\n  pkce: S256\n  dynamic_client_registration: true\n  token_endpoint_auth_methods:\n  - none\n  authorization_endpoint: https://getminds.ai/oauth/authorize\n  token_endpoint: https://getminds.ai/oauth/token\n  registration_endpoint: https://getminds.ai/oauth/register\n  revocation_endpoint: https://getminds.ai/oauth/revoke\n  protected_resource: https://getminds.ai/mcp\n  scopes:\n  - sparks:read\n  - sparks:write\n  - sparks:chat\n  - flows:read\n  - flows:write\n  description: >-\n    RFC 9728 protected-resource metadata is served at\n    /.well-known/oauth-protected-resource; the authorization server metadata\n    (RFC 8414) and OpenID configuration are served on the same host. Public\n    client (token_endpoint_auth_method none) with PKCE and dynamic client\n    registration. The MCP server also accepts a Minds API key in\
  \ place of OAuth.\n  docs: https://getminds.ai/mcp/setup\n  sources:\n  - well-known/getminds-oauth-authorization-server.json\n  - well-known/getminds-oauth-protected-resource.json\n  - well-known/getminds-openid-configuration.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/getminds/refs/heads/main/authentication/getminds-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Synthetic Research
- Market Research
- Surveys
- User Research
- Marketing Analytics
- ai-personas
- MCP
- agent-native
- GDPR
---
