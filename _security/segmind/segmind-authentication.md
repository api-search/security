---
api_key_in:
- header
api_specs:
- filename: segmind-inference-api-openapi.yml
  format: yaml
  label: Segmind Inference API
  slug: segmind-inference-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/segmind/refs/heads/main/openapi/segmind-inference-api-openapi.yml
- filename: segmind-account-api-openapi.yml
  format: yaml
  label: Segmind Account API
  slug: segmind-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/segmind/refs/heads/main/openapi/segmind-account-api-openapi.yml
- filename: segmind-storage-api-openapi.yml
  format: yaml
  label: Segmind Storage API
  slug: segmind-storage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/segmind/refs/heads/main/openapi/segmind-storage-api-openapi.yml
- filename: segmind-fine-tuning-api-openapi.yml
  format: yaml
  label: Segmind Fine-tuning API
  slug: segmind-fine-tuning-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/segmind/refs/heads/main/openapi/segmind-fine-tuning-api-openapi.yml
auth_types:
- apiKey
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Segmind Authentication
name_suffix: Authentication
oauth_flows: []
overview: Segmind secures its APIs with apiKey, http, and oauth2 across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Segmind
provider_slug: segmind
scheme_count: 4
schemes:
- expiry: API keys do not expire. The docs recommend rotating them periodically.
  hosts:
  - https://api.segmind.com
  - https://workflows-api.segmind.com
  - https://api.spotprod.segmind.com
  in: header
  key_format:
    body: 16 hexadecimal characters
    example_shape: SG_0123456789abcdef
    prefix: SG_
    total_length: 19
  management:
    console: https://platform.segmind.com/api-keys
    console_path: Developer -> API Keys
    create: 'POST https://platform.segmind.com/api/keys (Authorization: Bearer <access_token>)'
    note: Key management is itself a bearer-token operation on the platform host, not an x-api-key operation on the gateway — so a key cannot rotate itself.
    revoke: DELETE https://platform.segmind.com/api/keys/{key_id}
  name: apiKeyAuth
  parameter: x-api-key
  sources:
  - openapi/segmind-inference-api-openapi.yml
  - openapi/segmind-account-api-openapi.yml
  - openapi/segmind-fine-tuning-api-openapi.yml
  - openapi/segmind-storage-api-openapi.yml
  - https://docs.segmind.com/docs/get-started/authentication
  surface: AI Gateway
  type: apiKey
  verification: 'GET https://api.segmind.com/v1/get-user-credits is documented as the cheapest way to confirm a key works: it runs no model and costs nothing.'
- access_token_lifetime: 1 hour
  bearerFormat: JWT
  claims:
  - jti
  - exp
  - iat
  - nbf
  - identity
  cookie: The access token is also stored automatically in an HTTP-only secure cookie with a 30-day expiration, used for subsequent console requests.
  header: 'Authorization: Bearer <access_token>'
  host: https://platform.segmind.com
  identity_claim: identity — the email of the token user
  in_openapi: false
  name: bearerJWT
  note: Not accepted by the AI Gateway. Sending a bearer token to api.segmind.com returns 401 regardless of the endpoint.
  refresh: 'POST https://platform.segmind.com/auth/refresh with Authorization: Bearer <refresh_token>'
  refresh_token_lifetime: 30 days
  scheme: bearer
  surface: Platform / console API
  type: http
- authorization_url: https://platform.segmind.com/auth/login
  flow: authorizationCode
  in_openapi: false
  name: oauth2SocialLogin
  note: These are the scopes Segmind requests AT the identity provider in order to sign a user in — they are not Segmind API scopes. See scopes/segmind-scopes.yml.
  providers:
  - name: Google
    scopes:
    - email
    - profile
  - name: Microsoft
    scopes:
    - user.read
    - profile
    - email
  - name: Discord
    scopes:
    - identify
    - email
    - guilds
  redirect_url: https://platform.segmind.com/api/login/{provider}/authorized
  surface: Platform sign-in
  token_response: '{"access_token": "...", "refresh_token": "...", "expires_in": 3600}'
  type: oauth2
