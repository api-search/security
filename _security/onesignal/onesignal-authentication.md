---
api_key_in: []
api_specs:
- filename: onesignal-api-openapi.json
  format: json
  label: OneSignal REST API
  slug: onesignal-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/onesignal/refs/heads/main/openapi/_original/onesignal-api-openapi.json
- filename: onesignal-apps-api-openapi.yml
  format: yaml
  label: OneSignal Apps API
  slug: onesignal-apps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/onesignal/refs/heads/main/openapi/onesignal-apps-api-openapi.yml
- filename: onesignal-notifications-api-openapi.yml
  format: yaml
  label: OneSignal Notifications API
  slug: onesignal-notifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/onesignal/refs/heads/main/openapi/onesignal-notifications-api-openapi.yml
- filename: onesignal-players-api-openapi.yml
  format: yaml
  label: OneSignal Players API
  slug: onesignal-players-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/onesignal/refs/heads/main/openapi/onesignal-players-api-openapi.yml
- filename: onesignal-templates-api-openapi.yml
  format: yaml
  label: OneSignal Templates API
  slug: onesignal-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/onesignal/refs/heads/main/openapi/onesignal-templates-api-openapi.yml
auth_types:
- http
- oauth2
description: OneSignal authenticates the REST API with bearer API keys in two tiers, and authenticates agent/MCP clients with a separate OAuth 2.1 authorization server. The OAuth server is real and probed — RFC 8414 metadata at api.onesignal.com, PKCE S256 required, RFC 7591 dynamic client registration open — but it is not referenced anywhere in the published OpenAPI, so a spec reader sees only the bearer schemes.
kind: authentication
layout: security
method: searched
name: Onesignal Authentication
name_suffix: Authentication
oauth_flows: []
overview: OneSignal secures its APIs with http and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: OneSignal
provider_slug: onesignal
scheme_count: 3
schemes:
- description: 'App API key. Scoped to one app: sending messages, creating and updating users and subscriptions, reading message history and stats. Values are prefixed os_v2_app_ and are shown exactly once, at creation or rotation. Up to 16 per app.'
  format: 'Authorization: Key <APP_API_KEY>'
  header: Authorization
  in: header
  managed_by_api: true
  management_operations:
  - create-api-key
  - view-api-keys
  - update-api-key
  - rotate-api-key
  - delete-api-key
  name: rest_api_key
  scheme: bearer
  sources:
  - https://documentation.onesignal.com/docs/en/keys-and-ids
  - openapi/onesignal-apps-api-openapi.yml
  tier: app
  type: http
- description: Organization API key. Spans every app in the organization; required for creating apps and managing other API keys. Dashboard-only — there is no API endpoint to create one. Up to 16 per organization.
  header: Authorization
  in: header
  managed_by_api: false
  name: organization_api_key
  scheme: bearer
  sources:
  - https://documentation.onesignal.com/docs/en/keys-and-ids
  - openapi/_original/onesignal-openapi.yml
  tier: organization
  type: http
- authorization_endpoint: https://dashboard.onesignal.com/oauth/authorize
  description: OAuth 2.1 server backing the hosted MCP endpoint. Added 2026-07-31 so MCP-compatible clients (Claude, Cursor, Copilot, ChatGPT) can connect without a customer pasting an API key. Connected clients are listed in account settings and can be revoked.
  flow: authorization_code
  grant_types:
  - authorization_code
  - refresh_token
  issuer: https://api.onesignal.com
  name: onesignal_oauth
  pkce: required
  pkce_methods:
  - S256
  registration_endpoint: https://api.onesignal.com/oauth/register
  response_types:
  - code
  revocation_endpoint: https://api.onesignal.com/oauth/revoke
  scopes_note: The authorization-server metadata publishes no scopes_supported field and the docs document no scope vocabulary, so there is nothing to record in a scopes artifact. Access appears to be granted per authenticating user across every OneSignal app that user can reach.
  scopes_published: false
  sources:
  - https://api.onesignal.com/.well-known/oauth-authorization-server
  - https://api.onesignal.com/.well-known/oauth-protected-resource
  - https://documentation.onesignal.com/release-notes/changelog
  token_endpoint: https://api.onesignal.com/oauth/token
  token_endpoint_auth_methods:
  - client_secret_post
  - none
  type: oauth2
  used_by: https://api.onesignal.com/mcp/oauth
