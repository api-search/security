---
api_key_in:
- cookie
- header
api_specs:
- filename: fullcast-assistant-openapi-original.json
  format: json
  label: Fullcast Assistant API
  slug: fullcast-assistant-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fullcast/refs/heads/main/openapi/fullcast-assistant-openapi-original.json
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Fullcast Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Fullcast secures its APIs with apiKey and oauth2 across 5 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Fullcast
provider_slug: fullcast
scheme_count: 5
schemes:
- host: https://assistant.fullcast.io
  in: cookie
  name: APIKeyCookie
  note: browser session cookie, not a developer credential
  parameter: token
  sources:
  - openapi/fullcast-assistant-openapi-original.json
  surface: Fullcast Assistant API
  type: apiKey
- host: https://assistant.fullcast.io
  in: header
  name: APIKeyHeader
  note: CSRF companion to the cookie above
  parameter: csrf_token
  sources:
  - openapi/fullcast-assistant-openapi-original.json
  surface: Fullcast Assistant API
  type: apiKey
- bearer_in: header
  flows:
  - authorizationUrl: https://app.fullcast.io/mcp/authorize
    flow: authorizationCode
    issuer: https://app.fullcast.io/mcp
    pkce:
    - S256
    registrationUrl: https://app.fullcast.io/mcp/register
    scopes: []
    tokenUrl: https://app.fullcast.io/mcp/token
    token_endpoint_auth_methods:
    - client_secret_post
    - none
  host: https://app.fullcast.io/mcp
  name: Fullcast MCP OAuth 2.1
  sources:
  - well-known/fullcast-app-mcp-oauth-authorization-server.json
  surface: Fullcast MCP
  type: oauth2
  verified: 401 MISSING_BEARER with WWW-Authenticate Bearer realm="mcp-openapi" observed 2026-08-13
- bearer_in: header
  flows:
  - authorizationUrl: https://assistant.fullcast.io/oauth/authorize
    flow: authorizationCode
    issuer: https://assistant.fullcast.io
    pkce:
    - plain
    - S256
    registrationUrl: https://assistant.fullcast.io/oauth/register
    scopes:
    - openid
    - email
    - profile
    - offline_access
    - mcp:resources
    - mcp:tools
    - mcp:prompts
    tokenUrl: https://assistant.fullcast.io/oauth/token
    token_endpoint_auth_methods:
    - client_secret_post
    - none
    userinfoUrl: https://assistant.fullcast.io/oauth/userinfo
  host: https://assistant.fullcast.io
  name: Fullcast Assistant OAuth 2.1
  refresh_tokens: true
  sources:
  - well-known/fullcast-assistant-oauth-authorization-server.json
  surface: Fullcast Assistant MCP Server
  token_response_fields:
  - access_token
  - jwe_access_token
  - token_type
  - expires_in
  - refresh_token
  - scope
  type: oauth2
- host: https://api.copy.ai/api
  in: header
  lifecycle:
    created_in: Configuration > API Keys > Create API Key
    default_expiry: never
    managed_by:
    - Workspace Owner
    - Admin
    operations:
    - disable
    - enable
    - rename
    - delete
    permission_model: key inherits all access permissions of the user it is assigned to
    recommended_expiry: 12 months
    scoping_advice: assign the key to a restricted user or Teamspace to limit its blast radius
    shown_once: true
  name: Copy.ai workspace API key
  parameter: x-copy-ai-api-key
  sources:
  - https://support.fullcast.com/copy-ai/docs/api-key-management.md
  surface: Fullcast Copy.ai Workflows API
  type: apiKey
