---
anonymous_access: false
api_key_in: []
api_specs:
- filename: api-video-videos-api-openapi.yml
  format: yaml
  label: API.Video Videos API
  slug: api-video-videos-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/api-video/openapi/api-video-videos-api-openapi.yml
- filename: api-video-advanced-authentication-api-openapi.yml
  format: yaml
  label: API.Video Advanced authentication API
  slug: api-video-advanced-authentication-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/api-video/openapi/api-video-advanced-authentication-api-openapi.yml
- filename: api-video-analytics-api-openapi.yml
  format: yaml
  label: API.Video Analytics API
  slug: api-video-analytics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/api-video/openapi/api-video-analytics-api-openapi.yml
- filename: api-video-captions-api-openapi.yml
  format: yaml
  label: API.Video Captions API
  slug: api-video-captions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/api-video/openapi/api-video-captions-api-openapi.yml
- filename: api-video-chapters-api-openapi.yml
  format: yaml
  label: API.Video Chapters API
  slug: api-video-chapters-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/api-video/openapi/api-video-chapters-api-openapi.yml
- filename: api-video-live-streams-api-openapi.yml
  format: yaml
  label: API.Video Live Streams API
  slug: api-video-live-streams-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/api-video/openapi/api-video-live-streams-api-openapi.yml
- filename: api-video-player-themes-api-openapi.yml
  format: yaml
  label: API.Video Player Themes API
  slug: api-video-player-themes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/api-video/openapi/api-video-player-themes-api-openapi.yml
- filename: api-video-summaries-api-openapi.yml
  format: yaml
  label: API.Video Summaries API
  slug: api-video-summaries-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/api-video/openapi/api-video-summaries-api-openapi.yml
- filename: api-video-tags-api-openapi.yml
  format: yaml
  label: API.Video Tags API
  slug: api-video-tags-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/api-video/openapi/api-video-tags-api-openapi.yml
- filename: api-video-upload-tokens-api-openapi.yml
  format: yaml
  label: API.Video Upload Tokens API
  slug: api-video-upload-tokens-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/api-video/openapi/api-video-upload-tokens-api-openapi.yml
- filename: api-video-watermarks-api-openapi.yml
  format: yaml
  label: API.Video Watermarks API
  slug: api-video-watermarks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/api-video/openapi/api-video-watermarks-api-openapi.yml
- filename: api-video-webhooks-api-openapi.yml
  format: yaml
  label: API.Video Webhooks API
  slug: api-video-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/api-video/openapi/api-video-webhooks-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Api Video Authentication
name_suffix: Authentication
oauth_flows: []
overview: API.Video secures its APIs with http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: API.Video
provider_slug: api-video
scheme_count: 3
schemes:
- description: 'HTTP Basic Auth with the API key as the username and an empty password ("curl -u api_key: https://ws.api.video/videos"; keep the trailing colon). Invalid credentials return 401 Unauthorized with a problem+json body.'
  docs: https://docs.api.video/reference/basic-authentication
  name: apiKey
  scheme: basic
  sources:
  - openapi/api-video-advanced-authentication-api-openapi.yml
  - openapi/api-video-analytics-api-openapi.yml
  - openapi/api-video-captions-api-openapi.yml
  - openapi/api-video-chapters-api-openapi.yml
  - openapi/api-video-live-streams-api-openapi.yml
  - openapi/api-video-player-themes-api-openapi.yml
  - openapi/api-video-summaries-api-openapi.yml
  - openapi/api-video-tags-api-openapi.yml
  - openapi/api-video-upload-tokens-api-openapi.yml
  - openapi/api-video-videos-api-openapi.yml
  - openapi/api-video-watermarks-api-openapi.yml
  - openapi/api-video-webhooks-api-openapi.yml
  type: http
- bearerFormat: JWT
  description: 'Disposable bearer token. POST /auth/api-key with {"apiKey": ...} returns access_token (JWT, valid 3600 seconds), token_type "bearer", refresh_token and expires_in; POST /auth/refresh with {"refreshToken": ...} rotates it. Send as "Authorization: Bearer <access_token>". The docs suggest either a scheduled refresh every 3600 seconds or refreshing on a 401.'
  docs: https://docs.api.video/reference/disposable-bearer-token-authentication
  name: bearerAuth
  refresh_endpoint: POST https://ws.api.video/auth/refresh
  scheme: bearer
  sources:
  - openapi/api-video-advanced-authentication-api-openapi.yml
  - openapi/api-video-analytics-api-openapi.yml
  - openapi/api-video-captions-api-openapi.yml
  - openapi/api-video-chapters-api-openapi.yml
  - openapi/api-video-live-streams-api-openapi.yml
  - openapi/api-video-player-themes-api-openapi.yml
  - openapi/api-video-summaries-api-openapi.yml
  - openapi/api-video-tags-api-openapi.yml
  - openapi/api-video-upload-tokens-api-openapi.yml
  - openapi/api-video-videos-api-openapi.yml
  - openapi/api-video-watermarks-api-openapi.yml
  - openapi/api-video-webhooks-api-openapi.yml
  token_endpoint: POST https://ws.api.video/auth/api-key
  token_lifetime_seconds: 3600
  type: http
