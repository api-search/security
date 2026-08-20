---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Bluma Authentication
name_suffix: Authentication
oauth_flows: []
overview: Bluma declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: Bluma
provider_slug: bluma
scheme_count: 3
schemes:
- applies_to: REST API (https://api.getbluma.com/api/v1)
  failure_modes:
  - cause: Missing API key
    status: 401
    title: Authentication Required
    type: authentication_error
  - cause: Key is invalid or revoked; response metadata echoes the key_prefix
    status: 401
    title: Invalid API Key
    type: authentication_error
  - cause: Key lacks the required scope; response metadata names required_scope and available_scopes
    status: 403
    title: Insufficient Permissions
    type: permission_denied
  format: Bearer <api_key>
  header: Authorization
  id: api_key_bearer
  issuance:
  - channel: dashboard
    note: Create API Key; the secret is displayed exactly once.
    url: https://app.getbluma.com/settings?tab=api
  - channel: api
    note: Requires an existing session token, not an API key. Accepts name, environment (test|production) and rate_limit_per_hour.
    operation: POST /api/v1/api-keys
  key_prefixes:
  - behavior: Watermarked, lower-quality (720p max, 24fps) renders; consumes no credits; unlimited keys; same rate limit as the account tier.
    environment: test
    prefix: bluma_test_
  - behavior: Full-quality renders up to 4K, no watermark, credits charged, priority processing.
    environment: production
    prefix: bluma_live_
  listing:
    behavior: Returns keys with a truncated prefix; never re-exposes the full secret.
    operation: GET /api/v1/api-keys
    supported: true
  revocation:
    behavior: Immediate; all requests using that key stop.
    operation: DELETE /api/v1/api-keys/{id}
    supported: true
  rotation:
    behavior: Issues a new key and schedules the old key to expire in 30 days, enabling zero-downtime rotation.
    operation: POST /api/v1/api-keys/{id}/rotate
    recommended_interval: 90 days
    supported: true
  scheme: bearer
  scoped: true
  scopes_source: scopes/bluma-scopes.yml
  type: http
- applies_to: MCP server (https://api.getbluma.com/api/mcp)
  discovery:
  - spec: RFC 9728 Protected Resource Metadata
    status: 200
    url: https://api.getbluma.com/.well-known/oauth-protected-resource
  - spec: RFC 8414 Authorization Server Metadata
    status: 200
    url: https://clerk.getbluma.com/.well-known/oauth-authorization-server
  - spec: OpenID Connect Discovery 1.0
    status: 200
    url: https://clerk.getbluma.com/.well-known/openid-configuration
  documented_in_provider_docs: false
  dynamic_client_registration:
    endpoint: https://clerk.getbluma.com/oauth/register
    supported: true
  flows:
    authorizationCode:
      authorizationUrl: https://clerk.getbluma.com/oauth/authorize
      refreshUrl: https://clerk.getbluma.com/oauth/token
      scopes:
        email: Access the user's email address
        offline_access: Issue a refresh token for long-lived agent sessions
        profile: Access the user's basic profile
      tokenUrl: https://clerk.getbluma.com/oauth/token
  id: oauth2_clerk
  id_token_signing_alg_values_supported:
  - RS256
  identity_provider: Clerk
  issuer: https://clerk.getbluma.com
  jwks_uri: https://clerk.getbluma.com/.well-known/jwks.json
  pkce_required_methods:
  - S256
  revocation_endpoint: https://clerk.getbluma.com/oauth/token/revoke
  token_endpoint_auth_methods_supported:
  - client_secret_basic
  - client_secret_post
  - none
  type: oauth2
- applies_to: API key management operations (POST/GET/DELETE /api/v1/api-keys)
  documented_issuance: false
  id: session_token
  note: The docs show these operations authenticated with "YOUR_SESSION_TOKEN" rather than an API key, implying a dashboard session credential. The docs never define how a session token is obtained outside the dashboard, which makes fully programmatic key provisioning undocumented.
  scheme: bearer
  type: http
slug: bluma-authentication
source_filename: bluma-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: searched\nsource: >-\n  https://docs.getbluma.com/authentication ,\n  https://docs.getbluma.com/api-reference/overview ,\n  https://api.getbluma.com/.well-known/oauth-protected-resource ,\n  https://clerk.getbluma.com/.well-known/oauth-authorization-server\ndocs: https://docs.getbluma.com/authentication\nnote: >-\n  Bluma runs two independent authentication models against the same API host. The REST\n  API at /api/v1 uses long-lived prefixed API keys presented as HTTP bearer tokens; the\n  MCP server at /api/mcp uses OAuth 2.1 delegated to Clerk. There is no published\n  OpenAPI securitySchemes block to derive from — the advertised spec at\n  /api/v1/openapi.json returns 401 — so this profile is read from the documentation and\n  from live anonymous metadata probes.\nschemes:\n- id: api_key_bearer\n  type: http\n  scheme: bearer\n  applies_to: REST API (https://api.getbluma.com/api/v1)\n  header: Authorization\n  format: 'Bearer <api_key>'\n\
  \  key_prefixes:\n  - prefix: bluma_test_\n    environment: test\n    behavior: >-\n      Watermarked, lower-quality (720p max, 24fps) renders; consumes no credits;\n      unlimited keys; same rate limit as the account tier.\n  - prefix: bluma_live_\n    environment: production\n    behavior: Full-quality renders up to 4K, no watermark, credits charged, priority processing.\n  scoped: true\n  scopes_source: scopes/bluma-scopes.yml\n  issuance:\n  - channel: dashboard\n    url: https://app.getbluma.com/settings?tab=api\n    note: Create API Key; the secret is displayed exactly once.\n  - channel: api\n    operation: POST /api/v1/api-keys\n    note: >-\n      Requires an existing session token, not an API key. Accepts name, environment\n      (test|production) and rate_limit_per_hour.\n  rotation:\n    supported: true\n    operation: POST /api/v1/api-keys/{id}/rotate\n    behavior: >-\n      Issues a new key and schedules the old key to expire in 30 days, enabling\n      zero-downtime rotation.\n\
  \    recommended_interval: 90 days\n  revocation:\n    supported: true\n    operation: DELETE /api/v1/api-keys/{id}\n    behavior: Immediate; all requests using that key stop.\n  listing:\n    supported: true\n    operation: GET /api/v1/api-keys\n    behavior: Returns keys with a truncated prefix; never re-exposes the full secret.\n  failure_modes:\n  - status: 401\n    type: authentication_error\n    title: Authentication Required\n    cause: Missing API key\n  - status: 401\n    type: authentication_error\n    title: Invalid API Key\n    cause: Key is invalid or revoked; response metadata echoes the key_prefix\n  - status: 403\n    type: permission_denied\n    title: Insufficient Permissions\n    cause: >-\n      Key lacks the required scope; response metadata names required_scope and\n      available_scopes\n- id: oauth2_clerk\n  type: oauth2\n  applies_to: MCP server (https://api.getbluma.com/api/mcp)\n  flows:\n    authorizationCode:\n      authorizationUrl: https://clerk.getbluma.com/oauth/authorize\n\
  \      tokenUrl: https://clerk.getbluma.com/oauth/token\n      refreshUrl: https://clerk.getbluma.com/oauth/token\n      scopes:\n        email: Access the user's email address\n        profile: Access the user's basic profile\n        offline_access: Issue a refresh token for long-lived agent sessions\n  issuer: https://clerk.getbluma.com\n  identity_provider: Clerk\n  pkce_required_methods:\n  - S256\n  dynamic_client_registration:\n    supported: true\n    endpoint: https://clerk.getbluma.com/oauth/register\n  revocation_endpoint: https://clerk.getbluma.com/oauth/token/revoke\n  jwks_uri: https://clerk.getbluma.com/.well-known/jwks.json\n  id_token_signing_alg_values_supported:\n  - RS256\n  token_endpoint_auth_methods_supported:\n  - client_secret_basic\n  - client_secret_post\n  - none\n  discovery:\n  - spec: RFC 9728 Protected Resource Metadata\n    url: https://api.getbluma.com/.well-known/oauth-protected-resource\n    status: 200\n  - spec: RFC 8414 Authorization Server Metadata\n\
  \    url: https://clerk.getbluma.com/.well-known/oauth-authorization-server\n    status: 200\n  - spec: OpenID Connect Discovery 1.0\n    url: https://clerk.getbluma.com/.well-known/openid-configuration\n    status: 200\n  documented_in_provider_docs: false\n- id: session_token\n  type: http\n  scheme: bearer\n  applies_to: API key management operations (POST/GET/DELETE /api/v1/api-keys)\n  note: >-\n    The docs show these operations authenticated with \"YOUR_SESSION_TOKEN\" rather than an\n    API key, implying a dashboard session credential. The docs never define how a session\n    token is obtained outside the dashboard, which makes fully programmatic key\n    provisioning undocumented.\n  documented_issuance: false\nwebhook_authentication:\n  direction: inbound-to-consumer\n  scheme: HMAC-SHA256\n  header: X-Bluma-Signature\n  format: 'sha256=<hex digest>'\n  signed_payload: raw request body\n  secret_issuance: >-\n    Returned once in the POST /api/v1/webhooks response as a whsec_-prefixed\
  \ secret.\n  helper: Bluma.webhooks.verify() in both the TypeScript and Python SDKs\n  additional_headers:\n  - X-Bluma-Event-Id\n  - X-Bluma-Event-Type\n  - 'User-Agent: Bluma-Webhooks/1.0'\ntransport_security:\n  https_required: true\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_preload: true\ngaps:\n- No mTLS, no openIdConnect scheme on the REST surface, no short-lived token exchange —\n  the REST API is long-lived-static-secret only.\n- The OAuth scopes exposed to MCP clients are identity scopes (email, profile,\n  offline_access) and do not correspond to the REST product scopes, so what an MCP token\n  is authorized to do inside Bluma is not stated anywhere public.\n- Session-token issuance is referenced but never documented, so API key lifecycle cannot\n  be fully automated from the published material.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bluma/refs/heads/main/authentication/bluma-authentication.yml
summary_line: 3 schemes
tags:
- Company
- Artificial Intelligence
- Video
- Video Generation
- Advertising
- Marketing
- Content Creation
- Short-Form Video
- Social-Media
- Generative AI
- Creative Tools
- Text-to-Speech
- Media
- Automation
- Webhook
---