slug: fullcast-authentication
source_filename: fullcast-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: openapi/fullcast-assistant-openapi-original.json\ndocs:\n- https://support.fullcast.com/docs/set-up-the-model-context-protocol-mcp.md\n- https://support.fullcast.com/copy-ai/docs/api-key-management.md\n- https://assistant.fullcast.io/.well-known/oauth-authorization-server\n- https://app.fullcast.io/mcp/.well-known/oauth-authorization-server\nnote: >-\n  Upgraded from the mechanical derive, which saw only the two apiKey schemes declared in the\n  Assistant OpenAPI. Fullcast actually runs THREE distinct authentication models across three\n  surfaces, and the OpenAPI declares the weakest one: the same host that serves that spec also\n  runs a full OAuth 2.1 authorization server whose /oauth/* operations are IN the document but\n  are not wired into components.securitySchemes. All OAuth detail below was read from live\n  RFC 8414 / RFC 9728 metadata, not inferred.\nsummary:\n  types: [apiKey, oauth2]\n  api_key_in: [cookie, header]\n\
  \  oauth2_flows: [authorizationCode]\n  pkce: [S256, plain]\n  dynamic_client_registration: true\n  surfaces: 3\nschemes:\n- name: APIKeyCookie\n  type: apiKey\n  in: cookie\n  parameter: token\n  surface: Fullcast Assistant API\n  host: https://assistant.fullcast.io\n  sources: [openapi/fullcast-assistant-openapi-original.json]\n  note: browser session cookie, not a developer credential\n- name: APIKeyHeader\n  type: apiKey\n  in: header\n  parameter: csrf_token\n  surface: Fullcast Assistant API\n  host: https://assistant.fullcast.io\n  sources: [openapi/fullcast-assistant-openapi-original.json]\n  note: CSRF companion to the cookie above\n- name: Fullcast MCP OAuth 2.1\n  type: oauth2\n  surface: Fullcast MCP\n  host: https://app.fullcast.io/mcp\n  bearer_in: header\n  flows:\n  - flow: authorizationCode\n    issuer: https://app.fullcast.io/mcp\n    authorizationUrl: https://app.fullcast.io/mcp/authorize\n    tokenUrl: https://app.fullcast.io/mcp/token\n    registrationUrl: https://app.fullcast.io/mcp/register\n\
  \    pkce: [S256]\n    token_endpoint_auth_methods: [client_secret_post, none]\n    scopes: []\n  sources: [well-known/fullcast-app-mcp-oauth-authorization-server.json]\n  verified: >-\n    401 MISSING_BEARER with WWW-Authenticate Bearer realm=\"mcp-openapi\" observed 2026-08-13\n- name: Fullcast Assistant OAuth 2.1\n  type: oauth2\n  surface: Fullcast Assistant MCP Server\n  host: https://assistant.fullcast.io\n  bearer_in: header\n  flows:\n  - flow: authorizationCode\n    issuer: https://assistant.fullcast.io\n    authorizationUrl: https://assistant.fullcast.io/oauth/authorize\n    tokenUrl: https://assistant.fullcast.io/oauth/token\n    registrationUrl: https://assistant.fullcast.io/oauth/register\n    userinfoUrl: https://assistant.fullcast.io/oauth/userinfo\n    pkce: [plain, S256]\n    token_endpoint_auth_methods: [client_secret_post, none]\n    scopes: [openid, email, profile, offline_access, 'mcp:resources', 'mcp:tools', 'mcp:prompts']\n  sources: [well-known/fullcast-assistant-oauth-authorization-server.json]\n\
  \  refresh_tokens: true\n  token_response_fields: [access_token, jwe_access_token, token_type, expires_in, refresh_token, scope]\n- name: Copy.ai workspace API key\n  type: apiKey\n  in: header\n  parameter: x-copy-ai-api-key\n  surface: Fullcast Copy.ai Workflows API\n  host: https://api.copy.ai/api\n  sources: [https://support.fullcast.com/copy-ai/docs/api-key-management.md]\n  lifecycle:\n    created_in: Configuration > API Keys > Create API Key\n    shown_once: true\n    default_expiry: never\n    recommended_expiry: 12 months\n    permission_model: key inherits all access permissions of the user it is assigned to\n    scoping_advice: assign the key to a restricted user or Teamspace to limit its blast radius\n    operations: [disable, enable, rename, delete]\n    managed_by: [Workspace Owner, Admin]\ntenant_gate:\n  note: >-\n    MCP access is off by default. A tenant admin must enable it at\n    Settings > Application Settings > AI & Agents > Enable AI Assistant Features before any\n\
  \    token will work.\n  docs: https://support.fullcast.com/docs/enable-ai-features.md\nplatform_controls:\n- multi-factor authentication\n- role-based access control with granular permissions\n- IP and country login restrictions (https://support.fullcast.com/docs/configure-ip-and-country-restrictions.md)\ngaps:\n- >-\n  The OpenAPI does not declare the OAuth 2.1 scheme its own /oauth/* operations implement, so\n  a generated client sees only cookie + CSRF auth. Captured as a correction in\n  overlays/fullcast-assistant-overlay.yaml.\n- The assistant issuer still advertises PKCE method \"plain\" alongside S256.\n- 'mcp:tools is a single scope covering both read and write tools; there is no read-only scope.'\n- No published developer API key exists for the Fullcast platform itself - only for the acquired Copy.ai product.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fullcast/refs/heads/main/authentication/fullcast-authentication.yml
summary_line: apiKey/oauth2 · 5 schemes
tags:
- Company
- Enterprise
- Revenue Operations
- Sales Planning
- Territory Management
- Go-To-Market
- Incentive Compensation
- Forecasting
- Lead Routing
- MCP
- AI Agents
- Sales Compensation
---
