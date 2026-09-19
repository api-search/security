---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: clickup-authorization-api-openapi.yml
  format: yaml
  label: clickup Authorization API
  slug: clickup-authorization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clickup/refs/heads/main/openapi/clickup-authorization-api-openapi.yml
- filename: clickup-comments-api-openapi.yml
  format: yaml
  label: clickup Comments API
  slug: clickup-comments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clickup/refs/heads/main/openapi/clickup-comments-api-openapi.yml
- filename: clickup-custom-fields-api-openapi.yml
  format: yaml
  label: clickup Custom Fields API
  slug: clickup-custom-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clickup/refs/heads/main/openapi/clickup-custom-fields-api-openapi.yml
- filename: clickup-folders-api-openapi.yml
  format: yaml
  label: clickup Folders API
  slug: clickup-folders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clickup/refs/heads/main/openapi/clickup-folders-api-openapi.yml
- filename: clickup-goals-api-openapi.yml
  format: yaml
  label: clickup Goals API
  slug: clickup-goals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clickup/refs/heads/main/openapi/clickup-goals-api-openapi.yml
- filename: clickup-lists-api-openapi.yml
  format: yaml
  label: clickup Lists API
  slug: clickup-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clickup/refs/heads/main/openapi/clickup-lists-api-openapi.yml
- filename: clickup-spaces-api-openapi.yml
  format: yaml
  label: clickup Spaces API
  slug: clickup-spaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clickup/refs/heads/main/openapi/clickup-spaces-api-openapi.yml
- filename: clickup-tasks-api-openapi.yml
  format: yaml
  label: clickup Tasks API
  slug: clickup-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clickup/refs/heads/main/openapi/clickup-tasks-api-openapi.yml
- filename: clickup-teams-api-openapi.yml
  format: yaml
  label: clickup Teams API
  slug: clickup-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clickup/refs/heads/main/openapi/clickup-teams-api-openapi.yml
- filename: clickup-time-tracking-api-openapi.yml
  format: yaml
  label: clickup Time Tracking API
  slug: clickup-time-tracking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clickup/refs/heads/main/openapi/clickup-time-tracking-api-openapi.yml
- filename: clickup-views-api-openapi.yml
  format: yaml
  label: clickup Views API
  slug: clickup-views-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clickup/refs/heads/main/openapi/clickup-views-api-openapi.yml
- filename: clickup-webhooks-api-openapi.yml
  format: yaml
  label: clickup Webhooks API
  slug: clickup-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clickup/refs/heads/main/openapi/clickup-webhooks-api-openapi.yml
- filename: clickup-oauth-api-openapi.yml
  format: yaml
  label: Clickup O Auth API
  slug: clickup-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clickup/refs/heads/main/openapi/clickup-oauth-api-openapi.yml
- filename: clickup-api-v2-reference-openapi.json
  format: json
  label: ClickUp API v2
  slug: clickup-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clickup/refs/heads/main/openapi/clickup-api-v2-reference-openapi.json
- filename: clickup-public-api-v3-openapi.json
  format: json
  label: ClickUp Public API v3
  slug: clickup-api-v3
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clickup/refs/heads/main/openapi/clickup-public-api-v3-openapi.json
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 4
method: searched
name: Clickup Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Clickup secures its APIs with apiKey and oauth2 across 4 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Clickup
provider_slug: clickup
scheme_count: 4
schemes:
- description: Personal API token (prefix `pk_`, generated in Settings > Apps, never expires) or an OAuth 2.0 access token sent as a Bearer value.
  in: header
  name: Authorization_Token
  parameter: Authorization
  sources:
  - openapi/clickup-api-v2-reference-openapi.json
  type: apiKey
- in: header
  name: authHeader
  parameter: Authorization
  sources:
  - openapi/clickup-public-api-v3-openapi.json
  type: apiKey
