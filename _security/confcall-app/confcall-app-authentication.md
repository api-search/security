---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: confcall-app-artifacts-api-openapi.yml
  format: yaml
  label: confcall Artifacts API
  slug: confcall-app-artifacts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/confcall-app/openapi/confcall-app-artifacts-api-openapi.yml
- filename: confcall-app-embed-api-openapi.yml
  format: yaml
  label: confcall Embed API
  slug: confcall-app-embed-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/confcall-app/openapi/confcall-app-embed-api-openapi.yml
- filename: confcall-app-recordings-api-openapi.yml
  format: yaml
  label: confcall Recordings API
  slug: confcall-app-recordings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/confcall-app/openapi/confcall-app-recordings-api-openapi.yml
- filename: confcall-app-rooms-api-openapi.yml
  format: yaml
  label: confcall Rooms API
  slug: confcall-app-rooms-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/confcall-app/openapi/confcall-app-rooms-api-openapi.yml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 4
method: searched
name: confcall Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: confcall secures its APIs with apiKey and oauth2 across 4 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: confcall
provider_slug: confcall-app
scheme_count: 4
schemes:
- description: A confcall secret (sk_live_/sk_test_) API key. Publishable (pk_) keys are rejected on every route documented here.
  in: header
  name: ApiKeyAuth
  parameter: X-API-Key
  sources:
  - openapi/confcall-app-openapi.yml
  type: apiKey
- description: 'OAuth 2.0 client-credentials grant. Exchange a client id/secret at the token URL for a short-lived bearer JWT and send it as `Authorization: Bearer <token>`. Operations with x-auth jwtOrApiKey accept either this or ApiKeyAuth; x-auth jwt operations need a user-context token.'
  flows:
  - flow: clientCredentials
    scopes: 2
    tokenUrl: https://auth.confcall.app/oauth/token
  name: OAuth2ClientCredentials
  sources:
  - openapi/confcall-app-openapi.yml
  type: oauth2
- description: Room/user-scoped JWT. Routes marked "JWT or sk_" accept it; GET /api/recordings/{id} and /download are "JWT only" (human session). Embed session tokens from POST /api/embed/sessions feed the widget auth-token attribute.
  name: RoomScopedJWT
  scheme: bearer
  sources:
  - https://docs.confcall.app/api-reference.html
  - https://docs.confcall.app/widget.html
  type: http
- description: pk_live_/pk_test_ publishable key for the <agent-widget> only; can be restricted to allowed origins. Rejected on every control-plane route.
  in: attribute
  name: PublishableKey
  parameter: api-key
  sources:
  - https://docs.confcall.app/agent-widget.html
  type: apiKey
slug: confcall-app-authentication
source_filename: confcall-app-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://docs.confcall.app/api-reference.html\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: A confcall secret (sk_live_/sk_test_) API key. Publishable (pk_) keys are rejected on every route\n    documented here.\n  sources:\n  - openapi/confcall-app-openapi.yml\n- name: OAuth2ClientCredentials\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.confcall.app/oauth/token\n    scopes: 2\n  description: 'OAuth 2.0 client-credentials grant. Exchange a client id/secret at the token URL for a short-lived\n    bearer JWT and send it as `Authorization: Bearer <token>`. Operations with x-auth jwtOrApiKey accept either\n    this or ApiKeyAuth; x-auth jwt operations need a user-context token.'\n  sources:\n  - openapi/confcall-app-openapi.yml\n\
  - name: RoomScopedJWT\n  type: http\n  scheme: bearer\n  description: Room/user-scoped JWT. Routes marked \"JWT or sk_\" accept it; GET /api/recordings/{id} and /download\n    are \"JWT only\" (human session). Embed session tokens from POST /api/embed/sessions feed the widget auth-token\n    attribute.\n  sources:\n  - https://docs.confcall.app/api-reference.html\n  - https://docs.confcall.app/widget.html\n- name: PublishableKey\n  type: apiKey\n  in: attribute\n  parameter: api-key\n  description: pk_live_/pk_test_ publishable key for the <agent-widget> only; can be restricted to allowed origins.\n    Rejected on every control-plane route.\n  sources:\n  - https://docs.confcall.app/agent-widget.html\ndocs: https://docs.confcall.app/api-reference.html\nkey_prefixes:\n  secret:\n  - sk_live_\n  - sk_test_\n  publishable:\n  - pk_live_\n  - pk_test_\nnotes:\n- 'MCP server (https://mcp.confcall.app) accepts X-API-Key: sk_... or Authorization: Bearer sk_...; a request with\n  no key is rejected\
  \ with 401 (per docs, not probed).'\n- Keys are created in the dashboard at meet.confcall.app under Developers / API & Embed.\ndocs_pages:\n- https://docs.confcall.app/api-reference.html\n- https://docs.confcall.app/mcp-server.html\n- https://docs.confcall.app/agent-widget.html\n"
source_yaml_url: https://artifacts.apis.io/confcall-app/authentication/confcall-app-authentication.yml
summary_line: apiKey/oauth2 · 4 schemes
tags:
- Company
- Video Conferencing
- AI Agents
- Embeddable Widgets
- Telephony
- Transcription
- MCP
- Communications
---
