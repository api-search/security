---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: probed
name: Pimento Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Pimento secures its APIs with oauth2 and openIdConnect across 0 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Pimento
provider_slug: pimento
scheme_count: 0
schemes: []
slug: pimento-authentication
source_filename: pimento-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: https://gopimento.eu.auth0.com/.well-known/openid-configuration\nx-pointer-suppressed:\n  type: Authentication\n  why: >-\n    No apis.yml `Authentication` pointer is emitted for this file, and a later round\n    should not add one without new evidence. The discovery document is real and\n    anonymous, but it is (a) served from auth0.com rather than a Pimento-controlled\n    domain and (b) auto-generated Auth0 tenant boilerplate for the product login — it\n    is not authentication documentation Pimento wrote for an API, because Pimento\n    publishes no API for developers. Emitting the pointer would credit the\n    `authentication_documented` / `auth_clarity` checks for a developer-facing auth\n    contract that does not exist. This artifact is a record of what was probed, not a\n    claim of published developer auth.\nsummary:\n  public_api: false\n  types: [oauth2, openIdConnect]\n  oauth2_flows: [authorizationCode]\n  pkce:\
  \ true\n  audience: https://api.gopimento.co\n  note: >-\n    Applies to Pimento's own first-party web application only. There is no public API\n    program, no developer key issuance, and no published authentication guide.\nidentity_provider:\n  vendor: Auth0\n  tenant: gopimento.eu.auth0.com\n  region: eu\n  issuer: https://gopimento.eu.auth0.com/\n  discovered_from: >-\n    the app.pimento.design JavaScript bundle (assets/index-DeJG39iw.js), which\n    configures the Auth0 SPA SDK with domain gopimento.eu.auth0.com (prod),\n    redirectUri https://app.pimento.design/ and audience https://api.gopimento.co\nendpoints:\n  authorization: https://gopimento.eu.auth0.com/authorize\n  token: https://gopimento.eu.auth0.com/oauth/token\n  device_authorization: https://gopimento.eu.auth0.com/oauth/device/code\n  userinfo: https://gopimento.eu.auth0.com/userinfo\n  revocation: https://gopimento.eu.auth0.com/oauth/revoke\n  registration: https://gopimento.eu.auth0.com/oidc/register\n  jwks_uri:\
  \ https://gopimento.eu.auth0.com/.well-known/jwks.json\ncapabilities:\n  code_challenge_methods_supported: [S256, plain]\n  response_types_supported: [code, token, id_token, code token, code id_token, token id_token, code token id_token]\n  token_endpoint_auth_methods_supported: [client_secret_basic, client_secret_post, private_key_jwt, none]\n  scopes_supported:\n  - openid\n  - profile\n  - offline_access\n  - name\n  - given_name\n  - family_name\n  - nickname\n  - email\n  - email_verified\n  - picture\n  - created_at\n  - identities\n  - phone\n  - address\n  note: >-\n    These are Auth0's default OIDC scopes for the tenant. No API-specific\n    (audience-scoped) permissions are published, so no scopes/ artifact is written.\nprotected_resource:\n  audience: https://api.gopimento.co\n  resolves_publicly: false\n  dns: NXDOMAIN as of 2026-08-12\n  note: >-\n    `https://api.gopimento.co` is the Auth0 API audience identifier, not a reachable\n    host — it does not resolve in public\
  \ DNS. The API it identifies is served\n    same-origin at https://app.pimento.design/api/*.\nobserved_challenge:\n  url: https://app.pimento.design/api/users/me\n  method: GET\n  http_status: 401\n  content_type: application/json\n  body: '{\"detail\":\"Unable to authenticate\"}'\n  note: >-\n    Confirms a live, credentialed API behind the application. Unrouted paths under\n    /api/ fall through to the SPA shell with a 200, so the 401 is the positive signal.\nraw:\n  file: ../well-known/pimento-auth0-openid-configuration.json\nx-evidence:\n- {url: 'https://gopimento.eu.auth0.com/.well-known/openid-configuration', http_status: 200, content_type: application/json, fetched: '2026-08-12'}\n- {url: 'https://gopimento.eu.auth0.com/.well-known/oauth-authorization-server', http_status: 200, content_type: application/json, fetched: '2026-08-12'}\n- {url: 'https://app.pimento.design/api/users/me', http_status: 401, content_type: application/json, fetched: '2026-08-12'}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pimento/refs/heads/main/authentication/pimento-authentication.yml
summary_line: oauth2/openIdConnect · 0 schemes
tags:
- Company
- Ai/Ml
- Advertising
- Creative
- Marketing
- Generative AI
- AdTech
---
