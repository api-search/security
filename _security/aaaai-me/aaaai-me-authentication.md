---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: aaaai-me-openapi.json
  format: json
  label: AAAAI Platform API
  slug: aaaai-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aaaai-me/refs/heads/main/openapi/aaaai-me-openapi.json
auth_types:
- apiKey
- cookie
description: ''
kind: authentication
layout: security
mechanism_count: 4
method: searched
name: Aaaai Me Authentication
name_suffix: Authentication
oauth_flows: []
overview: AAA AI secures its APIs with apiKey and cookie across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: AAA AI
provider_slug: aaaai-me
scheme_count: 4
schemes:
- evidence: GET https://web.aaaai.me/api/status without credentials -> 401 {"message":"Authentication required. Please login or provide X-User-Login header.","status":"error"}; no WWW-Authenticate header.
  how_to_obtain: 'auth.md: "Programmatic clients should use API keys configured in the product (Settings -> API keys)". Key format is not published.'
  in: header
  name: ApiKeyAuth
  parameter: X-User-Login
  sources:
  - openapi/aaaai-me-openapi.json
  type: apiKey
- evidence: 'GET https://web.aaaai.me/ sets "session=...; Expires=+30 days; HttpOnly; Path=/; SameSite=Lax". auth.md: "After authentication, the platform issues a session cookie for browser clients."'
  in: cookie
  name: session cookie
  obtained_via:
  - POST /api/auth/login {login, password} (bare POST -> 400 "Login and password required")
  - POST /api/auth/apple {identity_token, authorization_code, email} (Sign in with Apple)
  - Google sign-in on https://web.aaaai.me/ (auth.md; no API route in the contract)
  parameter: session
  revoked_via: POST /api/auth/logout (also named revocation_endpoint in the OAuth metadata)
  sources:
  - https://aaaai.me/auth.md
  type: cookie
- evidence: Named only in that operation's summary; not declared as a parameter or securityDefinition. Identifies a paired device agent (see GET /api/nodes). Format and issuance not published.
  in: header
  name: X-Agent-Token
  parameter: X-Agent-Token
  sources:
  - 'openapi/aaaai-me-openapi.json#POST /api/approvals (summary: "Create approval (agent when destructive + no TTY). Header: X-Agent-Token.")'
  type: apiKey
- authorizationUrl: https://web.aaaai.me/
  evidence: Metadata is served from aaaai.me (200) but the issuer host returns 404 for /.well-known/oauth-authorization-server, /.well-known/openid-configuration and the declared jwks_uri; the token endpoint is the password-login route. Recorded for completeness; see scopes/ and conformance/ for the RFC 8414 / OIDC Discovery / RFC 9728 verdicts.
  issuer: https://web.aaaai.me
  name: OAuth 2.0 / OpenID Connect (advertised)
  scopes:
  - openid
  - profile
  - email
  - api
  - offline_access
  sources:
  - well-known/aaaai-me-oauth-authorization-server.json
  - well-known/aaaai-me-openid-configuration.json
  - well-known/aaaai-me-oauth-protected-resource.json
  status: advertised-not-verified
  tokenUrl: https://web.aaaai.me/api/auth/login
  type: oauth2
slug: aaaai-me-authentication
source_filename: aaaai-me-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: searched\nsource: openapi/aaaai-me-openapi.json\ndocs: https://aaaai.me/auth.md\nsummary:\n  types:\n  - apiKey\n  - cookie\n  api_key_in:\n  - header\n  oauth2_flows: []\n  note: >-\n    The contract declares ONE scheme, ApiKeyAuth (apiKey, header X-User-Login), and applies it to no\n    operation, so the derived profile is thin; the rest is from https://aaaai.me/auth.md, the live 401\n    text, response headers observed 2026-09-19 and the OAuth/OIDC discovery documents on aaaai.me.\n    OAuth is advertised in metadata only (scopes/aaaai-me-scopes.yml): the issuer host web.aaaai.me\n    serves no discovery document and no JWKS, so oauth2 is not listed as a working type here.\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-User-Login\n  sources:\n  - openapi/aaaai-me-openapi.json\n  evidence: >-\n    GET https://web.aaaai.me/api/status without credentials -> 401 {\"message\":\"Authentication required.\n    Please\
  \ login or provide X-User-Login header.\",\"status\":\"error\"}; no WWW-Authenticate header.\n  how_to_obtain: 'auth.md: \"Programmatic clients should use API keys configured in the product (Settings -> API keys)\". Key format is not published.'\n- name: session cookie\n  type: cookie\n  in: cookie\n  parameter: session\n  sources:\n  - https://aaaai.me/auth.md\n  evidence: >-\n    GET https://web.aaaai.me/ sets \"session=...; Expires=+30 days; HttpOnly; Path=/; SameSite=Lax\".\n    auth.md: \"After authentication, the platform issues a session cookie for browser clients.\"\n  obtained_via:\n  - 'POST /api/auth/login {login, password} (bare POST -> 400 \"Login and password required\")'\n  - 'POST /api/auth/apple {identity_token, authorization_code, email} (Sign in with Apple)'\n  - 'Google sign-in on https://web.aaaai.me/ (auth.md; no API route in the contract)'\n  revoked_via: POST /api/auth/logout (also named revocation_endpoint in the OAuth metadata)\n- name: X-Agent-Token\n  type:\
  \ apiKey\n  in: header\n  parameter: X-Agent-Token\n  sources:\n  - 'openapi/aaaai-me-openapi.json#POST /api/approvals (summary: \"Create approval (agent when destructive + no TTY). Header: X-Agent-Token.\")'\n  evidence: Named only in that operation's summary; not declared as a parameter or securityDefinition. Identifies a paired device agent (see GET /api/nodes). Format and issuance not published.\n- name: OAuth 2.0 / OpenID Connect (advertised)\n  type: oauth2\n  status: advertised-not-verified\n  sources:\n  - well-known/aaaai-me-oauth-authorization-server.json\n  - well-known/aaaai-me-openid-configuration.json\n  - well-known/aaaai-me-oauth-protected-resource.json\n  issuer: https://web.aaaai.me\n  authorizationUrl: https://web.aaaai.me/\n  tokenUrl: https://web.aaaai.me/api/auth/login\n  scopes: [openid, profile, email, api, offline_access]\n  evidence: >-\n    Metadata is served from aaaai.me (200) but the issuer host returns 404 for\n    /.well-known/oauth-authorization-server,\
  \ /.well-known/openid-configuration and the declared\n    jwks_uri; the token endpoint is the password-login route. Recorded for completeness; see\n    scopes/ and conformance/ for the RFC 8414 / OIDC Discovery / RFC 9728 verdicts.\naccount_security:\n  two_factor: 'docs.html s9 Security: \"Enable two-factor authentication (2FA) ... Scan a QR code with your authenticator app and save backup codes. View connected devices and active sessions.\"'\nanonymous_routes_observed:\n- GET /api/health\n- GET /api/billing/crypto/config\n- GET /api/billing/yookassa/config\n- GET /api/mcp/marketplace\nsubscription_gate:\n  status: 403\n  field: subscribe_url\n  source: https://aaaai.me/.well-known/agent-payments.json#access_gate\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aaaai-me/refs/heads/main/authentication/aaaai-me-authentication.yml
summary_line: apiKey/cookie · 4 schemes
tags:
- Artificial Intelligence
- Agents
- Multi-Agent
- LLM Orchestration
- Meetings
- Voice
- Video
- Workflows
- MCP
- Agentic Commerce
- OpenAI-Compatible
- Self-Hosted
- agent-native
- Montenegro
---
