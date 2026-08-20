---
api_key_in:
- header
api_specs:
- filename: decart-api-openapi-original.json
  format: json
  label: Decart API
  slug: decart-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/decart/refs/heads/main/openapi/decart-api-openapi-original.json
auth_types:
- apiKey
description: 'Decart uses a two-tier API-key model. Server-side callers present a permanent account key (dct_ prefix) in an x-api-key request header. Browser and mobile clients never see that key: a backend mints a short-lived ephemeral client token (ek_ prefix) through POST /v1/client/tokens, optionally scoped to a model allow-list, an origin allow-list, and a maximum realtime session duration. There is no OAuth 2.0, OIDC, or mTLS surface. The gRPC Oasis service carries the same account key in its InitializeRequest message rather than an HTTP header.'
kind: authentication
layout: security
method: searched
name: Decart Authentication
name_suffix: Authentication
oauth_flows: []
overview: Decart secures its APIs with apiKey across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Decart
provider_slug: decart
scheme_count: 3
schemes:
- description: Permanent account API key created in the Decart platform console. Required on every REST call. Declared as a required header parameter on each operation rather than as an OpenAPI securityScheme.
  in: header
  name: x-api-key
  parameter: x-api-key
  scope: full account access
  sources:
  - openapi/decart-api-openapi-original.json
  - https://docs.platform.decart.ai/getting-started/authentication
  token_prefix: dct_
  type: apiKey
- constraints:
    allowedModels: Restrict which models this token can access (max 20)
    allowedOrigins: Restrict which web origins this token can be used from (max 20)
    constraints.realtime.maxSessionDuration: Ceiling on a single realtime session, in seconds
    expiresIn: Seconds until the token expires (default 60)
  description: Ephemeral client token minted server-side for browser and mobile realtime sessions. Default TTL 60 seconds. Cannot be used to mint another client token (HTTP 403).
  in: header
  minted_by: POST /v1/client/tokens (create_client_token_v1_client_tokens_post)
  name: client-token
  parameter: x-api-key
  sources:
  - openapi/decart-api-openapi-original.json
  - https://docs.platform.decart.ai/getting-started/client-tokens
  token_prefix: ek_
  type: apiKey
- description: The Oasis 3 Preview action-to-video gRPC service authenticates on the Initialize call by carrying the account API key in the request message. An invalid or missing key returns ERROR_CODE_INVALID_API_KEY.
  in: message-field
  name: grpc-api-key
  parameter: InitializeRequest.api_key
  sources:
  - grpc/decart-a2v.proto
  - https://docs.platform.decart.ai/models/realtime/oasis-3
  type: apiKey
slug: decart-authentication
source_filename: decart-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-01'\nmethod: searched\nsource: https://docs.platform.decart.ai/getting-started/authentication\ndocs: https://docs.platform.decart.ai/getting-started/authentication\nalso: https://docs.platform.decart.ai/getting-started/client-tokens\ndescription: 'Decart uses a two-tier API-key model. Server-side callers present a\n  permanent account key (dct_ prefix) in an x-api-key request header. Browser and\n  mobile clients never see that key: a backend mints a short-lived ephemeral client\n  token (ek_ prefix) through POST /v1/client/tokens, optionally scoped to a model\n  allow-list, an origin allow-list, and a maximum realtime session duration. There\n  is no OAuth 2.0, OIDC, or mTLS surface. The gRPC Oasis service carries the same\n  account key in its InitializeRequest message rather than an HTTP header.'\nsummary:\n  types: [apiKey]\n  api_key_in: [header]\n  oauth2_flows: []\n  openid_connect: false\n  mutual_tls: false\n  ephemeral_tokens: true\nschemes:\n\
  - name: x-api-key\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  token_prefix: dct_\n  description: Permanent account API key created in the Decart platform console. Required\n    on every REST call. Declared as a required header parameter on each operation\n    rather than as an OpenAPI securityScheme.\n  scope: full account access\n  sources:\n  - openapi/decart-api-openapi-original.json\n  - https://docs.platform.decart.ai/getting-started/authentication\n- name: client-token\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  token_prefix: ek_\n  description: Ephemeral client token minted server-side for browser and mobile realtime\n    sessions. Default TTL 60 seconds. Cannot be used to mint another client token\n    (HTTP 403).\n  minted_by: POST /v1/client/tokens (create_client_token_v1_client_tokens_post)\n  constraints:\n    expiresIn: Seconds until the token expires (default 60)\n    allowedModels: Restrict which models this token can access (max 20)\n    allowedOrigins:\
  \ Restrict which web origins this token can be used from (max 20)\n    constraints.realtime.maxSessionDuration: Ceiling on a single realtime session,\n      in seconds\n  sources:\n  - openapi/decart-api-openapi-original.json\n  - https://docs.platform.decart.ai/getting-started/client-tokens\n- name: grpc-api-key\n  type: apiKey\n  in: message-field\n  parameter: InitializeRequest.api_key\n  description: The Oasis 3 Preview action-to-video gRPC service authenticates on the\n    Initialize call by carrying the account API key in the request message. An invalid\n    or missing key returns ERROR_CODE_INVALID_API_KEY.\n  sources:\n  - grpc/decart-a2v.proto\n  - https://docs.platform.decart.ai/models/realtime/oasis-3\nkey_management:\n  console: https://platform.decart.ai/api-keys\n  environment_variable: DECART_API_KEY\n  rotation: Documented as a best practice; no published automated rotation endpoint.\n  separation: Docs advise separate keys for development and production.\nerrors:\n- status:\
  \ 401\n  meaning: No or invalid API key provided\n  operation: create_client_token_v1_client_tokens_post\n- status: 403\n  meaning: Cannot create client token from a client token\n  operation: create_client_token_v1_client_tokens_post\nnotes:\n- Neither published OpenAPI document declares components.securitySchemes. Authentication\n  is expressed as a required `x-api-key` header parameter on each operation, so the\n  mechanical securityScheme derivation returns nothing; this profile is taken from\n  the documented auth pages and the operation parameters instead.\n- No OAuth 2.0 or OpenID Connect surface exists, so scopes/ is intentionally absent\n  rather than empty. Authorization granularity is expressed through client-token constraints\n  (allowedModels / allowedOrigins / maxSessionDuration), not through scopes.\n- Enterprise SSO for organizations is offered for platform console sign-in (May 2026\n  changelog); it governs dashboard access, not API request authentication.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/decart/refs/heads/main/authentication/decart-authentication.yml
summary_line: apiKey · 3 schemes
tags:
- Artificial Intelligence
- Machine-Learning
- Video
- Video Generation
- Video Editing
- Image Editing
- Real-Time
- Generative AI
- World Models
- Streaming
- WebRTC
- Media
- Developer Tools
- Company
---
