---
api_key_in: []
api_specs:
- filename: silent-push-web-scanner.postman_collection.json
  format: json
  label: Silent Push API
  slug: silent-push-api
  spec_type: Postman
  url: https://raw.githubusercontent.com/api-evangelist/silent-push/refs/heads/main/postman/silent-push-web-scanner.postman_collection.json
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Silent Push Authentication
name_suffix: Authentication
oauth_flows: []
overview: Silent Push declares 5 security scheme(s) across its OpenAPI definitions.
provider_name: Silent Push
provider_slug: silent-push
scheme_count: 5
schemes:
- description: Organization-scoped API key. Every Silent Push REST endpoint requires one.
  docs: https://help.silentpush.com/docs/security-and-api-integration
  evidence: 'API reference declares "SecurityAPI Key: ApiKeyAuthHeader parameter name x-api-key"'
  header_casing_note: the Get Started guide writes the header as X-API-KEY and the API reference page as x-api-key; HTTP header names are case-insensitive so both work.
  id: ApiKeyAuth
  in: header
  issuance:
    expiry: user-set expiration date at creation time
    fields:
    - nickname
    - expiration date
    role_required: Organizational Admin
    rotation: keys can be copied, edited or deleted from the API Keys table
    self_service: true
    ui_path: user icon > Organization > API Keys > +Add New API Key
  name: x-api-key
  surface: rest
  type: apiKey
- description: A separate, organization-specific access key for the Threat Check API, found under user icon > Subscription rather than under Organization > API Keys. Threat Check calls do not consume usage credits and are unmetered for Enterprise customers.
  docs: https://help.silentpush.com/docs/security-and-api-integration
  id: ThreatCheckKey
  in: header
  name: x-api-key
  note: Threat Check also supports DNS-based lookups as an alternative to HTTP, intended for high-volume filtering. That path is not API-key authenticated in the same way; the docs do not detail its authorization model.
  surface: rest
  type: apiKey
- description: The hosted MCP server accepts a bearer token in the Authorization header.
  evidence: 'POST https://mcp.silentpush.com/mcp without credentials returns 401 with body ''Missing or invalid Authorization header. Use: Authorization: Bearer <token>'' (probed 2026-08-27)'
  id: McpBearer
  scheme: bearer
  surface: mcp
  type: http
- description: The MCP server publishes RFC 8414 OAuth 2.0 Authorization Server Metadata, so MCP clients can complete an OAuth 2.1 authorization-code flow rather than pasting a static token.
  dynamic_client_registration: true
  evidence: GET https://mcp.silentpush.com/.well-known/oauth-authorization-server -> 200 application/json (probed 2026-08-27)
  flows:
    authorization_code:
      authorization_url: https://mcp.silentpush.com/oauth/authorize
      pkce: S256
      pkce_required: true
      scopes: {}
      token_url: https://mcp.silentpush.com/oauth/token
  grant_types:
  - authorization_code
  - refresh_token
  id: McpOAuth
  metadata_document: well-known/silent-push-oauth-authorization-server.json
  registration_endpoint: https://mcp.silentpush.com/oauth/register
  response_types:
  - code
  surface: mcp
  token_endpoint_auth_methods:
  - client_secret_post
  type: oauth2
- description: The first-party CLI reads the same organization API key from an environment variable.
  docs: https://github.com/Silent-Push/SP---CLI
  id: SilentPushApiKeyEnv
  in: environment
  name: SILENT_PUSH_API_KEY
  surface: cli
  type: apiKey
