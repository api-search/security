---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: probed
name: Reflexivity Authentication
name_suffix: Authentication
oauth_flows: []
overview: Reflexivity declares 4 security scheme(s) across its OpenAPI definitions.
provider_name: Reflexivity
provider_slug: reflexivity
scheme_count: 4
schemes:
- client_authentication:
  - client_secret_post
  - client_secret_basic
  - none
  credential_issuance: account id and secret are requested from the Reflexivity back office; no public sign-up for API credentials was found
  expires_in: 86400
  expires_in_note: 24-hour access-token lifetime, stated on the Reflexivity API documentation authentication page
  flow: clientCredentials
  id: oauth2_client_credentials
  scopes_ref: scopes/reflexivity-scopes.yml
  token_type: Bearer
  token_url: https://identity.reflexivity.com/oauth/token
  type: oauth2
- authorization_url: https://identity.reflexivity.com/oauth/authorize
  flow: authorizationCode
  id: oauth2_authorization_code
  pkce:
    code_challenge_methods:
    - S256
    - plain
    note: '`plain` is advertised alongside S256. RFC 7636 §4.2 and OAuth 2.1 both direct clients to use S256 where available; advertising `plain` is a downgrade surface worth flagging to the provider.'
    supported: true
  refresh_supported: true
  token_url: https://identity.reflexivity.com/oauth/token
  type: oauth2
- id: dynamic_client_registration
  note: An open dynamic client registration endpoint is the pattern MCP clients use to self-register. Not probed with a write request — this pipeline does not POST to registration endpoints.
  registration_url: https://identity.reflexivity.com/oauth/register
  spec: RFC 7591
  type: oauth2-registration
- header: Authorization
  id: bearer_http
  note: 'Observed on https://api.reflexivity.com/alfred/v1 — an unauthenticated GET returns HTTP 401 with `authorization: Bearer` and a set of `authorization-is-*` / `authorization-user-*` response headers, confirming a bearer-token gateway in front of every API route.'
  scheme: bearer
  type: http
slug: reflexivity-authentication
source_filename: reflexivity-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: >-\n  https://identity.reflexivity.com/.well-known/oauth-authorization-server (RFC 8414, HTTP 200, anonymous)\n  plus the published Reflexivity API documentation at https://api-docs.tgl.ai/ and observed response\n  headers from https://api.reflexivity.com/alfred/v1 (HTTP 401)\ndocs: https://api-docs.tgl.ai/\nnote: >-\n  Derived from the provider's own authorization-server metadata rather than from an OpenAPI\n  securitySchemes block — Reflexivity publishes no public OpenAPI. The documentation site is\n  password-protected, so the auth model here is reconstructed from three anonymous, verifiable\n  surfaces: the RFC 8414 document, the 401 response headers on the production API host, and the\n  publicly indexed text of the API documentation's authentication page.\nsummary: >-\n  OAuth 2.0. Machine clients use the client_credentials grant with an account id (client_id) and secret\n  issued by Reflexivity, exchanged at the token\
  \ endpoint for a Bearer access token; interactive clients\n  use authorization_code with PKCE. The access token is presented in the HTTP Authorization header as\n  `Bearer <token>`. Credentials are issued by the Reflexivity back office — there is no self-service\n  key provisioning.\nschemes:\n  - id: oauth2_client_credentials\n    type: oauth2\n    flow: clientCredentials\n    token_url: https://identity.reflexivity.com/oauth/token\n    client_authentication:\n      - client_secret_post\n      - client_secret_basic\n      - none\n    token_type: Bearer\n    expires_in: 86400\n    expires_in_note: >-\n      24-hour access-token lifetime, stated on the Reflexivity API documentation authentication page\n    scopes_ref: scopes/reflexivity-scopes.yml\n    credential_issuance: >-\n      account id and secret are requested from the Reflexivity back office; no public sign-up for API\n      credentials was found\n  - id: oauth2_authorization_code\n    type: oauth2\n    flow: authorizationCode\n\
  \    authorization_url: https://identity.reflexivity.com/oauth/authorize\n    token_url: https://identity.reflexivity.com/oauth/token\n    refresh_supported: true\n    pkce:\n      supported: true\n      code_challenge_methods:\n        - S256\n        - plain\n      note: >-\n        `plain` is advertised alongside S256. RFC 7636 §4.2 and OAuth 2.1 both direct clients to use\n        S256 where available; advertising `plain` is a downgrade surface worth flagging to the provider.\n  - id: dynamic_client_registration\n    type: oauth2-registration\n    registration_url: https://identity.reflexivity.com/oauth/register\n    spec: RFC 7591\n    note: >-\n      An open dynamic client registration endpoint is the pattern MCP clients use to self-register.\n      Not probed with a write request — this pipeline does not POST to registration endpoints.\n  - id: bearer_http\n    type: http\n    scheme: bearer\n    header: Authorization\n    note: >-\n      Observed on https://api.reflexivity.com/alfred/v1\
  \ — an unauthenticated GET returns HTTP 401 with\n      `authorization: Bearer` and a set of `authorization-is-*` / `authorization-user-*` response\n      headers, confirming a bearer-token gateway in front of every API route.\nlegacy_environment:\n  note: >-\n    The publicly indexed authentication page names https://auth.dev.rflx.co.uk/oauth/token as the token\n    endpoint. rflx.co.uk is a Reflexivity-controlled domain (identity.rflx.co.uk and\n    identity.staging.rflx.co.uk are both referenced in the reflexivity.com terminal bundle), but `dev`\n    is a non-production environment. The production issuer per the live RFC 8414 document is\n    https://identity.reflexivity.com — that is what is recorded above.\n  probed:\n    - url: https://auth.dev.rflx.co.uk/.well-known/openid-configuration\n      status: 404\noidc:\n  openid_configuration: absent\n  probed:\n    - url: https://identity.reflexivity.com/.well-known/openid-configuration\n      status: 404\n  note: >-\n    OAuth 2.0 authorization-server\
  \ metadata is published; OpenID Connect discovery is not. The\n    authorization server is an OAuth AS, not an OIDC provider, on the public surface.\nmtls: false\napi_keys: false\nx-evidence:\n  - url: https://identity.reflexivity.com/.well-known/oauth-authorization-server\n    status: 200\n  - url: https://api.reflexivity.com/alfred/v1\n    status: 401\n  - url: https://api-docs.tgl.ai/\n    status: 301\n    note: 301 to https://docs.reflexivity.com/ which returns a PASSWORD_PROTECTED interstitial\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/reflexivity/refs/heads/main/authentication/reflexivity-authentication.yml
summary_line: 4 schemes
tags:
- Company
- Financial Services
- Investment Analysis
- Market Data
- Artificial Intelligence
- Machine Learning
- Fintech
- Research
- Knowledge Graph
- Agents
---