- authorization_unit: workspace
  authorization_url: https://app.clickup.com/api
  docs: https://developer.clickup.com/docs/authentication
  expires: false
  flow: authorizationCode
  name: ClickUp OAuth 2.0
  note: Users authorize specific Workspaces rather than scopes. Access tokens do not expire (developer FAQ). Client credentials are issued when an app is created by a Workspace owner or admin.
  scopes: []
  token_operation: GetAccessToken
  token_url: https://api.clickup.com/api/v2/oauth/token
  type: oauth2
- authorization_url: https://mcp.clickup.com/oauth/authorize
  flow: authorizationCode
  name: ClickUp MCP OAuth 2.0
  note: Separate authorization server from the public API; dynamic client registration is open (token_endpoint_auth_methods_supported ["none"]).
  pkce: S256
  registration_url: https://mcp.clickup.com/oauth/register
  resource: https://mcp.clickup.com
  scopes:
  - read
  - write
  sources:
  - well-known/clickup-mcp-oauth-authorization-server.json
  - well-known/clickup-mcp-oauth-protected-resource.json
  token_url: https://mcp.clickup.com/oauth/token
  type: oauth2
slug: clickup-authentication
source_filename: clickup-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-17'\nmethod: searched\ndocs: https://developer.clickup.com/docs/authentication\nsource: >-\n  https://developer.clickup.com/docs/authentication (docs) upgraded over the derived read of\n  openapi/clickup-api-v2-reference-openapi.json and openapi/clickup-public-api-v3-openapi.json\nsummary:\n  types: [apiKey, oauth2]\n  api_key_in: [header]\n  api_key_names: [Authorization]\n  oauth2_flows: [authorizationCode]\n  token_expiry: none\n  note: >-\n    ClickUp carries BOTH credentials in the same `Authorization` header, which is why both specs declare\n    only an apiKey scheme: a personal token is sent bare (`Authorization: pk_...`) and an OAuth access\n    token is sent as `Authorization: Bearer {access_token}`. The OAuth flow is documented in prose and by\n    the GetAccessToken operation, not by an oauth2 securityScheme.\nschemes:\n- name: Authorization_Token\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: >-\n    Personal API token\
  \ (prefix `pk_`, generated in Settings > Apps, never expires) or an OAuth 2.0 access\n    token sent as a Bearer value.\n  sources: [openapi/clickup-api-v2-reference-openapi.json]\n- name: authHeader\n  type: apiKey\n  in: header\n  parameter: Authorization\n  sources: [openapi/clickup-public-api-v3-openapi.json]\n- name: ClickUp OAuth 2.0\n  type: oauth2\n  flow: authorizationCode\n  authorization_url: https://app.clickup.com/api\n  token_url: https://api.clickup.com/api/v2/oauth/token\n  token_operation: GetAccessToken\n  scopes: []\n  authorization_unit: workspace\n  expires: false\n  docs: https://developer.clickup.com/docs/authentication\n  note: >-\n    Users authorize specific Workspaces rather than scopes. Access tokens do not expire (developer FAQ).\n    Client credentials are issued when an app is created by a Workspace owner or admin.\n- name: ClickUp MCP OAuth 2.0\n  type: oauth2\n  flow: authorizationCode\n  authorization_url: https://mcp.clickup.com/oauth/authorize\n  token_url:\
  \ https://mcp.clickup.com/oauth/token\n  registration_url: https://mcp.clickup.com/oauth/register\n  pkce: S256\n  scopes: [read, write]\n  resource: https://mcp.clickup.com\n  sources: [well-known/clickup-mcp-oauth-authorization-server.json, well-known/clickup-mcp-oauth-protected-resource.json]\n  note: Separate authorization server from the public API; dynamic client registration is open (token_endpoint_auth_methods_supported [\"none\"]).\nwebhook_authentication:\n  mechanism: HMAC-SHA256\n  header: X-Signature\n  secret: per-webhook shared secret returned when the webhook is created\n  docs: https://developer.clickup.com/docs/webhooksignature\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/clickup/refs/heads/main/authentication/clickup-authentication.yml
summary_line: apiKey/oauth2 · 4 schemes
tags:
- Project Management
- Work Management
- Productivity
- Collaboration
- Task
- Documents
- Chat
- Time Tracking
- MCP
---
