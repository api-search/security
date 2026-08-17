---
api_key_in:
- header
api_specs:
- filename: postiz-analytics-api-openapi.yml
  format: yaml
  label: Postiz Analytics API
  slug: postiz-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/postiz/refs/heads/main/openapi/postiz-analytics-api-openapi.yml
- filename: postiz-integrations-api-openapi.yml
  format: yaml
  label: Postiz Integrations API
  slug: postiz-integrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/postiz/refs/heads/main/openapi/postiz-integrations-api-openapi.yml
- filename: postiz-notifications-api-openapi.yml
  format: yaml
  label: Postiz Notifications API
  slug: postiz-notifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/postiz/refs/heads/main/openapi/postiz-notifications-api-openapi.yml
- filename: postiz-posts-api-openapi.yml
  format: yaml
  label: Postiz Posts API
  slug: postiz-posts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/postiz/refs/heads/main/openapi/postiz-posts-api-openapi.yml
- filename: postiz-uploads-api-openapi.yml
  format: yaml
  label: Postiz Uploads API
  slug: postiz-uploads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/postiz/refs/heads/main/openapi/postiz-uploads-api-openapi.yml
- filename: postiz-public-api-openapi.json
  format: json
  label: Postiz Public API
  slug: postiz-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/postiz/refs/heads/main/openapi/postiz-public-api-openapi.json
- filename: postiz-platform-swagger-openapi.json
  format: json
  label: Postiz Platform API
  slug: postiz-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/postiz/refs/heads/main/openapi/postiz-platform-swagger-openapi.json
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Postiz Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- deviceFlow
overview: Postiz secures its APIs with apiKey and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and deviceFlow flow(s).
provider_name: Postiz
provider_slug: postiz
scheme_count: 3
schemes:
- description: Your Postiz API key.
  in: header
  name: ApiKeyAuth
  parameter: Authorization
  scheme_note: The raw key is the entire header value — there is no Bearer prefix on the Public API. Obtained from Settings > Developers > Public API.
  sources:
  - openapi/postiz-public-api-openapi.json
  - openapi/_original/postiz-openapi.yml
  type: apiKey
- authorizationUrl: https://platform.postiz.com/oauth/authorize
  client_id_prefix: pca_
  client_secret_prefix: pcs_
  code_lifetime: 10 minutes, single use
  flow: authorizationCode
  name: PostizOAuth2
  pkce: S256 (advertised in the MCP authorization-server metadata)
  scopes:
  - mcp:read
  - mcp:write
  scopes_note: Scopes are advertised for the MCP resource only; the Public API OAuth flow documents no scope parameter. See scopes/postiz-scopes.yml.
  sources:
  - https://docs.postiz.com/public-api/oauth
  - well-known/postiz-oauth-authorization-server-mcp-oauth.json
  state_parameter: supported, recommended for CSRF protection
  tokenUrl: https://api.postiz.com/oauth/token
  token_lifetime: does not expire; user-revocable from Settings > Approved Apps
  token_prefix: pos_
  type: oauth2
  usage: 'The pos_ token is sent as the Authorization header value, exactly like an API key, and works against every Public API endpoint. On the MCP endpoint it is sent as "Authorization: Bearer <token>".'
- auth_server: https://cli-auth.postiz.com
  description: '`postiz auth:login` runs an OAuth2 device flow through a hosted auth server that mediates the standard authorization-code exchange, so CLI users never handle a client id or secret. Credentials are stored at ~/.postiz/credentials.json. Self-hosters can run their own auth server (gitroomhq/postiz-agent, server/).'
  flow: deviceCode
  name: PostizCLIDeviceFlow
  precedence: OAuth2 credentials take priority over POSTIZ_API_KEY when both are present.
  sources:
  - https://docs.postiz.com/cli/authentication
  type: oauth2
