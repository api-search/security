---
api_key_in: []
auth_types:
- http
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Keel Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- refreshToken
- password
overview: Keel secures its APIs with http, oauth2, and openIdConnect across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, refreshToken, and password flow(s).
provider_name: Keel
provider_slug: keel
scheme_count: 2
schemes:
- bearerFormat: JWT
  description: 'Access tokens are sent as `Authorization: Bearer <access_token>`. Access tokens are short-lived (default expires_in 86400s); refresh via POST /auth/token grant_type=refresh_token (default refresh token lifetime 3 months, rotated on each use).'
  name: bearerAuth
  scheme: bearer
  source: https://docs.keel.so/authentication/tokens
  type: http
- description: OIDC-based Single Sign-On providers configured per project; PKCE-protected authorization code flow, plus ID-token exchange for pre-authenticated clients.
  name: oidcSso
  source: https://docs.keel.so/authentication/providers
  type: openIdConnect
slug: keel-authentication
source_filename: keel-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://docs.keel.so/authentication/tokens + https://docs.keel.so/authentication/providers\ndocs: https://docs.keel.so/authentication/getting-started\nnotes: >-\n  Keel generates authentication for each project. End-user/API access uses short-lived\n  bearer access tokens (JWT, RS256) obtained from the project's /auth/token endpoint, with\n  long-lived refresh tokens and refresh-token rotation on by default. Identity is OIDC-based:\n  Keel supports Single Sign-On (SSO) providers, ID-token exchange, and password flows, with\n  PKCE in the SSO/authorization-code flow. Permissions are enforced via a role-based\n  permissions model declared in the Keel schema (see conventions + docs/permissions).\nsummary:\n  types: [http, oauth2, openIdConnect]\n  api_key_in: []\n  token_format: JWT (RS256)\n  oauth2_flows: [authorizationCode, refreshToken, password]\n  refresh_token_rotation: true\n  pkce: true\nschemes:\n- name: bearerAuth\n\
  \  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: >-\n    Access tokens are sent as `Authorization: Bearer <access_token>`. Access tokens are\n    short-lived (default expires_in 86400s); refresh via POST /auth/token grant_type=refresh_token\n    (default refresh token lifetime 3 months, rotated on each use).\n  source: https://docs.keel.so/authentication/tokens\n- name: oidcSso\n  type: openIdConnect\n  description: >-\n    OIDC-based Single Sign-On providers configured per project; PKCE-protected authorization\n    code flow, plus ID-token exchange for pre-authenticated clients.\n  source: https://docs.keel.so/authentication/providers\nendpoints:\n  token: /auth/token\n  token_response_fields: [access_token, token_type, expires_in, refresh_token, identity_created]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/keel/refs/heads/main/authentication/keel-authentication.yml
summary_line: http/oauth2/openIdConnect · 2 schemes
tags:
- Company
- Operations
- ERP
- Backend
- GraphQL
- API
- Low-Code
- Developer Tools
- Workflow
- Authentication
- TypeScript
---
