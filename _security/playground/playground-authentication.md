---
anonymous_access: false
api_key_in: []
api_specs:
- filename: playground-auth-api-openapi.yml
  format: yaml
  label: Playground API — Free Stateful Mock REST & GraphQL Service Auth API
  slug: playground-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/playground/refs/heads/main/openapi/playground-auth-api-openapi.yml
- filename: playground-avatars-api-openapi.yml
  format: yaml
  label: Playground API — Free Stateful Mock REST & GraphQL Service Avatars API
  slug: playground-avatars-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/playground/refs/heads/main/openapi/playground-avatars-api-openapi.yml
- filename: playground-comments-api-openapi.yml
  format: yaml
  label: Playground API — Free Stateful Mock REST & GraphQL Service Comments API
  slug: playground-comments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/playground/refs/heads/main/openapi/playground-comments-api-openapi.yml
- filename: playground-custom-api-openapi.yml
  format: yaml
  label: Playground API — Free Stateful Mock REST & GraphQL Service Custom API
  slug: playground-custom-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/playground/refs/heads/main/openapi/playground-custom-api-openapi.yml
- filename: playground-posts-api-openapi.yml
  format: yaml
  label: Playground API — Free Stateful Mock REST & GraphQL Service Posts API
  slug: playground-posts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/playground/refs/heads/main/openapi/playground-posts-api-openapi.yml
- filename: playground-session-api-openapi.yml
  format: yaml
  label: Playground API — Free Stateful Mock REST & GraphQL Service Session API
  slug: playground-session-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/playground/refs/heads/main/openapi/playground-session-api-openapi.yml
- filename: playground-thumbnails-api-openapi.yml
  format: yaml
  label: Playground API — Free Stateful Mock REST & GraphQL Service Thumbnails API
  slug: playground-thumbnails-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/playground/refs/heads/main/openapi/playground-thumbnails-api-openapi.yml
- filename: playground-users-api-openapi.yml
  format: yaml
  label: Playground API — Free Stateful Mock REST & GraphQL Service Users API
  slug: playground-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/playground/refs/heads/main/openapi/playground-users-api-openapi.yml
- filename: playground-to-dos-api-openapi.yml
  format: yaml
  label: Playground API — Free Stateful Mock REST & GraphQL Service To Dos API
  slug: playground-to-dos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/playground/refs/heads/main/openapi/playground-to-dos-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Playground Authentication
name_suffix: Authentication
oauth_flows: []
overview: Playground API — Free Stateful Mock REST & GraphQL Service declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Playground API — Free Stateful Mock REST & GraphQL Service
provider_slug: playground
scheme_count: 1
schemes:
- applies_to:
  - GET /api/v1/auth/me
  - PATCH /api/v1/auth/me
  bearerFormat: JWT
  description: Simulated JWT bearer token obtained from POST /auth/login, /auth/register or /auth/refresh. Applies only to GET /auth/me and PATCH /auth/me. Access token lifetime is 900 seconds (expires_in), refreshable via the refresh token. Not a real credential; issued to any caller.
  name: bearerAuth
  scheme: bearer
  type: http
slug: playground-authentication
source_filename: playground-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-14'\nmethod: searched\nsource: >-\n  https://playground.nileslabs.com/llms-full.txt (Resource: Authentication) and\n  https://playground.nileslabs.com/product.json (authentication block), fetched\n  2026-09-14. The published OpenAPI declares no securitySchemes, so this profile\n  is authored from the provider's own documentation.\napi: Playground REST API\nsummary: >-\n  The API is public and requires NO authentication for the mock data surface\n  (users, posts, comments, todos, custom collections, media, session). A\n  SIMULATED JWT flow exists purely so developers can exercise bearer-protected\n  routes: POST /auth/login and POST /auth/register return signed HS256 JWT\n  access + refresh tokens, POST /auth/refresh rotates them, and GET/PATCH\n  /auth/me require an Authorization: Bearer <access_token> header. Tokens are\n  cosmetic sandbox artifacts, not real credentials — any username/password is\n  accepted and no account is provisioned.\nrequired: false\n\
  schemes:\n  - name: bearerAuth\n    type: http\n    scheme: bearer\n    bearerFormat: JWT\n    description: >-\n      Simulated JWT bearer token obtained from POST /auth/login, /auth/register\n      or /auth/refresh. Applies only to GET /auth/me and PATCH /auth/me. Access\n      token lifetime is 900 seconds (expires_in), refreshable via the refresh\n      token. Not a real credential; issued to any caller.\n    applies_to:\n      - GET /api/v1/auth/me\n      - PATCH /api/v1/auth/me\nsession_identity:\n  description: >-\n    Session state (the per-session mutation overlay), not authentication, is how\n    Playground isolates callers. In browsers, send credentials: 'include' /\n    withCredentials so the session cookie is carried. In non-browser clients\n    (Node, Playwright, cURL) send a stable X-Playground-Identity: <session-id>\n    header to bind mutations to a private overlay.\n  browser: cookie via credentials:'include'\n  non_browser_header: X-Playground-Identity\ntoken_endpoints:\n\
  \  login: POST /api/v1/auth/login\n  register: POST /api/v1/auth/register\n  refresh: POST /api/v1/auth/refresh\n  profile: GET /api/v1/auth/me\nnotes: >-\n  No OAuth2/OIDC: /.well-known/openid-configuration and\n  /.well-known/oauth-authorization-server both 404. No API keys, no signup, no\n  billing. MIT licensed.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/playground/refs/heads/main/authentication/playground-authentication.yml
summary_line: 1 scheme
tags:
- Developer Tools
- Testing
- Mock API
- api-sandbox
- REST
- GraphQL
- E2E Testing
---
