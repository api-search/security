---
api_key_in:
- header
api_specs:
- filename: ontraport-metadata-api-openapi.yml
  format: yaml
  label: Ontraport Metadata API
  slug: ontraport-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ontraport/refs/heads/main/openapi/ontraport-metadata-api-openapi.yml
- filename: ontraport-objects-api-openapi.yml
  format: yaml
  label: Ontraport Objects API
  slug: ontraport-objects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ontraport/refs/heads/main/openapi/ontraport-objects-api-openapi.yml
auth_types:
- apiKey
- oauth2
description: Ontraport runs two different authentication models on two different surfaces. The REST API uses a pair of static, unscoped, non-expiring account headers — Api-Key AND Api-Appid, both required, both sent on every request. The MCP server runs a modern OAuth 2.1 flow (authorization code + PKCE S256, refresh tokens, dynamic client registration, one scope) and accepts the REST header pair as a fallback for clients that cannot do OAuth. The REST surface has no OAuth, no scopes, no token expiry and no documented rotation procedure; what bounds a key is the Ontraport package-level and user-level permissions of the user who owns it, which have applied to API requests since 2019-02-01.
kind: authentication
layout: security
method: searched
name: Ontraport Authentication
name_suffix: Authentication
oauth_flows: []
overview: Ontraport secures its APIs with apiKey and oauth2 across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Ontraport
provider_slug: ontraport
scheme_count: 4
schemes:
- description: The account's unique API key. Must be used in conjunction with the App ID or the request will not authenticate.
  in: header
  name: ApiKeyAuth
  parameter: Api-Key
  required: true
  sources:
  - openapi/ontraport-objects-api-openapi.yml
  - openapi/ontraport-metadata-api-openapi.yml
  - https://api.ontraport.com/doc/#authentication
  surface: rest
  type: apiKey
- description: The account's unique site/App ID.
  in: header
  name: AppIdAuth
  parameter: Api-Appid
  required: true
  sources:
  - openapi/ontraport-objects-api-openapi.yml
  - openapi/ontraport-metadata-api-openapi.yml
  - https://api.ontraport.com/doc/#authentication
  surface: rest
  type: apiKey
- authorization_url: https://app.ontraport.com/oauth/authorize
  description: The standard connection flow for MCP clients that support OAuth (Claude Desktop, Claude Code, ChatGPT). Dynamic client registration is supported, as is the client-id metadata document.
  flow: authorizationCode
  grant_types:
  - authorization_code
  - refresh_token
  name: McpOAuth
  pkce: S256
  registration_url: https://app.ontraport.com/oauth/register
  resource: https://mcp.ontraport.com
  revocation_url: https://app.ontraport.com/oauth/revoke
  scopes:
  - mcp:tools
  see: scopes/ontraport-scopes.yml
  sources:
  - well-known/ontraport-oauth-protected-resource.json
  - well-known/ontraport-oauth-authorization-server.json
  surface: mcp
  token_endpoint_auth_methods:
  - client_secret_post
  - none
  token_url: https://app.ontraport.com/oauth/token
  type: oauth2
- alternate_form: 'Authorization: Bearer <app-id>:<api-key>'
  description: 'For orchestration platforms and agent frameworks where the OAuth flow is not practical. The App ID and API Key are NOT used as an OAuth client id/secret — they are passed directly as headers. Ontraport states keys are never surfaced after setup: not in MCP connection summaries, tool responses, URLs, user-facing error messages, or standard logs.'
  in: header
  name: McpApiKeyFallback
  parameter: Api-Appid + Api-Key
  sources:
  - https://ontraport.com/support/My-account/mcp-server
  surface: mcp
  type: apiKey
