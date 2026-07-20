---
api_key_in:
- http-basic
auth_types:
- http-basic
- jwt
- session-token
description: ''
kind: authentication
layout: security
method: searched
name: Cuenca Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cuenca secures its APIs with http-basic, jwt, and session-token across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Cuenca
provider_slug: cuenca
scheme_count: 4
schemes:
- credential_prefix: PK
  description: 'Primary credential: an API key (id prefixed `PK...`) and API secret sent as HTTP Basic auth on every request. Configured via CUENCA_API_KEY / CUENCA_API_SECRET env vars or cuenca.configure(api_key=..., api_secret=...).'
  name: apiKeySecretBasic
  scheme: basic
  type: http
- bearerFormat: JWT
  description: Optional JWT auth (cuenca.configure(use_jwt=True)). A JWT is created from the API key/secret and auto-renewed when under 5 minutes to expiry. Requires sufficient permissions on the credential.
  name: jwt
  scheme: bearer
  type: http
- description: A LoginToken (7-day validity, created via biometric/user login) supplied in the X-Cuenca-LoginToken header for user-scoped sessions.
  in: header
  name: loginToken
  parameterName: X-Cuenca-LoginToken
  type: apiKey
- description: Session identifier supplied in the X-Cuenca-SessionId header.
  in: header
  name: sessionId
  parameterName: X-Cuenca-SessionId
  type: apiKey
slug: cuenca-authentication
source_filename: cuenca-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://github.com/cuenca-mx/cuenca-python (http/client.py, jwt.py, README)\ndocs: https://github.com/cuenca-mx/cuenca-python#authentication\nsummary:\n  types: [http-basic, jwt, session-token]\n  api_key_in: [http-basic]\n  notes: >-\n    Cuenca has no OpenAPI/OAuth2 scope surface. Primary auth is an API key +\n    secret sent as HTTP Basic. Optional short-lived JWTs and login/session\n    tokens layer on top for delegated/user-scoped access.\nschemes:\n- name: apiKeySecretBasic\n  type: http\n  scheme: basic\n  description: >-\n    Primary credential: an API key (id prefixed `PK...`) and API secret sent as\n    HTTP Basic auth on every request. Configured via CUENCA_API_KEY /\n    CUENCA_API_SECRET env vars or cuenca.configure(api_key=..., api_secret=...).\n  credential_prefix: PK\n- name: jwt\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: >-\n    Optional JWT auth (cuenca.configure(use_jwt=True)). A\
  \ JWT is created from the\n    API key/secret and auto-renewed when under 5 minutes to expiry. Requires\n    sufficient permissions on the credential.\n- name: loginToken\n  type: apiKey\n  in: header\n  parameterName: X-Cuenca-LoginToken\n  description: >-\n    A LoginToken (7-day validity, created via biometric/user login) supplied in\n    the X-Cuenca-LoginToken header for user-scoped sessions.\n- name: sessionId\n  type: apiKey\n  in: header\n  parameterName: X-Cuenca-SessionId\n  description: Session identifier supplied in the X-Cuenca-SessionId header.\nheaders:\n  api_version: X-Cuenca-Api-Version\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cuenca/refs/heads/main/authentication/cuenca-authentication.yml
summary_line: http-basic/jwt/session-token · 4 schemes
tags:
- Company
- Fintech
- Payments
- Banking
- Neobank
- SPEI
- Card Issuing
- Money Transfer
- Mexico
- KYC
---
