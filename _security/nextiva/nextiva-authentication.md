---
api_key_in: []
api_specs:
- filename: nextiva-authentication-openapi.yml
  format: yaml
  label: Nextiva Provider Authentication API
  slug: provider-authentication
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nextiva/refs/heads/main/openapi/nextiva-authentication-openapi.yml
- filename: nextiva-provider-authentication-openapi.yml
  format: yaml
  label: Nextiva Provider Token Service API
  slug: provider-token-service
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nextiva/refs/heads/main/openapi/nextiva-provider-authentication-openapi.yml
- filename: nextiva-workitem-service-openapi.yml
  format: yaml
  label: Nextiva Workitem Service API
  slug: workitem-service
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nextiva/refs/heads/main/openapi/nextiva-workitem-service-openapi.yml
- filename: nextiva-conversation-openapi.yml
  format: yaml
  label: Nextiva Conversation API
  slug: conversation
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nextiva/refs/heads/main/openapi/nextiva-conversation-openapi.yml
- filename: nextiva-sms-messaging-openapi.yml
  format: yaml
  label: Nextiva SMS Messaging API
  slug: sms-messaging
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nextiva/refs/heads/main/openapi/nextiva-sms-messaging-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Nextiva Authentication
name_suffix: Authentication
oauth_flows: []
overview: Nextiva secures its APIs with http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Nextiva
provider_slug: nextiva
scheme_count: 3
schemes:
- description: Basic authentication using username and password.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/nextiva-authentication-openapi.yml
  type: http
- bearerFormat: JWT
  description: Bearer token authentication (JWT).
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/nextiva-authentication-openapi.yml
  - openapi/nextiva-sms-messaging-openapi.yml
  - openapi/nextiva-workitem-service-openapi.yml
  type: http
- bearerFormat: JWT
  description: Spring Security authentication using JWT tokens. All endpoints require an authenticated user context.
  name: springAuth
  scheme: bearer
  sources:
  - openapi/nextiva-provider-authentication-openapi.yml
  type: http
slug: nextiva-authentication
source_filename: nextiva-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-31'\nmethod: derived\nsource: openapi/nextiva-authentication-openapi.yml, openapi/nextiva-provider-authentication-openapi.yml,\n  openapi/nextiva-sms-messaging-openapi.yml, openapi/nextiva-workitem-service-openapi.yml\ndocs: https://developer.nextiva.com/nextiva/docs/authentication\ndocs_note: >-\n  The developer portal's Authentication page is an unfilled ReadMe placeholder\n  (\"Set up the welcome page for your API to help users make their first call\")\n  as of 2026-07-31, so the auth model below is derived from the published\n  OpenAPI security schemes and the SDK architecture guide rather than from a\n  written auth guide.\nsummary:\n  types: [http]\n  http_schemes: [basic, bearer]\n  bearer_formats: [JWT]\n  api_key_in: []\n  oauth2_flows: []\n  openid_connect: false\n  mutual_tls: false\nmodel: >-\n  Two-step. HTTP basic credentials are exchanged for a JWT that carries the\n  user's authorities; that JWT is then sent as an Authorization bearer token\
  \ on\n  every other operation and refreshed before expiry. There is no OAuth 2.0, no\n  OpenID Connect, no API-key scheme and no mTLS anywhere in the published\n  contracts, so there is also no scope surface (scopes/ is intentionally absent).\nflow:\n- step: 1\n  operation: generateTokenWithAuthorities\n  path: GET https://api.nextiva.com/provider/token-with-authorities\n  auth: basicAuth\n  returns: TokenResponse (JWT + user authorities)\n- step: 2\n  operation: '*'\n  header: 'Authorization: Bearer <jwt>'\n  auth: bearerAuth\n- step: 3\n  operation: refreshToken\n  path: GET https://api.nextiva.com/provider/api/token-refresh\n  auth: bearerAuth\n  returns: RefreshTokenResponse\n  note: A 401 here means the token is already expired — restart at step 1.\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: Basic authentication using username and password.\n  sources:\n  - openapi/nextiva-authentication-openapi.yml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n\
  \  bearerFormat: JWT\n  description: Bearer token authentication (JWT).\n  sources:\n  - openapi/nextiva-authentication-openapi.yml\n  - openapi/nextiva-sms-messaging-openapi.yml\n  - openapi/nextiva-workitem-service-openapi.yml\n- name: springAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: >-\n    Spring Security authentication using JWT tokens. All endpoints require an\n    authenticated user context.\n  sources:\n  - openapi/nextiva-provider-authentication-openapi.yml\nauthorization:\n  model: authorities\n  detail: >-\n    The token embeds the user's \"authorities\" — the Provider Token Service\n    documents generating JWTs with various permission levels, plus time-limited\n    portal access tokens and multi-tenant location-based tokens. A 403 \"Access\n    denied\" is returned when the authenticated user lacks the authority for the\n    requested token scope. No authority/permission catalog is published.\nsdk_handling: >-\n  Per the SDK architecture guide,\
  \ the SDKs post credentials to the Provider\n  Service, receive the token plus a payload describing where to route future\n  requests, and attach the token to the HTTP header automatically on every\n  subsequent call.\ngaps:\n- developer portal authentication page is an empty ReadMe placeholder\n- no published authority/permission reference\n- no token lifetime documented\n- no OAuth 2.0 or OpenID Connect\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nextiva/refs/heads/main/authentication/nextiva-authentication.yml
summary_line: http · 3 schemes
tags:
- Company
- Communications
- Voice
- Contact Center
- Customer Experience
- SMS
- Messaging
- Unified Communications
- VoIP
- Telephony
- Conversational AI
- Call Center
---
