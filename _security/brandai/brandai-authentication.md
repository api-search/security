---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: probed
name: Brandai Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Brand.ai secures its APIs with oauth2 and openIdConnect across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Brand.ai
provider_slug: brandai
scheme_count: 3
schemes:
- code_challenge_methods:
  - S256
  flows:
  - authorizationUrl: https://app.brand.ai/api/auth/oauth2/authorize
    flow: authorizationCode
    scope_count: 13
    tokenUrl: https://app.brand.ai/api/auth/oauth2/token
  grant_types:
  - authorization_code
  - refresh_token
  name: OAuth2
  sources:
  - https://app.brand.ai/.well-known/oauth-authorization-server
  token_endpoint_auth_methods:
  - none
  - client_secret_basic
  - client_secret_post
  type: oauth2
- acr_values_supported:
  - urn:mace:incommon:iap:bronze
  claims_supported:
  - sub
  - iss
  - aud
  - exp
  - iat
  - sid
  - scope
  - azp
  - email
  - email_verified
  - name
  - picture
  - family_name
  - given_name
  end_session_endpoint: https://app.brand.ai/api/auth/oauth2/end-session
  id_token_signing_alg_values_supported:
  - EdDSA
  issuer: https://app.brand.ai/api/auth
  jwks_uri: https://app.brand.ai/api/auth/jwks
  name: OpenIDConnect
  openIdConnectUrl: https://app.brand.ai/.well-known/openid-configuration
  prompt_values_supported:
  - login
  - consent
  - create
  - select_account
  - none
  sources:
  - https://app.brand.ai/.well-known/openid-configuration
  subject_types_supported:
  - public
  type: openIdConnect
  userinfo_endpoint: https://app.brand.ai/api/auth/oauth2/userinfo
- name: BearerToken
  observed_challenge: 'WWW-Authenticate: Bearer realm="brand-ai-mcp"'
  realm: brand-ai-mcp
  scheme: bearer
  sources:
  - https://app.brand.ai/api/mcp
  type: http
slug: brandai-authentication
source_filename: brandai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: https://app.brand.ai/.well-known/oauth-authorization-server\ndocs: null\nnote: >-\n  Brand.ai publishes no OpenAPI and no developer authentication page, so this profile\n  is built from the provider's own live OAuth 2.0 / OpenID Connect discovery documents\n  on the application host, plus the observed WWW-Authenticate challenge from the MCP\n  endpoint. The identity layer is Clerk (the 401 carries x-clerk-auth-status and\n  x-clerk-auth-reason headers, and the app CSP allow-lists clerk.brand.ai).\nsummary:\n  types: [oauth2, openIdConnect]\n  api_key_in: []\n  oauth2_flows: [authorizationCode]\n  bearer: true\n  dynamic_client_registration: true\n  pkce_required_methods: [S256]\n  identity_provider: Clerk\nschemes:\n- name: OAuth2\n  type: oauth2\n  sources: [https://app.brand.ai/.well-known/oauth-authorization-server]\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://app.brand.ai/api/auth/oauth2/authorize\n\
  \    tokenUrl: https://app.brand.ai/api/auth/oauth2/token\n    scope_count: 13\n  token_endpoint_auth_methods: [none, client_secret_basic, client_secret_post]\n  grant_types: [authorization_code, refresh_token]\n  code_challenge_methods: [S256]\n- name: OpenIDConnect\n  type: openIdConnect\n  sources: [https://app.brand.ai/.well-known/openid-configuration]\n  openIdConnectUrl: https://app.brand.ai/.well-known/openid-configuration\n  issuer: https://app.brand.ai/api/auth\n  userinfo_endpoint: https://app.brand.ai/api/auth/oauth2/userinfo\n  end_session_endpoint: https://app.brand.ai/api/auth/oauth2/end-session\n  jwks_uri: https://app.brand.ai/api/auth/jwks\n  id_token_signing_alg_values_supported: [EdDSA]\n  subject_types_supported: [public]\n  acr_values_supported: [urn:mace:incommon:iap:bronze]\n  prompt_values_supported: [login, consent, create, select_account, none]\n  claims_supported: [sub, iss, aud, exp, iat, sid, scope, azp, email, email_verified,\n    name, picture, family_name,\
  \ given_name]\n- name: BearerToken\n  type: http\n  scheme: bearer\n  sources: [https://app.brand.ai/api/mcp]\n  realm: brand-ai-mcp\n  observed_challenge: 'WWW-Authenticate: Bearer realm=\"brand-ai-mcp\"'\nendpoints:\n  authorization: https://app.brand.ai/api/auth/oauth2/authorize\n  token: https://app.brand.ai/api/auth/oauth2/token\n  registration: https://app.brand.ai/api/auth/oauth2/register\n  introspection: https://app.brand.ai/api/auth/oauth2/introspect\n  revocation: https://app.brand.ai/api/auth/oauth2/revoke\n  userinfo: https://app.brand.ai/api/auth/oauth2/userinfo\n  jwks: https://app.brand.ai/api/auth/jwks\n  end_session: https://app.brand.ai/api/auth/oauth2/end-session\nposture:\n  strengths:\n  - Open Dynamic Client Registration (RFC 7591) — an MCP client can self-register\n    with no human onboarding step, which is what makes the server agent-reachable.\n  - PKCE S256 is the only code challenge method offered.\n  - EdDSA (Ed25519) ID token signing, ahead of the RS256 default.\n\
  \  - Token introspection (RFC 7662) and revocation (RFC 7009) both published.\n  - authorization_response_iss_parameter_supported (RFC 9207) — mix-up defence.\n  weaknesses:\n  - No RFC 9728 protected-resource metadata, and the 401 challenge omits the\n    resource_metadata parameter, so the AS is not discoverable from the resource.\n  - token_endpoint_auth_methods_supported includes \"none\" (public clients).\n  - No documentation of any of this on a developer-facing page.\nx-evidence:\n- url: https://app.brand.ai/.well-known/oauth-authorization-server\n  http_status: 200\n  fetched: '2026-08-13'\n- url: https://app.brand.ai/.well-known/openid-configuration\n  http_status: 200\n  fetched: '2026-08-13'\n- url: https://app.brand.ai/api/auth/jwks\n  http_status: 200\n  fetched: '2026-08-13'\n- url: https://app.brand.ai/api/mcp\n  http_status: 401\n  fetched: '2026-08-13'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/brandai/refs/heads/main/authentication/brandai-authentication.yml
summary_line: oauth2/openIdConnect · 3 schemes
tags:
- Company
- Brand Management
- Artificial Intelligence
- Marketing
- SaaS
- Brand Operating System
- AI Agents
- Design
- Model Context Protocol
- Brand Governance
- Brand Intelligence
---
