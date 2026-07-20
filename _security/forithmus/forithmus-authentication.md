---
api_key_in: []
api_specs:
- filename: forithmus-openapi-original.json
  format: json
  label: Forithmus Challenge Platform API
  slug: forithmus-challenge-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/forithmus/refs/heads/main/openapi/forithmus-openapi-original.json
auth_types:
- http-bearer
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Forithmus Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Forithmus secures its APIs with http-bearer, oauth2, and openIdConnect across 4 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Forithmus
provider_slug: forithmus
scheme_count: 4
schemes:
- bearerFormat: JWT
  name: bearerAuth
  obtain: POST /auth/login or POST /auth/google
  refresh: POST /auth/refresh
  revoke: POST /auth/logout
  scheme: bearer
  type: http
- callback: POST /auth/google
  flow: authorizationCode
  name: googleOAuth
  note: Google social sign-in; issues platform JWT access+refresh tokens.
  state: GET /auth/google/state
  type: oauth2
- complete: POST /auth/cli-session/{session_id}/complete
  name: cliDeviceSession
  note: Browser-based device authorization used by the `forithmus login` CLI command.
  poll: GET /auth/cli-session/{session_id}
  start: POST /auth/cli-session
  type: oauth2-device-like
- confirm: POST /auth/2fa/confirm
  mechanism: TOTP
  name: totp2fa
  recovery: POST /auth/2fa/recovery-codes/regenerate
  setup: POST /auth/2fa/setup
  type: mfa
  verify: POST /auth/2fa/verify
slug: forithmus-authentication
source_filename: forithmus-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource:\n- https://research.forithmus.com/api/openapi.json\n- https://research.forithmus.com/getting-started\n- pypi:forithmus (forithmus_cli.auth)\ndocs: https://research.forithmus.com/getting-started\nsummary:\n  types:\n  - http-bearer\n  - oauth2\n  - openIdConnect\n  api_key_in: []\n  oauth2_flows:\n  - authorizationCode\n  mfa:\n  - totp\n  note: The OpenAPI declares no formal securitySchemes; the model below is captured from the live auth\n    endpoints and the first-party CLI.\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  obtain: POST /auth/login or POST /auth/google\n  refresh: POST /auth/refresh\n  revoke: POST /auth/logout\n- name: googleOAuth\n  type: oauth2\n  flow: authorizationCode\n  state: GET /auth/google/state\n  callback: POST /auth/google\n  note: Google social sign-in; issues platform JWT access+refresh tokens.\n- name: cliDeviceSession\n  type: oauth2-device-like\n  start:\
  \ POST /auth/cli-session\n  poll: GET /auth/cli-session/{session_id}\n  complete: POST /auth/cli-session/{session_id}/complete\n  note: Browser-based device authorization used by the `forithmus login` CLI command.\n- name: totp2fa\n  type: mfa\n  mechanism: TOTP\n  setup: POST /auth/2fa/setup\n  confirm: POST /auth/2fa/confirm\n  verify: POST /auth/2fa/verify\n  recovery: POST /auth/2fa/recovery-codes/regenerate\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/forithmus/refs/heads/main/authentication/forithmus-authentication.yml
summary_line: http-bearer/oauth2/openIdConnect · 4 schemes
tags:
- Medical Imaging
- Radiology
- Machine Learning
- Foundation Models
- Healthcare AI
- Challenge Platform
- Benchmarks
- Research
- Developer Tools
- API
---