- announced: '2026-06-16'
  description: Segmind runs an OAuth 2.1 authorization server so third-party applications, "including MCP clients", can request scoped, user-authorized access and call the API without ever handling an API key. Described as fully additive.
  discoverable: false
  endpoint_base: /oauth/ (host not stated in the release note)
  in_openapi: false
  name: oauth21AuthorizationServer
  note: 'Not discoverable and not documented beyond the release note. There is no /.well-known/oauth-authorization-server (RFC 8414) or /.well-known/oauth-protected-resource (RFC 9728) on any Segmind host, no scope reference, no registration flow, and no page under /docs describing it. Probed 2026-08-27: platform.segmind.com/.well-known/oauth-authorization-server -> 404, platform.segmind.com/oauth/authorize -> 404, api.segmind.com/oauth/authorize -> 400. Recorded as announced-but-undiscoverable rather than as a usable scheme.'
  source: https://docs.segmind.com/docs/platform/release-notes/2026-06-21-weekly
  status: announced
  surface: Third-party application access
  type: oauth2
slug: segmind-authentication
source_filename: segmind-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-27'\nmethod: searched\nsource: >-\n  https://docs.segmind.com/docs/get-started/authentication,\n  https://docs.segmind.com/docs/serverless-api,\n  https://docs.segmind.com/docs/platform/account-and-billing-apis,\n  https://docs.segmind.com/docs/pixelflow/api-reference,\n  https://docs.segmind.com/docs/platform/release-notes/2026-06-21-weekly,\n  openapi/ in this repo\ndocs: https://docs.segmind.com/docs/get-started/authentication\nsummary:\n  types:\n    - apiKey\n    - http\n    - oauth2\n  api_key_in:\n    - header\n  primary: 'API key in the x-api-key header'\n  note: >-\n    Three distinct auth models on two distinct surfaces. The AI Gateway\n    (api.segmind.com, workflows-api.segmind.com, api.spotprod.segmind.com) takes an API\n    key in x-api-key and NOTHING else — it rejects the same key as a bearer token with 401.\n    The platform/console surface (platform.segmind.com) takes a JWT bearer token obtained\n    through OAuth 2.0 social login. Since\
  \ June 2026 Segmind also runs its own OAuth 2.1\n    authorization server for third-party apps and MCP clients.\nschemes:\n  - name: apiKeyAuth\n    type: apiKey\n    in: header\n    parameter: x-api-key\n    surface: AI Gateway\n    hosts:\n      - https://api.segmind.com\n      - https://workflows-api.segmind.com\n      - https://api.spotprod.segmind.com\n    key_format:\n      prefix: SG_\n      body: 16 hexadecimal characters\n      total_length: 19\n      example_shape: SG_0123456789abcdef\n    expiry: >-\n      API keys do not expire. The docs recommend rotating them periodically.\n    management:\n      console: https://platform.segmind.com/api-keys\n      console_path: Developer -> API Keys\n      create: 'POST https://platform.segmind.com/api/keys (Authorization: Bearer <access_token>)'\n      revoke: 'DELETE https://platform.segmind.com/api/keys/{key_id}'\n      note: >-\n        Key management is itself a bearer-token operation on the platform host, not an\n        x-api-key\
  \ operation on the gateway — so a key cannot rotate itself.\n    verification: >-\n      GET https://api.segmind.com/v1/get-user-credits is documented as the cheapest way to\n      confirm a key works: it runs no model and costs nothing.\n    sources:\n      - openapi/segmind-inference-api-openapi.yml\n      - openapi/segmind-account-api-openapi.yml\n      - openapi/segmind-fine-tuning-api-openapi.yml\n      - openapi/segmind-storage-api-openapi.yml\n      - https://docs.segmind.com/docs/get-started/authentication\n  - name: bearerJWT\n    type: http\n    scheme: bearer\n    bearerFormat: JWT\n    surface: Platform / console API\n    host: https://platform.segmind.com\n    header: 'Authorization: Bearer <access_token>'\n    claims: [jti, exp, iat, nbf, identity]\n    identity_claim: 'identity — the email of the token user'\n    access_token_lifetime: 1 hour\n    refresh_token_lifetime: 30 days\n    refresh: 'POST https://platform.segmind.com/auth/refresh with Authorization: Bearer <refresh_token>'\n\
  \    cookie: >-\n      The access token is also stored automatically in an HTTP-only secure cookie with a\n      30-day expiration, used for subsequent console requests.\n    note: >-\n      Not accepted by the AI Gateway. Sending a bearer token to api.segmind.com returns\n      401 regardless of the endpoint.\n    in_openapi: false\n  - name: oauth2SocialLogin\n    type: oauth2\n    flow: authorizationCode\n    surface: Platform sign-in\n    authorization_url: https://platform.segmind.com/auth/login\n    redirect_url: 'https://platform.segmind.com/api/login/{provider}/authorized'\n    token_response: '{\"access_token\": \"...\", \"refresh_token\": \"...\", \"expires_in\": 3600}'\n    providers:\n      - name: Google\n        scopes: [email, profile]\n      - name: Microsoft\n        scopes: [user.read, profile, email]\n      - name: Discord\n        scopes: [identify, email, guilds]\n    note: >-\n      These are the scopes Segmind requests AT the identity provider in order to sign a\n\
  \      user in — they are not Segmind API scopes. See scopes/segmind-scopes.yml.\n    in_openapi: false\n  - name: oauth21AuthorizationServer\n    type: oauth2\n    surface: Third-party application access\n    status: announced\n    announced: '2026-06-16'\n    endpoint_base: '/oauth/ (host not stated in the release note)'\n    description: >-\n      Segmind runs an OAuth 2.1 authorization server so third-party applications,\n      \"including MCP clients\", can request scoped, user-authorized access and call the API\n      without ever handling an API key. Described as fully additive.\n    discoverable: false\n    note: >-\n      Not discoverable and not documented beyond the release note. There is no\n      /.well-known/oauth-authorization-server (RFC 8414) or\n      /.well-known/oauth-protected-resource (RFC 9728) on any Segmind host, no scope\n      reference, no registration flow, and no page under /docs describing it. Probed\n      2026-08-27: platform.segmind.com/.well-known/oauth-authorization-server\
  \ -> 404,\n      platform.segmind.com/oauth/authorize -> 404, api.segmind.com/oauth/authorize -> 400.\n      Recorded as announced-but-undiscoverable rather than as a usable scheme.\n    in_openapi: false\n    source: https://docs.segmind.com/docs/platform/release-notes/2026-06-21-weekly\nmutual_tls: false\nopenid_connect: false\nerrors:\n  - status: 401\n    code: invalid_token\n    description: Token is invalid or expired.\n  - status: 401\n    code: invalid_api_key\n    description: API key is invalid.\n  - status: 403\n    code: insufficient_scope\n    description: Token lacks required permissions.\n  - status: 429\n    code: rate_limit_exceeded\n    description: Too many requests.\nauth_rate_limits:\n  - scope: ip\n    surface: Authentication endpoints\n    limit: 5 requests/minute\n  - scope: user\n    surface: Token refresh\n    limit: 10 requests/hour\nbest_practices_published:\n  - Never expose API keys in client-side code\n  - Use environment variables for key storage (the Python\
  \ SDK reads SEGMIND_API_KEY)\n  - Rotate API keys periodically\n  - Implement retry logic with exponential backoff\n  - Watch Cost Analytics, which can filter by API key and break spend down per key\ngaps:\n  - >-\n    No per-key scoping is exposed to users. The key-creation example accepts a scopes\n    array, but no scope reference is published and the console UI is not documented as\n    offering it.\n  - >-\n    No OIDC discovery, no JWKS endpoint, and no published token-introspection or\n    revocation endpoint for the JWT surface.\nmaintainers:\n  - FN: Kin Lane\n    email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/segmind/refs/heads/main/authentication/segmind-authentication.yml
summary_line: apiKey/http/oauth2 · 4 schemes
tags:
- Artificial Intelligence
- Machine-Learning
- Generative AI
- Inference
- Image-Generation
- Video Generation
- Text-to-Image
- Text-to-Video
- Serverless
- GPU
- Workflows
- Fine-Tuning
---
