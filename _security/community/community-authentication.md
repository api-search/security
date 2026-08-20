---
api_key_in:
- header
api_specs:
- filename: community-member-data-api-openapi.yml
  format: yaml
  label: Community member-data API
  slug: community-member-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/community/refs/heads/main/openapi/community-member-data-api-openapi.yml
- filename: community-messaging-api-openapi.yml
  format: yaml
  label: Community messaging API
  slug: community-messaging-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/community/refs/heads/main/openapi/community-messaging-api-openapi.yml
- filename: community-tags-api-openapi.yml
  format: yaml
  label: Community tags API
  slug: community-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/community/refs/heads/main/openapi/community-tags-api-openapi.yml
auth_types:
- http
- oauth2
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Community Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Community secures its APIs with http, oauth2, and apiKey across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Community
provider_slug: community
scheme_count: 3
schemes:
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/_original/community-async-openapi-original.yml
  type: http
- flows:
  - authorizationUrl: https://oauth-login.community.com/
    flow: authorizationCode
    scopes: 0
    tokenUrl: https://api.community.com/oauth/v1/token
  name: oAuth
  notes: The OpenAPI declares tokenUrl as the relative path /oauth/v1/token; the Sample Code page publishes the absolute form https://api.community.com/oauth/v1/token. The docs value is recorded here. The scopes map is empty in the spec and the sample requests scope=[], so Community's OAuth has no published scope surface.
  sources:
  - openapi/_original/community-async-openapi-original.yml
  - https://developer.community.com/reference/sample-code
  type: oauth2
- applies_to:
  - Async REST API
  - Data Export API
  format: Bearer <API Token>
  in: header
  management: Community Dashboard -> Settings > API Tokens (a.k.a. Settings > Auth Tokens)
  name: apiToken
  notes: Not present in the OpenAPI — captured from the docs. This is the primary, documented credential for both APIs; the token is prefixed community_api and is presented as a bearer token in the Authorization header.
  parameter: Authorization
  sources:
  - https://developer.community.com/reference/webhook-api-authentication
  - https://developer.community.com/reference/data-export-api-authentication
  token_prefix: community_api
  type: apiKey
slug: community-authentication
source_filename: community-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: openapi/_original/community-async-openapi-original.yml\ndocs:\n- https://developer.community.com/reference/webhook-api-authentication\n- https://developer.community.com/reference/data-export-api-authentication\n- https://developer.community.com/reference/sample-code\nsummary:\n  types:\n  - http\n  - oauth2\n  - apiKey\n  api_key_in:\n  - header\n  oauth2_flows:\n  - authorizationCode\n  provisioning: >-\n    Not self-serve. An account seat must have Async REST API and/or Data Export\n    access enabled by the Community team before any credential can be issued\n    (technical onboarding packet; saleseng@community.com).\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/_original/community-async-openapi-original.yml\n- name: oAuth\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://oauth-login.community.com/\n    tokenUrl: https://api.community.com/oauth/v1/token\n\
  \    scopes: 0\n  sources:\n  - openapi/_original/community-async-openapi-original.yml\n  - https://developer.community.com/reference/sample-code\n  notes: >-\n    The OpenAPI declares tokenUrl as the relative path /oauth/v1/token; the\n    Sample Code page publishes the absolute form\n    https://api.community.com/oauth/v1/token. The docs value is recorded here.\n    The scopes map is empty in the spec and the sample requests scope=[], so\n    Community's OAuth has no published scope surface.\n- name: apiToken\n  type: apiKey\n  in: header\n  parameter: Authorization\n  format: 'Bearer <API Token>'\n  token_prefix: community_api\n  management: Community Dashboard -> Settings > API Tokens (a.k.a. Settings > Auth Tokens)\n  applies_to:\n  - Async REST API\n  - Data Export API\n  sources:\n  - https://developer.community.com/reference/webhook-api-authentication\n  - https://developer.community.com/reference/data-export-api-authentication\n  notes: >-\n    Not present in the OpenAPI — captured\
  \ from the docs. This is the primary,\n    documented credential for both APIs; the token is prefixed community_api and\n    is presented as a bearer token in the Authorization header.\ntoken_lifetimes:\n- credential: OAuth 2.0 access token (JWT)\n  lifetime: 60 minutes\n  refresh: OAuth refresh_token issued alongside the access token\n  source: https://developer.community.com/reference/sample-code\n- credential: Seat Context session token (JWT)\n  lifetime: 7 days\n  revocation: DELETE https://dl.community.com/download/v2/auth/logout\n  source: https://developer.community.com/reference/data-export-api-authentication\n- credential: Data Export download redirect URL\n  lifetime: 15 minutes\n  source: https://developer.community.com/reference/data-export-api-downloading-data\n  notes: Time-limited redirect; must not be cached.\nseat_context_api:\n  purpose: >-\n    Alternative Data Export authentication for enterprises managing several\n    Community accounts from one seat (email). Login\
  \ returns a JWT scoped to a\n    client_id; the caller then lists and switches account contexts.\n  base: https://dl.community.com/download/v2\n  operations:\n  - method: POST\n    path: /auth/login\n    description: Establish a session from an account seat email + password; returns seat_id, client_id, device_id and a JWT.\n  - method: POST\n    path: /auth/login/callback/mfa\n    description: Complete two-factor authentication with a six-digit TOTP code when 2FA is enabled on any account the seat can reach.\n  - method: GET\n    path: /auth/context\n    description: List the Community accounts (contexts) the seat can access, each identified by client_id.\n  - method: PUT\n    path: /auth/context\n    description: Switch to a given client_id context and receive a new JWT scoped to it.\n  - method: DELETE\n    path: /auth/logout\n    description: Expire the session token before its 7-day lifetime elapses.\n  mfa: TOTP six-digit code, required when 2FA is enabled on the account\n  source:\
  \ https://developer.community.com/reference/data-export-api-authentication\nwebhook_authentication:\n  direction: inbound (Community -> subscriber endpoint)\n  header: community-signature\n  scheme: HMAC computed with a per-webhook shared signature secret\n  source: https://developer.community.com/reference/webhooks-introduction\nnotes: >-\n  Upgraded from derived to searched on 2026-08-13. The OpenAPI only declares\n  bearerAuth and oAuth; the developer docs add the primary credential actually\n  issued to customers (a community_api-prefixed API token), the concrete token\n  lifetimes, and the Seat Context API used for multi-account Data Export access.\n  No scopes are published for the oauth2 flow — see scopes/community-scopes.yml.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/community/refs/heads/main/authentication/community-authentication.yml
summary_line: http/oauth2/apiKey · 3 schemes
tags:
- Messaging
- SMS
- Communications
- Conversational
- Marketing
- Creators
- Webhook
- Company
---
