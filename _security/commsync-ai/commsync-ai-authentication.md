---
anonymous_access: false
api_key_in: []
auth_types: []
description: CommSync accepts two credentials on the MCP endpoint (https://server.commsync.ai/api/mcp), both sent as a Bearer token and both reaching the same tools, scoped to one user and their org role. API keys also authenticate the REST webhook-management API. No OpenAPI is published, so this profile is read from the docs.
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: CommSync Authentication
name_suffix: Authentication
oauth_flows: []
overview: CommSync declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: CommSync
provider_slug: commsync-ai
scheme_count: 2
schemes:
- client_auth_methods:
  - none
  - client_secret_post
  - client_secret_basic
  client_registration: Dynamic client registration (RFC 7591) at https://server.commsync.ai/oauth/register, or a Client ID Metadata Document (an https URL as the client_id)
  discovery:
    authorization_server_metadata: https://server.commsync.ai/.well-known/oauth-authorization-server
    protected_resource_metadata: https://server.commsync.ai/.well-known/oauth-protected-resource/api/mcp
    www_authenticate: Bearer resource_metadata="https://server.commsync.ai/.well-known/oauth-protected-resource/api/mcp"
  docs: https://commsync.ai/docs/connect-ai-apps
  flows:
  - authorizationCode
  name: oauth2
  pkce: S256 only
  primary: true
  resource_indicator: https://server.commsync.ai/api/mcp (RFC 8707)
  revocation: https://server.commsync.ai/oauth/revoke (RFC 7009)
  scopes:
  - mcp
  standards:
  - OAuth 2.1
  - RFC 9728
  - RFC 8414
  - RFC 7591
  - RFC 8707
  - RFC 7009
  tokens:
    access_token: csat_… prefix, 1 hour
    refresh_token: csrt_… prefix, 90 days, rotated on every use; a rotated token stays valid for 30 seconds, reuse after that revokes the family
  type: oauth2
- applies_to:
  - MCP server
  - REST webhook-management API (/api/webhooks/endpoints)
  docs: https://commsync.ai/docs/api-keys
  expiry: There is no automatic key expiry or scheduled rotation.
  header: 'Authorization: Bearer csk_<your_api_key>'
  key_format: csk_ followed by 48 hex characters; shown once at creation, stored only as a SHA-256 hash
  name: apiKey
  revocation: Settings → API Keys → Revoke key; in-flight requests start to receive 401 Unauthorized
  scheme: bearer
  scoping: inherits the creating user's org role (OWNER, ADMIN, MEMBER) and channel access; optionally restricted to specific lines (email addresses / phone numbers) and to Redacted security details
  type: http
slug: commsync-ai-authentication
source_filename: commsync-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://commsync.ai/auth.md\ndocs: https://commsync.ai/docs/api-keys\ndescription: CommSync accepts two credentials on the MCP endpoint (https://server.commsync.ai/api/mcp), both sent as a Bearer token and both reaching the same tools, scoped to one user and their org role. API keys also authenticate the REST webhook-management API. No OpenAPI is published, so this profile is read from the docs.\nschemes:\n- name: oauth2\n  type: oauth2\n  primary: true\n  flows:\n  - authorizationCode\n  pkce: S256 only\n  scopes:\n  - mcp\n  discovery:\n    protected_resource_metadata: https://server.commsync.ai/.well-known/oauth-protected-resource/api/mcp\n    authorization_server_metadata: https://server.commsync.ai/.well-known/oauth-authorization-server\n    www_authenticate: 'Bearer resource_metadata=\"https://server.commsync.ai/.well-known/oauth-protected-resource/api/mcp\"'\n  client_registration: Dynamic client registration (RFC 7591)\
  \ at https://server.commsync.ai/oauth/register, or a Client ID Metadata Document (an https URL as the client_id)\n  client_auth_methods: [none, client_secret_post, client_secret_basic]\n  resource_indicator: https://server.commsync.ai/api/mcp (RFC 8707)\n  tokens:\n    access_token: \"csat_… prefix, 1 hour\"\n    refresh_token: \"csrt_… prefix, 90 days, rotated on every use; a rotated token stays valid for 30 seconds, reuse after that revokes the family\"\n  revocation: https://server.commsync.ai/oauth/revoke (RFC 7009)\n  standards: [OAuth 2.1, RFC 9728, RFC 8414, RFC 7591, RFC 8707, RFC 7009]\n  docs: https://commsync.ai/docs/connect-ai-apps\n- name: apiKey\n  type: http\n  scheme: bearer\n  header: 'Authorization: Bearer csk_<your_api_key>'\n  key_format: csk_ followed by 48 hex characters; shown once at creation, stored only as a SHA-256 hash\n  expiry: There is no automatic key expiry or scheduled rotation.\n  revocation: Settings → API Keys → Revoke key; in-flight requests start\
  \ to receive 401 Unauthorized\n  scoping: inherits the creating user's org role (OWNER, ADMIN, MEMBER) and channel access; optionally restricted to specific lines (email addresses / phone numbers) and to Redacted security details\n  applies_to: [MCP server, REST webhook-management API (/api/webhooks/endpoints)]\n  docs: https://commsync.ai/docs/api-keys\nwebhook_signing:\n  scheme: HMAC-SHA256\n  header: 'X-CommSync-Signature: t=<unix-seconds>,v1=<hex>'\n  docs: https://commsync.ai/docs/webhooks\n"
source_yaml_url: https://artifacts.apis.io/commsync-ai/authentication/commsync-ai-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Unified Inbox
- SMS
- Email
- Messaging
- Artificial Intelligence
- AI Agents
- MCP
- Webhook
- Communications
---