slug: ontraport-authentication
source_filename: ontraport-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: >-\n  https://api.ontraport.com/doc/#authentication (REST),\n  https://ontraport.com/support/My-account/mcp-server plus the RFC 9728/8414 metadata at\n  https://mcp.ontraport.com/.well-known/oauth-protected-resource and\n  https://app.ontraport.com/.well-known/oauth-authorization-server (MCP), cross-checked\n  against openapi/ontraport-objects-api-openapi.yml\ndocs: https://api.ontraport.com/doc/#authentication\ndescription: >-\n  Ontraport runs two different authentication models on two different surfaces. The REST API\n  uses a pair of static, unscoped, non-expiring account headers — Api-Key AND Api-Appid,\n  both required, both sent on every request. The MCP server runs a modern OAuth 2.1 flow\n  (authorization code + PKCE S256, refresh tokens, dynamic client registration, one scope)\n  and accepts the REST header pair as a fallback for clients that cannot do OAuth. The REST\n  surface has no OAuth, no scopes, no token expiry\
  \ and no documented rotation procedure;\n  what bounds a key is the Ontraport package-level and user-level permissions of the user\n  who owns it, which have applied to API requests since 2019-02-01.\n\nsummary:\n  surfaces: 2\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - header\n  oauth_scopes: 1\n  token_expiry: none on REST; refresh-token rotation on MCP\n  mtls: false\n  jwt: false\n\nschemes:\n- name: ApiKeyAuth\n  surface: rest\n  type: apiKey\n  in: header\n  parameter: Api-Key\n  required: true\n  description: >-\n    The account's unique API key. Must be used in conjunction with the App ID or the request\n    will not authenticate.\n  sources:\n  - openapi/ontraport-objects-api-openapi.yml\n  - openapi/ontraport-metadata-api-openapi.yml\n  - https://api.ontraport.com/doc/#authentication\n- name: AppIdAuth\n  surface: rest\n  type: apiKey\n  in: header\n  parameter: Api-Appid\n  required: true\n  description: The account's unique site/App ID.\n  sources:\n  - openapi/ontraport-objects-api-openapi.yml\n\
  \  - openapi/ontraport-metadata-api-openapi.yml\n  - https://api.ontraport.com/doc/#authentication\n- name: McpOAuth\n  surface: mcp\n  type: oauth2\n  flow: authorizationCode\n  pkce: S256\n  authorization_url: https://app.ontraport.com/oauth/authorize\n  token_url: https://app.ontraport.com/oauth/token\n  registration_url: https://app.ontraport.com/oauth/register\n  revocation_url: https://app.ontraport.com/oauth/revoke\n  grant_types:\n  - authorization_code\n  - refresh_token\n  token_endpoint_auth_methods:\n  - client_secret_post\n  - none\n  scopes:\n  - mcp:tools\n  resource: https://mcp.ontraport.com\n  description: >-\n    The standard connection flow for MCP clients that support OAuth (Claude Desktop, Claude\n    Code, ChatGPT). Dynamic client registration is supported, as is the client-id metadata\n    document.\n  sources:\n  - well-known/ontraport-oauth-protected-resource.json\n  - well-known/ontraport-oauth-authorization-server.json\n  see: scopes/ontraport-scopes.yml\n-\
  \ name: McpApiKeyFallback\n  surface: mcp\n  type: apiKey\n  in: header\n  parameter: Api-Appid + Api-Key\n  alternate_form: 'Authorization: Bearer <app-id>:<api-key>'\n  description: >-\n    For orchestration platforms and agent frameworks where the OAuth flow is not practical.\n    The App ID and API Key are NOT used as an OAuth client id/secret — they are passed\n    directly as headers. Ontraport states keys are never surfaced after setup: not in MCP\n    connection summaries, tool responses, URLs, user-facing error messages, or standard logs.\n  sources:\n  - https://ontraport.com/support/My-account/mcp-server\n\nauthorization_model:\n  rest:\n    scopes: false\n    bounded_by:\n    - Ontraport package-level permissions\n    - the permissions of the user who owns the credentials\n    - the per-object Access column in the Accessible Objects table (many types are GET-only)\n    effective_since: '2019-02-01'\n    source: 'https://api.ontraport.com/doc/#api-change-log (notice dated 2018-12-18)'\n\
  \  mcp:\n    scopes:\n    - mcp:tools\n    bounded_by:\n    - the single mcp:tools scope\n    - a per-connection tool allow/deny panel exposed after connecting\n    - a server-side guard that ignores requests to delete every record in a collection\n    - disabled generic writes on Invoices, Payments and Orders\n\nfailure_modes:\n- surface: rest\n  status: 401\n  body: Your App ID and API Key do not authenticate.\n  note: >-\n    Observed live on an unauthenticated GET https://api.ontraport.com/1/... during this pass.\n- surface: mcp\n  status: 401\n  body: '{\"error\":\"unauthorized\",\"error_description\":\"Bearer token required\"}'\n  www_authenticate: >-\n    Bearer resource_metadata=\"https://mcp.ontraport.com/.well-known/oauth-protected-resource\",\n    scope=\"mcp:tools\"\n  note: >-\n    Observed live on an unauthenticated tools/list POST to https://mcp.ontraport.com during\n    this pass. A correct RFC 9728 challenge.\n\ngaps:\n- REST keys do not expire and there is no documented\
  \ rotation or revocation procedure.\n- REST keys are unscoped — an integration that only needs to read contacts holds the same key that can charge a card.\n- No mutual TLS, no signed requests, no IP allowlist documented for the REST API.\n- No key-prefix convention that would let a leaked credential be recognised in logs or scanning.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ontraport/refs/heads/main/authentication/ontraport-authentication.yml
summary_line: apiKey/oauth2 · 4 schemes
tags:
- CRM
- Marketing Automation
- Email Marketing
- Ecommerce
- Landing Pages
- Membership Sites
- MCP
- AI Agents
- Payments
- Sales Automation
---