slug: postiz-authentication
source_filename: postiz-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: openapi/postiz-public-api-openapi.json\ndocs:\n- https://docs.postiz.com/public-api/introduction\n- https://docs.postiz.com/public-api/oauth\n- https://docs.postiz.com/mcp/introduction\n- https://docs.postiz.com/cli/authentication\nnote: >-\n  Upgraded from the spec-derived profile. The OpenAPI declares one apiKey scheme, but\n  Postiz documents three authentication paths in practice: a raw API key, an OAuth2\n  authorization-code token for third-party apps, and an OAuth2 device flow used by the\n  CLI. All three are sent in the same Authorization header, and OAuth tokens are\n  accepted anywhere an API key is.\nsummary:\n  types: [apiKey, oauth2]\n  api_key_in: [header]\n  oauth2_flows: [authorizationCode, deviceFlow]\n  transport: https\n  key_rotation: manual (regenerate in Settings; keys do not auto-rotate)\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  scheme_note: >-\n    The\
  \ raw key is the entire header value — there is no Bearer prefix on the Public\n    API. Obtained from Settings > Developers > Public API.\n  description: Your Postiz API key.\n  sources: [openapi/postiz-public-api-openapi.json, openapi/_original/postiz-openapi.yml]\n- name: PostizOAuth2\n  type: oauth2\n  flow: authorizationCode\n  authorizationUrl: https://platform.postiz.com/oauth/authorize\n  tokenUrl: https://api.postiz.com/oauth/token\n  token_prefix: pos_\n  client_id_prefix: pca_\n  client_secret_prefix: pcs_\n  pkce: S256 (advertised in the MCP authorization-server metadata)\n  code_lifetime: 10 minutes, single use\n  token_lifetime: does not expire; user-revocable from Settings > Approved Apps\n  state_parameter: supported, recommended for CSRF protection\n  scopes: [mcp:read, mcp:write]\n  scopes_note: >-\n    Scopes are advertised for the MCP resource only; the Public API OAuth flow\n    documents no scope parameter. See scopes/postiz-scopes.yml.\n  usage: >-\n    The pos_\
  \ token is sent as the Authorization header value, exactly like an API key,\n    and works against every Public API endpoint. On the MCP endpoint it is sent as\n    \"Authorization: Bearer <token>\".\n  sources: [https://docs.postiz.com/public-api/oauth, well-known/postiz-oauth-authorization-server-mcp-oauth.json]\n- name: PostizCLIDeviceFlow\n  type: oauth2\n  flow: deviceCode\n  auth_server: https://cli-auth.postiz.com\n  description: >-\n    `postiz auth:login` runs an OAuth2 device flow through a hosted auth server that\n    mediates the standard authorization-code exchange, so CLI users never handle a\n    client id or secret. Credentials are stored at ~/.postiz/credentials.json.\n    Self-hosters can run their own auth server (gitroomhq/postiz-agent, server/).\n  precedence: OAuth2 credentials take priority over POSTIZ_API_KEY when both are present.\n  sources: [https://docs.postiz.com/cli/authentication]\nself_hosted:\n  note: >-\n    Self-hosted instances authenticate identically\
  \ against {NEXT_PUBLIC_BACKEND_URL}.\n    Postiz separately supports OIDC for signing in to the application itself\n    (https://docs.postiz.com/configuration/oauth) — that is end-user SSO into the app,\n    not API authentication, and is not modelled as an API scheme here.\nerrors:\n  401: Authorization header missing or the API key is unrecognised.\n  403: Key is valid but does not own the resource.\n  oauth:\n    invalid_client: client id or secret wrong at token exchange\n    invalid_grant: code invalid, expired or already used\n    unsupported_grant_type: grant_type is not authorization_code\n    access_denied: user denied the authorization request\nmaintainers:\n- FN: Kin Lane\n  email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/postiz/refs/heads/main/authentication/postiz-authentication.yml
summary_line: apiKey/oauth2 · 3 schemes
tags:
- Social Media
- Scheduling
- Open Source
- Content
- Marketing
- Agents
- MCP
- Automation
- Publishing
- Analytics
---