- description: Not a securityScheme in the OpenAPI, but a documented credential - POST /upload-tokens (optionally with a ttl) issues a token an end user passes to POST /upload?token=... so browsers and mobile apps can upload without the account API key. Tokens are listed, retrieved and deleted at /upload-tokens; the docs recommend the shortest TTL possible.
  docs: https://docs.api.video/reference/api/Upload-Tokens
  in: query
  name: delegated upload token
  scheme: null
  sources:
  - openapi/api-video-upload-tokens-api-openapi.yml
  - openapi/api-video-videos-api-openapi.yml
  type: apiKey
slug: api-video-authentication
source_filename: api-video-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: searched\nsource: 'https://docs.api.video/reference/authentication-guide, https://docs.api.video/reference/basic-authentication, https://docs.api.video/reference/disposable-bearer-token-authentication, https://docs.api.video/reference/api/Advanced-authentication, https://docs.api.video/reference/api/Upload-Tokens, https://docs.api.video/sdks/security/; securitySchemes of openapi/_original/api-video-openapi.yml (bearerAuth: http bearer; apiKey: http basic)'\ndocs: https://docs.api.video/reference/authentication-guide\nsummary:\n  types: [http]\n  schemes: [basic, bearer]\n  recommended: Disposable bearer token (the official clients use it by default); Basic auth is positioned for quick testing.\n  environments: separate API keys for sandbox (https://sandbox.api.video) and production (https://ws.api.video); a key used against the wrong environment returns 401.\n  key_management: API keys are created on https://dashboard.api.video (API Keys page);\
  \ production allows multiple keys per project for different applications. The docs tell developers never to ship keys in frontend or mobile code.\nschemes:\n  - name: apiKey\n    type: http\n    scheme: basic\n    description: 'HTTP Basic Auth with the API key as the username and an empty password (\"curl -u api_key: https://ws.api.video/videos\"; keep the trailing colon). Invalid credentials return 401 Unauthorized with a problem+json body.'\n    docs: https://docs.api.video/reference/basic-authentication\n    sources:\n      - openapi/api-video-advanced-authentication-api-openapi.yml\n      - openapi/api-video-analytics-api-openapi.yml\n      - openapi/api-video-captions-api-openapi.yml\n      - openapi/api-video-chapters-api-openapi.yml\n      - openapi/api-video-live-streams-api-openapi.yml\n      - openapi/api-video-player-themes-api-openapi.yml\n      - openapi/api-video-summaries-api-openapi.yml\n      - openapi/api-video-tags-api-openapi.yml\n      - openapi/api-video-upload-tokens-api-openapi.yml\n\
  \      - openapi/api-video-videos-api-openapi.yml\n      - openapi/api-video-watermarks-api-openapi.yml\n      - openapi/api-video-webhooks-api-openapi.yml\n  - name: bearerAuth\n    type: http\n    scheme: bearer\n    bearerFormat: JWT\n    description: 'Disposable bearer token. POST /auth/api-key with {\"apiKey\": ...} returns access_token (JWT, valid 3600 seconds), token_type \"bearer\", refresh_token and expires_in; POST /auth/refresh with {\"refreshToken\": ...} rotates it. Send as \"Authorization: Bearer <access_token>\". The docs suggest either a scheduled refresh every 3600 seconds or refreshing on a 401.'\n    token_endpoint: POST https://ws.api.video/auth/api-key\n    refresh_endpoint: POST https://ws.api.video/auth/refresh\n    token_lifetime_seconds: 3600\n    docs: https://docs.api.video/reference/disposable-bearer-token-authentication\n    sources:\n      - openapi/api-video-advanced-authentication-api-openapi.yml\n      - openapi/api-video-analytics-api-openapi.yml\n   \
  \   - openapi/api-video-captions-api-openapi.yml\n      - openapi/api-video-chapters-api-openapi.yml\n      - openapi/api-video-live-streams-api-openapi.yml\n      - openapi/api-video-player-themes-api-openapi.yml\n      - openapi/api-video-summaries-api-openapi.yml\n      - openapi/api-video-tags-api-openapi.yml\n      - openapi/api-video-upload-tokens-api-openapi.yml\n      - openapi/api-video-videos-api-openapi.yml\n      - openapi/api-video-watermarks-api-openapi.yml\n      - openapi/api-video-webhooks-api-openapi.yml\n  - name: delegated upload token\n    type: apiKey\n    in: query\n    scheme: null\n    description: Not a securityScheme in the OpenAPI, but a documented credential - POST /upload-tokens (optionally with a ttl) issues a token an end user passes to POST /upload?token=... so browsers and mobile apps can upload without the account API key. Tokens are listed, retrieved and deleted at /upload-tokens; the docs recommend the shortest TTL possible.\n    docs: https://docs.api.video/reference/api/Upload-Tokens\n\
  \    sources:\n      - openapi/api-video-upload-tokens-api-openapi.yml\n      - openapi/api-video-videos-api-openapi.yml\nerrors:\n  - {status: 401, title: The API key is invalid.}\n  - {status: 401, title: The access token is invalid or expired.}\n  - {status: 401, title: The refresh token is invalid.}\n  - {status: 401, title: The \"Authorization\" header is missing.}\n  - {status: 403, title: Suspended account}\n"
source_yaml_url: https://artifacts.apis.io/api-video/authentication/api-video-authentication.yml
summary_line: http · 3 schemes
tags:
- Artificial Intelligence
- Analytics
- CDN
- Encoding
- Live Streaming
- Transcription
- Video
- Video-on-Demand
---