slug: silent-push-authentication
source_filename: silent-push-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-27'\nmethod: searched\nsource: >-\n  https://help.silentpush.com/docs/get-started-with-api,\n  https://help.silentpush.com/docs/security-and-api-integration,\n  https://help.silentpush.com/apidocs/perform-a-live-scan, and probes of\n  https://mcp.silentpush.com/.well-known/oauth-authorization-server\nnote: >-\n  Derived-from-spec was not possible: the Silent Push OpenAPI at\n  https://api.silentpush.com/api/schema/ returns 401 (content-type\n  application/vnd.oai.openapi), so securitySchemes could not be read. This\n  profile is built from the published documentation and from live probes of the\n  MCP authorization surface instead.\n\nschemes:\n- id: ApiKeyAuth\n  surface: rest\n  type: apiKey\n  in: header\n  name: x-api-key\n  header_casing_note: >-\n    the Get Started guide writes the header as X-API-KEY and the API reference\n    page as x-api-key; HTTP header names are case-insensitive so both work.\n  description: >-\n    Organization-scoped API key.\
  \ Every Silent Push REST endpoint requires one.\n  issuance:\n    self_service: true\n    ui_path: 'user icon > Organization > API Keys > +Add New API Key'\n    role_required: Organizational Admin\n    fields: [nickname, expiration date]\n    rotation: keys can be copied, edited or deleted from the API Keys table\n    expiry: user-set expiration date at creation time\n  docs: https://help.silentpush.com/docs/security-and-api-integration\n  evidence: 'API reference declares \"SecurityAPI Key: ApiKeyAuthHeader parameter name x-api-key\"'\n\n- id: ThreatCheckKey\n  surface: rest\n  type: apiKey\n  in: header\n  name: x-api-key\n  description: >-\n    A separate, organization-specific access key for the Threat Check API, found\n    under user icon > Subscription rather than under Organization > API Keys.\n    Threat Check calls do not consume usage credits and are unmetered for\n    Enterprise customers.\n  docs: https://help.silentpush.com/docs/security-and-api-integration\n  note: >-\n \
  \   Threat Check also supports DNS-based lookups as an alternative to HTTP,\n    intended for high-volume filtering. That path is not API-key authenticated\n    in the same way; the docs do not detail its authorization model.\n\n- id: McpBearer\n  surface: mcp\n  type: http\n  scheme: bearer\n  description: >-\n    The hosted MCP server accepts a bearer token in the Authorization header.\n  evidence: >-\n    POST https://mcp.silentpush.com/mcp without credentials returns 401 with\n    body 'Missing or invalid Authorization header. Use: Authorization: Bearer\n    <token>' (probed 2026-08-27)\n\n- id: McpOAuth\n  surface: mcp\n  type: oauth2\n  description: >-\n    The MCP server publishes RFC 8414 OAuth 2.0 Authorization Server Metadata,\n    so MCP clients can complete an OAuth 2.1 authorization-code flow rather than\n    pasting a static token.\n  flows:\n    authorization_code:\n      authorization_url: https://mcp.silentpush.com/oauth/authorize\n      token_url: https://mcp.silentpush.com/oauth/token\n\
  \      pkce: S256\n      pkce_required: true\n      scopes: {}\n  registration_endpoint: https://mcp.silentpush.com/oauth/register\n  dynamic_client_registration: true\n  grant_types: [authorization_code, refresh_token]\n  token_endpoint_auth_methods: [client_secret_post]\n  response_types: [code]\n  metadata_document: well-known/silent-push-oauth-authorization-server.json\n  evidence: >-\n    GET https://mcp.silentpush.com/.well-known/oauth-authorization-server -> 200\n    application/json (probed 2026-08-27)\n\n- id: SilentPushApiKeyEnv\n  surface: cli\n  type: apiKey\n  in: environment\n  name: SILENT_PUSH_API_KEY\n  description: >-\n    The first-party CLI reads the same organization API key from an environment\n    variable.\n  docs: https://github.com/Silent-Push/SP---CLI\n\naccount_security:\n  two_factor:\n    supported: true\n    method: TOTP authenticator app\n    recovery_codes: true\n    ui_path: 'user icon > Account Settings > Set Up Two Factor Authentication'\n    docs: https://help.silentpush.com/docs/security-and-api-integration\n\
  \  sso:\n    documented: false\n\nscopes:\n  published: false\n  note: >-\n    No scope surface exists. The REST API is authorized by a single\n    organization-wide key with no per-scope subdivision, and the MCP\n    authorization server metadata declares no scopes_supported. scopes/ is\n    deliberately not emitted rather than filled with an empty artifact.\n\nx-evidence:\n- url: https://help.silentpush.com/docs/get-started-with-api\n  http_status: 200\n  fetched: '2026-08-27'\n- url: https://help.silentpush.com/docs/security-and-api-integration\n  http_status: 200\n  fetched: '2026-08-27'\n- url: https://help.silentpush.com/apidocs/perform-a-live-scan\n  http_status: 200\n  fetched: '2026-08-27'\n- url: https://mcp.silentpush.com/.well-known/oauth-authorization-server\n  http_status: 200\n  fetched: '2026-08-27'\n- url: https://api.silentpush.com/api/schema/\n  http_status: 401\n  content_type: application/vnd.oai.openapi\n  fetched: '2026-08-27'\n  finding: OpenAPI exists but is auth-gated\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/silent-push/refs/heads/main/authentication/silent-push-authentication.yml
summary_line: 5 schemes
tags:
- Company
- Security
- Threat Intelligence
- Cybersecurity
- DNS
- Domain Intelligence
- Passive DNS
- Enrichment
- Threat Feeds
- WHOIS
- Model Context Protocol
---