slug: onesignal-authentication
source_filename: onesignal-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://documentation.onesignal.com/docs/en/keys-and-ids, https://api.onesignal.com/.well-known/oauth-authorization-server,\n  openapi/onesignal-apps-api-openapi.yml\ndocs: https://documentation.onesignal.com/docs/en/keys-and-ids\nprovider: OneSignal\nproviderId: onesignal\ndescription: >-\n  OneSignal authenticates the REST API with bearer API keys in two tiers, and\n  authenticates agent/MCP clients with a separate OAuth 2.1 authorization\n  server. The OAuth server is real and probed — RFC 8414 metadata at\n  api.onesignal.com, PKCE S256 required, RFC 7591 dynamic client registration\n  open — but it is not referenced anywhere in the published OpenAPI, so a spec\n  reader sees only the bearer schemes.\nsummary:\n  types:\n  - http\n  - oauth2\n  primary: API key (bearer)\n  agent_surface: OAuth 2.1 authorization code + PKCE\nschemes:\n- name: rest_api_key\n  type: http\n  scheme: bearer\n  in: header\n  header: Authorization\n\
  \  format: 'Authorization: Key <APP_API_KEY>'\n  tier: app\n  description: >-\n    App API key. Scoped to one app: sending messages, creating and updating\n    users and subscriptions, reading message history and stats. Values are\n    prefixed os_v2_app_ and are shown exactly once, at creation or rotation.\n    Up to 16 per app.\n  managed_by_api: true\n  management_operations:\n  - create-api-key\n  - view-api-keys\n  - update-api-key\n  - rotate-api-key\n  - delete-api-key\n  sources:\n  - https://documentation.onesignal.com/docs/en/keys-and-ids\n  - openapi/onesignal-apps-api-openapi.yml\n- name: organization_api_key\n  type: http\n  scheme: bearer\n  in: header\n  header: Authorization\n  tier: organization\n  description: >-\n    Organization API key. Spans every app in the organization; required for\n    creating apps and managing other API keys. Dashboard-only — there is no API\n    endpoint to create one. Up to 16 per organization.\n  managed_by_api: false\n  sources:\n  - https://documentation.onesignal.com/docs/en/keys-and-ids\n\
  \  - openapi/_original/onesignal-openapi.yml\n- name: onesignal_oauth\n  type: oauth2\n  flow: authorization_code\n  pkce: required\n  pkce_methods:\n  - S256\n  issuer: https://api.onesignal.com\n  authorization_endpoint: https://dashboard.onesignal.com/oauth/authorize\n  token_endpoint: https://api.onesignal.com/oauth/token\n  revocation_endpoint: https://api.onesignal.com/oauth/revoke\n  registration_endpoint: https://api.onesignal.com/oauth/register\n  grant_types:\n  - authorization_code\n  - refresh_token\n  response_types:\n  - code\n  token_endpoint_auth_methods:\n  - client_secret_post\n  - none\n  scopes_published: false\n  scopes_note: >-\n    The authorization-server metadata publishes no scopes_supported field and\n    the docs document no scope vocabulary, so there is nothing to record in a\n    scopes artifact. Access appears to be granted per authenticating user across\n    every OneSignal app that user can reach.\n  used_by: https://api.onesignal.com/mcp/oauth\n  description:\
  \ >-\n    OAuth 2.1 server backing the hosted MCP endpoint. Added 2026-07-31 so\n    MCP-compatible clients (Claude, Cursor, Copilot, ChatGPT) can connect\n    without a customer pasting an API key. Connected clients are listed in\n    account settings and can be revoked.\n  sources:\n  - https://api.onesignal.com/.well-known/oauth-authorization-server\n  - https://api.onesignal.com/.well-known/oauth-protected-resource\n  - https://documentation.onesignal.com/release-notes/changelog\nprotected_resource:\n  resource: https://api.onesignal.com\n  authorization_servers:\n  - https://api.onesignal.com\n  bearer_methods_supported:\n  - header\n  source: https://api.onesignal.com/.well-known/oauth-protected-resource\ncontrols:\n- name: IP allowlist\n  detail: Optional per-key IP allowlist so a leaked key cannot be used from another\n    address. Settable at creation and editable afterwards.\n- name: Key rotation\n  detail: Rotation issues a new secret while keeping the same Key ID, name and\
  \ IP allowlist.\n    The old secret stops working immediately.\n- name: Two-step authentication\n  detail: Organization administrators can enforce 2FA for all team members.\n- name: Single sign-on\n  detail: SSO through WorkOS, integrating major identity providers.\n- name: Identity Verification\n  detail: Optional subscription-level identity verification to prevent impersonation\n    using an exposed subscription_id.\nlegacy:\n  detail: >-\n    App and Organization API keys were introduced November 2024. The legacy User\n    Auth key and original REST API key are still accepted, but their management\n    UI has been removed and new legacy keys cannot be created.\n  source: https://documentation.onesignal.com/docs/en/keys-and-ids\npublic_identifiers:\n- name: App ID\n  secret: false\n  note: Public and safe to share; can only create new user records.\n- name: Organization ID\n  secret: false\nmaintainers:\n- FN: Kin Lane\n  email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/onesignal/refs/heads/main/authentication/onesignal-authentication.yml
summary_line: http/oauth2 · 3 schemes
tags:
- Notifications
- Push
- Email
- SMS
- Mobile
- Push Notifications
- Web Push
- Customer Engagement
- Marketing Automation
- Live Activities
- RCS
- In-App Messaging
- Journeys
- Lifecycle Marketing
- MCP
- Agent Ready
---
