---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: entergram-accounts-api-openapi.yml
  format: yaml
  label: Entergram Accounts API
  slug: entergram-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/entergram/refs/heads/main/openapi/entergram-accounts-api-openapi.yml
- filename: entergram-chat-commands-api-openapi.yml
  format: yaml
  label: Entergram Chat Commands API
  slug: entergram-chat-commands-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/entergram/refs/heads/main/openapi/entergram-chat-commands-api-openapi.yml
- filename: entergram-chats-api-openapi.yml
  format: yaml
  label: Entergram Chats API
  slug: entergram-chats-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/entergram/refs/heads/main/openapi/entergram-chats-api-openapi.yml
- filename: entergram-contacts-api-openapi.yml
  format: yaml
  label: Entergram Contacts API
  slug: entergram-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/entergram/refs/heads/main/openapi/entergram-contacts-api-openapi.yml
- filename: entergram-custom-fields-api-openapi.yml
  format: yaml
  label: Entergram Custom Fields API
  slug: entergram-custom-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/entergram/refs/heads/main/openapi/entergram-custom-fields-api-openapi.yml
- filename: entergram-events-api-openapi.yml
  format: yaml
  label: Entergram Events API
  slug: entergram-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/entergram/refs/heads/main/openapi/entergram-events-api-openapi.yml
- filename: entergram-groups-api-openapi.yml
  format: yaml
  label: Entergram Groups API
  slug: entergram-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/entergram/refs/heads/main/openapi/entergram-groups-api-openapi.yml
- filename: entergram-live-chats-api-openapi.yml
  format: yaml
  label: Entergram Live Chats API
  slug: entergram-live-chats-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/entergram/refs/heads/main/openapi/entergram-live-chats-api-openapi.yml
- filename: entergram-make-webhooks-api-openapi.yml
  format: yaml
  label: Entergram Make webhooks API
  slug: entergram-make-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/entergram/refs/heads/main/openapi/entergram-make-webhooks-api-openapi.yml
- filename: entergram-members-api-openapi.yml
  format: yaml
  label: Entergram Members API
  slug: entergram-members-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/entergram/refs/heads/main/openapi/entergram-members-api-openapi.yml
- filename: entergram-messages-api-openapi.yml
  format: yaml
  label: Entergram Messages API
  slug: entergram-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/entergram/refs/heads/main/openapi/entergram-messages-api-openapi.yml
- filename: entergram-system-api-openapi.yml
  format: yaml
  label: Entergram System API
  slug: entergram-system-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/entergram/refs/heads/main/openapi/entergram-system-api-openapi.yml
- filename: entergram-tickets-api-openapi.yml
  format: yaml
  label: Entergram Tickets API
  slug: entergram-tickets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/entergram/refs/heads/main/openapi/entergram-tickets-api-openapi.yml
- filename: entergram-webhooks-api-openapi.yml
  format: yaml
  label: Entergram Webhooks API
  slug: entergram-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/entergram/refs/heads/main/openapi/entergram-webhooks-api-openapi.yml
- filename: entergram-workspace-api-openapi.yml
  format: yaml
  label: Entergram Workspace API
  slug: entergram-workspace-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/entergram/refs/heads/main/openapi/entergram-workspace-api-openapi.yml
- filename: entergram-workspace-chats-api-openapi.yml
  format: yaml
  label: Entergram Workspace Chats API
  slug: entergram-workspace-chats-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/entergram/refs/heads/main/openapi/entergram-workspace-chats-api-openapi.yml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Entergram Authentication
name_suffix: Authentication
oauth_flows: []
overview: Entergram secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Entergram
provider_slug: entergram
scheme_count: 2
schemes:
- description: Workspace-scoped PRO API key created in Entergram Settings > Developers.
  in: header
  name: ApiKeyAuth
  parameter: X-API-Key
  sources:
  - openapi/entergram-openapi.json
  type: apiKey
- applies_to: MCP server (mcp.entergram.com/mcp)
  authorization_endpoint: https://app.entergram.com/oauth/authorize
  authorization_server: https://app.entergram.com
  description: OAuth2 with PKCE and dynamic client registration for the Entergram MCP server. Bearer token in the Authorization header. Scopes documented in scopes/entergram-scopes.yml.
  flow: authorization_code
  jwks_uri: https://app.entergram.com/oauth/jwks.json
  name: McpOAuth
  pkce: true
  registration_endpoint: https://app.entergram.com/oauth/register
  sources:
  - well-known/entergram-oauth-authorization-server.json
  - well-known/entergram-oauth-protected-resource.json
  token_endpoint: https://app.entergram.com/oauth/token
  type: oauth2
slug: entergram-authentication
source_filename: entergram-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-11'\nmethod: derived\nsource: openapi/entergram-openapi.json\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - header\n  note: >-\n    The REST API (api.entergram.com) authenticates with a workspace-scoped X-API-Key header. The\n    hosted MCP server (mcp.entergram.com) authenticates with OAuth2 authorization_code + PKCE against\n    app.entergram.com, with dynamic client registration. The OAuth profile was captured by probing\n    the RFC 8414 / RFC 9728 discovery documents, not from the REST OpenAPI (which declares apiKey only).\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: Workspace-scoped PRO API key created in Entergram Settings > Developers.\n  sources:\n  - openapi/entergram-openapi.json\n- name: McpOAuth\n  type: oauth2\n  flow: authorization_code\n  pkce: true\n  authorization_server: https://app.entergram.com\n  authorization_endpoint: https://app.entergram.com/oauth/authorize\n\
  \  token_endpoint: https://app.entergram.com/oauth/token\n  registration_endpoint: https://app.entergram.com/oauth/register\n  jwks_uri: https://app.entergram.com/oauth/jwks.json\n  applies_to: MCP server (mcp.entergram.com/mcp)\n  description: >-\n    OAuth2 with PKCE and dynamic client registration for the Entergram MCP server. Bearer token in the\n    Authorization header. Scopes documented in scopes/entergram-scopes.yml.\n  sources:\n  - well-known/entergram-oauth-authorization-server.json\n  - well-known/entergram-oauth-protected-resource.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/entergram/refs/heads/main/authentication/entergram-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- Messaging
- Notification
- Communications
- CRM
- Telegram
- Customer-Support
- Ticketing
- Sales
- MCP
- Webhook
---
