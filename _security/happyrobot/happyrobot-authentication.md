---
api_key_in:
- header
api_specs:
- filename: happyrobot-public-api-openapi.json
  format: json
  label: Happyrobot Public API
  slug: happyrobot-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/happyrobot/refs/heads/main/openapi/happyrobot-public-api-openapi.json
- filename: happyrobot-platform-v1-openapi.json
  format: json
  label: Happyrobot Platform API v1
  slug: happyrobot-platform-api-v1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/happyrobot/refs/heads/main/openapi/happyrobot-platform-v1-openapi.json
- filename: happyrobot-public-api-openapi.json
  format: json
  label: Happyrobot Public API (EU cluster)
  slug: happyrobot-public-api-eu-cluster
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/happyrobot/refs/heads/main/openapi/happyrobot-public-api-openapi.json
auth_types:
- http
- apiKey
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Happyrobot Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
- refreshToken
overview: Happyrobot secures its APIs with http, apiKey, oauth2, and openIdConnect across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, clientCredentials, and refreshToken flow(s).
provider_name: Happyrobot
provider_slug: happyrobot
scheme_count: 3
schemes:
- applied_to_operations: 205
  bearerFormat: Opaque
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/happyrobot-public-api-openapi.json
  type: http
- in: header
  name: authorization
  parameter: authorization
  sources:
  - openapi/happyrobot-platform-v1-openapi.json
  type: apiKey
- in: header
  name: x-organization-id
  note: tenant selector, required alongside `authorization` on every v1 operation
  parameter: x-organization-id
  sources:
  - openapi/happyrobot-platform-v1-openapi.json
  type: apiKey
