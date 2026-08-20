---
api_key_in:
- header
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Epsilon3 Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Epsilon3 secures its APIs with http and oauth2 across 4 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Epsilon3
provider_slug: epsilon3
scheme_count: 4
schemes:
- applies_to: Epsilon3 REST API (https://api.epsilon3.io/v1)
  description: 'A per-workspace API key is supplied as the USERNAME component of an HTTP Basic Authorization header with an empty password - curl -u "$EPSILON3_API_KEY": - which the docs demonstrate in curl, Python requests and PowerShell. There is no bearer token, no signed request and no separate secret.'
  key_generation: https://support.epsilon3.io/en/articles/8779712-generate-api-key
  key_scoping:
  - note: Team-scoped keys are the default and are REQUIRED for realtime (SocketIO/webhook) client authentication - the docs state user-scoped keys will not work there.
    scope: team
  - note: 'User-scoped API keys were added in Changelog #97 (2026-04-03) and are issued from User > Profile > API Keys. At least one documented endpoint requires a user key and returns 403 for a team key.'
    scope: user
  name: ApiKeyBasic
  scheme: basic
  source: https://docs.epsilon3.io/#authentication
  type: http
- algorithm_published: false
  applies_to: Epsilon3 Realtime API webhooks
  description: Inbound webhook deliveries carry an Epsilon3-Signature header. Epsilon3 ships a python module named webhook_auth exposing verify_webhook_signature(secret, payload, signature) which returns True/False. The signing algorithm is not published; the docs direct integrators to contact Epsilon3 support to verify signatures manually. A webhook key must be registered by Epsilon3 support - it is not self-service.
  header: Epsilon3-Signature
  name: RealtimeWebhookSignature
  secret_env: EPSILON3_WEBHOOK_KEY
  source: https://docs.epsilon3.io/#webhook-signature-verification
  type: signature
- applies_to: Epsilon3 MCP Server (https://mcp.epsilon3.io)
  description: The hosted MCP server is protected by OAuth 2.1 authorization-code with PKCE. Public clients only - token_endpoint_auth_methods_supported is ["none"] - and dynamic client registration (RFC 7591) is open, which is what lets an MCP client self-register as a connector. An Epsilon3 API key may alternatively be presented as a bearer token.
  flows:
  - authorizationUrl: https://app.epsilon3.io/oauth/authorize
    code_challenge_methods_supported:
    - S256
    flow: authorizationCode
    grant_types_supported:
    - authorization_code
    - refresh_token
    registrationUrl: https://app.epsilon3.io/oauth/register
    response_types_supported:
    - code
    scope_count: 15
    scopes: scopes/epsilon3-scopes.yml
    tokenUrl: https://app.epsilon3.io/oauth/token
    token_endpoint_auth_methods_supported:
    - none
  name: MCPOAuth
  sources:
  - well-known/epsilon3-mcp-oauth-authorization-server.json
  - well-known/epsilon3-mcp-oauth-protected-resource.json
  type: oauth2
- applies_to: api.epsilon3.io and api.uk.epsilon3.io
  description: The API hosts serve their own RFC 8414 authorization-server metadata with the same fifteen scopes, issuer-local endpoints, PKCE S256 and open dynamic client registration. This OAuth surface is NOT documented in the API Guide - the guide only describes API-key Basic auth - so it is recorded here from the served metadata, and an integrator should treat it as undocumented until Epsilon3 publishes it.
  flows:
  - authorizationUrl: https://api.epsilon3.io/oauth/authorize
    code_challenge_methods_supported:
    - S256
    flow: authorizationCode
    registrationUrl: https://api.epsilon3.io/oauth/register
    scope_count: 15
    tokenUrl: https://api.epsilon3.io/oauth/token
  name: PlatformOAuth
  sources:
  - well-known/epsilon3-oauth-authorization-server.json
  type: oauth2
slug: epsilon3-authentication
source_filename: epsilon3-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: searched\nsource: https://docs.epsilon3.io/#authentication\ndocs: https://support.epsilon3.io/en/articles/8779712-generate-api-key\nnote: >-\n  Derived mechanically from OpenAPI was not possible - Epsilon3 publishes no machine\n  readable spec. This profile is transcribed from the published API Guide plus the\n  RFC 8414 / RFC 9728 metadata documents actually served by the API and MCP hosts.\nsummary:\n  types: [http, oauth2]\n  http_schemes: [basic]\n  api_key_in: [header]\n  api_key_transport: HTTP Basic username component\n  oauth2_flows: [authorizationCode]\n  oauth2_surface: MCP server only\nschemes:\n- name: ApiKeyBasic\n  type: http\n  scheme: basic\n  applies_to: Epsilon3 REST API (https://api.epsilon3.io/v1)\n  description: >-\n    A per-workspace API key is supplied as the USERNAME component of an HTTP Basic\n    Authorization header with an empty password - curl -u \"$EPSILON3_API_KEY\": - which\n    the docs demonstrate in curl,\
  \ Python requests and PowerShell. There is no bearer\n    token, no signed request and no separate secret.\n  source: https://docs.epsilon3.io/#authentication\n  key_scoping:\n  - scope: team\n    note: >-\n      Team-scoped keys are the default and are REQUIRED for realtime (SocketIO/webhook)\n      client authentication - the docs state user-scoped keys will not work there.\n  - scope: user\n    note: >-\n      User-scoped API keys were added in Changelog #97 (2026-04-03) and are issued from\n      User > Profile > API Keys. At least one documented endpoint requires a user key\n      and returns 403 for a team key.\n  key_generation: https://support.epsilon3.io/en/articles/8779712-generate-api-key\n- name: RealtimeWebhookSignature\n  type: signature\n  applies_to: Epsilon3 Realtime API webhooks\n  description: >-\n    Inbound webhook deliveries carry an Epsilon3-Signature header. Epsilon3 ships a\n    python module named webhook_auth exposing verify_webhook_signature(secret, payload,\n\
  \    signature) which returns True/False. The signing algorithm is not published; the\n    docs direct integrators to contact Epsilon3 support to verify signatures manually.\n    A webhook key must be registered by Epsilon3 support - it is not self-service.\n  header: Epsilon3-Signature\n  secret_env: EPSILON3_WEBHOOK_KEY\n  algorithm_published: false\n  source: https://docs.epsilon3.io/#webhook-signature-verification\n- name: MCPOAuth\n  type: oauth2\n  applies_to: Epsilon3 MCP Server (https://mcp.epsilon3.io)\n  description: >-\n    The hosted MCP server is protected by OAuth 2.1 authorization-code with PKCE.\n    Public clients only - token_endpoint_auth_methods_supported is [\"none\"] - and\n    dynamic client registration (RFC 7591) is open, which is what lets an MCP client\n    self-register as a connector. An Epsilon3 API key may alternatively be presented\n    as a bearer token.\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://app.epsilon3.io/oauth/authorize\n\
  \    tokenUrl: https://app.epsilon3.io/oauth/token\n    registrationUrl: https://app.epsilon3.io/oauth/register\n    code_challenge_methods_supported: [S256]\n    grant_types_supported: [authorization_code, refresh_token]\n    response_types_supported: [code]\n    token_endpoint_auth_methods_supported: [none]\n    scope_count: 15\n    scopes: scopes/epsilon3-scopes.yml\n  sources:\n  - well-known/epsilon3-mcp-oauth-authorization-server.json\n  - well-known/epsilon3-mcp-oauth-protected-resource.json\n- name: PlatformOAuth\n  type: oauth2\n  applies_to: api.epsilon3.io and api.uk.epsilon3.io\n  description: >-\n    The API hosts serve their own RFC 8414 authorization-server metadata with the same\n    fifteen scopes, issuer-local endpoints, PKCE S256 and open dynamic client\n    registration. This OAuth surface is NOT documented in the API Guide - the guide only\n    describes API-key Basic auth - so it is recorded here from the served metadata, and\n    an integrator should treat it as\
  \ undocumented until Epsilon3 publishes it.\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.epsilon3.io/oauth/authorize\n    tokenUrl: https://api.epsilon3.io/oauth/token\n    registrationUrl: https://api.epsilon3.io/oauth/register\n    code_challenge_methods_supported: [S256]\n    scope_count: 15\n  sources:\n  - well-known/epsilon3-oauth-authorization-server.json\nsso:\n  available: true\n  mechanisms: [SAML, SSO, MFA]\n  tier: Pro and Enterprise plans\n  source: https://www.epsilon3.io/security\ngaps:\n- No OpenID Connect discovery document is served on any host (/.well-known/openid-configuration\n  404s on the docs/www hosts and returns the SPA shell on api/app).\n- The webhook signature algorithm is not published, so signature verification cannot be\n  implemented without contacting support - a real interoperability barrier for any\n  non-Python consumer.\n- The platform-level OAuth surface on api.epsilon3.io is served but undocumented.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/epsilon3/refs/heads/main/authentication/epsilon3-authentication.yml
summary_line: http/oauth2 · 4 schemes
tags:
- Company
- Aerospace
- Space
- Defense
- Manufacturing
- Procedures
- Workflows
- Inventory
- Telemetry
- Test Management
- Project Management
- MCP
---
