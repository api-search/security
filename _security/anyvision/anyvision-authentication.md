---
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Anyvision Authentication
name_suffix: Authentication
oauth_flows: []
overview: AnyVision secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: AnyVision
provider_slug: anyvision
scheme_count: 1
schemes:
- applies_to:
  - Oosto OnWatch API
  - Oosto OnAccess API
  bearerFormat: JWT
  description: 'Both products issue a bearer token from a username/password login and expect it on subsequent requests as `Authorization: Bearer <token>`. There is no public OAuth 2.0 authorization server, no scope surface, and no API-key issuance documented publicly — which is why no scopes/ artifact was written for this provider.'
  name: bearerAuth
  scheme: bearer
  sources:
  - https://github.com/AnyVisionltd/oosto-api-sample-code
  type: http
slug: anyvision-authentication
source_filename: anyvision-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-06'\nmethod: searched\nsource: https://github.com/AnyVisionltd/oosto-api-sample-code\ndocs: https://knowledge.oosto.com/docs\ndocs_access: gated\ndocs_note: >-\n  The Oosto knowledge base is the only reference documentation and it 302s to an email one-time-password\n  login (https://knowledge.oosto.com/login/?redirect_to=%2Fdocs). This profile is therefore derived\n  from the vendor's own PUBLIC sample code on GitHub, not from a published OpenAPI — no securityScheme\n  objects exist to aggregate, so derive-authentication.py produced nothing and this file was written\n  by hand from observed, first-party published code.\nsummary:\n  types:\n  - http\n  bearer_format: JWT\n  api_key_in: []\n  oauth2_flows: []\n  oauth2: false\n  openid_connect: false\n  mtls: false\n  mfa: not-documented-publicly\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: >-\n    Both products issue a bearer token from a username/password\
  \ login and expect it on subsequent\n    requests as `Authorization: Bearer <token>`. There is no public OAuth 2.0 authorization server,\n    no scope surface, and no API-key issuance documented publicly — which is why no scopes/ artifact\n    was written for this provider.\n  applies_to:\n  - Oosto OnWatch API\n  - Oosto OnAccess API\n  sources:\n  - https://github.com/AnyVisionltd/oosto-api-sample-code\nflows:\n- api: Oosto OnWatch API\n  base_path: /bt/api\n  steps:\n  - operation: POST /bt/api/login\n    body: '{ \"username\": \"...\", \"password\": \"...\" }'\n    returns: '{ \"token\": \"...\", \"isEulaConfirmed\": true|false }'\n  - operation: POST /bt/api/eula\n    body: '{ \"username\": \"...\", \"password\": \"...\" }'\n    note: >-\n      Required once per user when isEulaConfirmed is false. The login must then be repeated to obtain\n      a usable token. This EULA gate is unusual and worth noting — a first-time integration cannot\n      authenticate until the end-user licence\
  \ has been acknowledged over the API.\n  - operation: Authorization header\n    value: 'Authorization: Bearer <token>'\n  - operation: Socket.IO handshake\n    note: >-\n      The same token is passed as a `token` query parameter on the Socket.IO connection to\n      /bt/api/socket.io rather than in a header.\n- api: Oosto OnAccess API\n  base_path: /abx/api\n  steps:\n  - operation: POST /abx/api/login\n    body: '{ \"username\": \"...\", \"password\": \"...\" }'\n    returns: '{ \"token\": \"...\" }'\n  - operation: Authorization header\n    value: 'Authorization: Bearer <token>'\ntransport_security_warning: >-\n  Every published sample disables TLS verification — the JS samples set\n  `NODE_TLS_REJECT_UNAUTHORIZED = 0` / `rejectUnauthorized: false` and the Python sample passes\n  `verify=False`. The 2.3.1 README acknowledges this: \"Please take notice this not a secure way and\n  it's not recommended to work this way outside the development environment.\" This reflects the\n  on-premise\
  \ deployment model (self-signed certificates on customer servers) and is recorded as an\n  observation about the published sample code, not as a finding about a production deployment.\nx-evidence:\n  fetched: '2026-08-06'\n  urls:\n  - url: https://raw.githubusercontent.com/AnyVisionltd/oosto-api-sample-code/master/OnWatch/2.5.0/js/exmaple-code-login-socket.js\n    status: 200\n  - url: https://raw.githubusercontent.com/AnyVisionltd/oosto-api-sample-code/master/OnWatch/2.5.0/python/example-code-login-socket.py\n    status: 200\n  - url: https://raw.githubusercontent.com/AnyVisionltd/oosto-api-sample-code/master/OnAccess/1.1.0/js/createMember.js\n    status: 200\n  - url: https://knowledge.oosto.com/docs\n    status: 302\n    redirect_to: https://knowledge.oosto.com/login/?redirect_to=%2Fdocs\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/anyvision/refs/heads/main/authentication/anyvision-authentication.yml
summary_line: http · 1 scheme
tags:
- facial-recognition
- computer-vision
- video-analytics
- physical-security
- access-control
- biometrics
- surveillance
- edge-ai
- watchlist-alerting
- visitor-management
- israel
- Company
---