slug: happyrobot-authentication
source_filename: happyrobot-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-01'\nmethod: searched\nsource: openapi/happyrobot-public-api-openapi.json\ndocs: https://docs.happyrobot.ai/api-reference\nnotes: >-\n  Derived from both OpenAPI documents, then upgraded with the three discovery documents probed live on\n  2026-08-01: the Auth0 OIDC configuration on auth.happyrobot.ai, the RFC 8414 OAuth authorization server\n  metadata on platform.happyrobot.ai (MCP), and the RFC 8414 metadata on docs.happyrobot.ai (docs MCP).\n  Happyrobot runs three distinct authentication planes: a bearer API key for machine access to the Public\n  API, an Auth0 OIDC tenant for human sign-in to the console, and OAuth 2.0 authorization servers fronting\n  its two MCP surfaces.\nsummary:\n  types:\n  - http\n  - apiKey\n  - oauth2\n  - openIdConnect\n  api_key_in:\n  - header\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\n  - refreshToken\nplanes:\n- plane: public-api\n  audience: machine / server-to-server\n  mechanism: Bearer API key\n\
  \  header: 'Authorization: Bearer <api_key>'\n  applied: >-\n    every operation in the v2 OpenAPI carries security [{bearerAuth: []}] and there is a matching\n    top-level security requirement, so the scheme is both defined and applied\n  scoping: >-\n    An API key is bound to one organization and one environment. GET /api-key/describe returns the key's\n    id, orgId, org_slug, org_name, name, prefix, lastFour, createdAt, lastUsedAt and revokedAt — so keys\n    carry a visible prefix + last-four for identification and support explicit revocation.\n  introspection_operation: GET /api-key/describe\n  example_prefix_observed: sk_live_\n  example_prefix_source: https://github.com/happyrobot-ai/chatbot-sdk-example\n- plane: legacy-v1\n  audience: machine / server-to-server\n  mechanism: opaque token in an `authorization` header plus an explicit `x-organization-id` header\n  headers:\n  - authorization\n  - x-organization-id\n  applied: >-\n    every one of the ten v1 operations declares\
  \ both headers as required parameters; the v1 document\n    defines no components.securitySchemes, so auth is expressed as bare header parameters\n  source: openapi/happyrobot-platform-v1-openapi.json\n- plane: console-sign-in\n  audience: human\n  mechanism: OpenID Connect (Auth0 tenant)\n  issuer: https://auth.happyrobot.ai/\n  discovery: https://auth.happyrobot.ai/.well-known/openid-configuration\n  observed:\n    authorization_endpoint: https://auth.happyrobot.ai/authorize\n    token_endpoint: https://auth.happyrobot.ai/oauth/token\n    userinfo_endpoint: https://auth.happyrobot.ai/userinfo\n    jwks_uri: https://auth.happyrobot.ai/.well-known/jwks.json\n    registration_endpoint: https://auth.happyrobot.ai/oidc/register\n    end_session_endpoint: https://auth.happyrobot.ai/oidc/logout\n    revocation_endpoint: https://auth.happyrobot.ai/oauth/revoke\n    device_authorization_endpoint: https://auth.happyrobot.ai/oauth/device/code\n    mfa_challenge_endpoint: https://auth.happyrobot.ai/mfa/challenge\n\
  \    backchannel_logout_supported: true\n    id_token_signing_alg_values_supported:\n    - HS256\n    - RS256\n    - PS256\n    code_challenge_methods_supported:\n    - S256\n    - plain\n  client_flow_observed: >-\n    app.happyrobot.ai/login and /signup both 302 to auth.happyrobot.ai/authorize with\n    response_type=code, code_challenge_method=S256 and scope \"openid profile email offline_access\",\n    redirecting back to https://platform.happyrobot.ai/auth/callback — authorization code + PKCE.\n- plane: platform-mcp\n  audience: agent / MCP client\n  mechanism: OAuth 2.0 with dynamic client registration\n  issuer: https://platform.happyrobot.ai\n  discovery: https://platform.happyrobot.ai/.well-known/oauth-authorization-server\n  observed:\n    authorization_endpoint: https://platform.happyrobot.ai/mcp/authorize\n    token_endpoint: https://platform.happyrobot.ai/api/mcp/token\n    registration_endpoint: https://platform.happyrobot.ai/api/mcp/register\n    grant_types_supported:\n\
  \    - authorization_code\n    - refresh_token\n    - client_credentials\n    code_challenge_methods_supported:\n    - S256\n    token_endpoint_auth_methods_supported:\n    - none\n    scopes_supported:\n    - mcp:full\n- plane: docs-mcp\n  audience: agent / MCP client\n  mechanism: OAuth 2.0 with dynamic client registration\n  issuer: https://docs.happyrobot.ai/mcp/oauth\n  discovery: https://docs.happyrobot.ai/.well-known/oauth-authorization-server\n  protected_resource_metadata: https://docs.happyrobot.ai/.well-known/oauth-protected-resource\n  observed:\n    authorization_endpoint: https://docs.happyrobot.ai/mcp/oauth/authorize\n    token_endpoint: https://docs.happyrobot.ai/mcp/oauth/token\n    registration_endpoint: https://docs.happyrobot.ai/mcp/oauth/register\n    grant_types_supported:\n    - authorization_code\n    - client_credentials\n    - refresh_token\n    code_challenge_methods_supported:\n    - S256\n    token_endpoint_auth_methods_supported:\n    - none\n    - client_secret_post\n\
  \    - client_secret_basic\n    scopes_supported:\n    - mcp:search\n  challenge_observed: >-\n    POST tools/list without a token returns HTTP 401 with\n    'WWW-Authenticate: Bearer error=\"invalid_token\", error_description=\"No authorization provided\",\n    resource_metadata=\"https://docs.happyrobot.ai/.well-known/oauth-protected-resource\"' — a correct\n    RFC 9728 challenge.\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: Opaque\n  applied_to_operations: 205\n  sources:\n  - openapi/happyrobot-public-api-openapi.json\n- name: authorization\n  type: apiKey\n  in: header\n  parameter: authorization\n  sources:\n  - openapi/happyrobot-platform-v1-openapi.json\n- name: x-organization-id\n  type: apiKey\n  in: header\n  parameter: x-organization-id\n  note: tenant selector, required alongside `authorization` on every v1 operation\n  sources:\n  - openapi/happyrobot-platform-v1-openapi.json\ndelegated_tokens:\n  note: >-\n    The Public API issues short-lived,\
  \ scoped client tokens so browser code never sees the API key.\n    This two-tier model is documented in Happyrobot's own public SDK examples.\n  operations:\n  - operation: POST /chat/tokens/\n    returns: '{ token, expires_at }'\n    used_by: browser chat clients connecting to POST /chat/sessions/ and the session WebSocket\n  - operation: POST /voice/tokens/\n    returns: '{ url, token, room_name, run_id }'\n    used_by: browser WebRTC voice clients connecting to LiveKit\n  - operation: POST /realtime/tokens\n    returns: realtime session token\n  sources:\n  - https://github.com/happyrobot-ai/chatbot-sdk-example\n  - https://github.com/happyrobot-ai/voice-sdk-example\nx-evidence:\n  fetched: '2026-08-01'\n  probes:\n  - url: https://platform.happyrobot.ai/api/v2/docs/json\n    http_status: 200\n  - url: https://platform.happyrobot.ai/api/v1/openapi.json\n    http_status: 200\n  - url: https://auth.happyrobot.ai/.well-known/openid-configuration\n    http_status: 200\n  - url: https://platform.happyrobot.ai/.well-known/oauth-authorization-server\n\
  \    http_status: 200\n  - url: https://docs.happyrobot.ai/.well-known/oauth-authorization-server\n    http_status: 200\n  - url: https://docs.happyrobot.ai/.well-known/oauth-protected-resource\n    http_status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/happyrobot/refs/heads/main/authentication/happyrobot-authentication.yml
summary_line: http/apiKey/oauth2/openIdConnect · 3 schemes
tags:
- AI Agents
- Agent Orchestration
- Voice AI
- Conversational AI
- Logistics
- Freight
- Supply Chain
- Workflow-Automation
- Contact Center
- Telephony
- MCP
- agent-native
- Agent Governance
- Enterprise Automation
---
