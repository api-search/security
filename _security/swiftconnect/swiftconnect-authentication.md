---
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Swiftconnect Authentication
name_suffix: Authentication
oauth_flows: []
overview: SwiftConnect secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: SwiftConnect
provider_slug: swiftconnect
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: 'Requests carry `Authorization: Bearer <token>`. SwiftConnect''s published curl example uses a bearer token, and an unauthenticated request to a live resource returns HTTP 401 with `{"code":401,"message":"Invalid JWT","client_error_code":""}`, which names the token format as a JWT.'
  in: header
  name: bearerAuth
  parameter: Authorization
  scheme: bearer
  sources:
  - https://swiftconnect.io/developer-api/
  - probe:https://api.swiftconnect.io/credentials
  type: http
slug: swiftconnect-authentication
source_filename: swiftconnect-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-29'\nmethod: searched\nsource: https://swiftconnect.io/developer-api/\ndocs: https://swiftconnect.readme.io/\nnote: >-\n  Derived from SwiftConnect's own published Developer API page (the request examples it prints\n  verbatim) and confirmed against a live unauthenticated request to the API host. There is no public\n  OpenAPI to derive securitySchemes from — the reference lives on a password-protected ReadMe hub —\n  so this profile records only what the provider published in public and what the API itself\n  returned when called without credentials.\nsummary:\n  types:\n  - http\n  http_schemes:\n  - bearer\n  bearer_format: JWT\n  api_key_in: []\n  oauth2_flows: []\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  in: header\n  parameter: Authorization\n  description: >-\n    Requests carry `Authorization: Bearer <token>`. SwiftConnect's published curl example uses a\n    bearer token, and an unauthenticated request\
  \ to a live resource returns HTTP 401 with\n    `{\"code\":401,\"message\":\"Invalid JWT\",\"client_error_code\":\"\"}`, which names the token format as\n    a JWT.\n  sources:\n  - https://swiftconnect.io/developer-api/\n  - probe:https://api.swiftconnect.io/credentials\ntoken_issuance:\n  documented: false\n  note: >-\n    How a JWT is obtained is documented only inside the password-protected developer hub. There is\n    no public OIDC discovery document or OAuth authorization-server metadata on any SwiftConnect\n    host (/.well-known/openid-configuration and /.well-known/oauth-authorization-server both 404 on\n    api.swiftconnect.io; accounts-v2.swiftconnect.io answers 200 with a single-page-app shell for\n    every path, which is not a document).\n  sign_in: https://accounts-v2.swiftconnect.io/\nx-evidence:\n- url: https://api.swiftconnect.io/credentials\n  method: GET\n  http_status: 401\n  body: '{\"code\":401,\"message\":\"Invalid JWT\",\"client_error_code\":\"\"}'\n  fetched:\
  \ '2026-08-29'\n- url: https://swiftconnect.io/developer-api/\n  http_status: 301\n  redirects_to: https://www.swiftconnect.com/developer-api/\n  note: >-\n    The live page now 404s; the request examples above were read from the Internet Archive capture\n    of the provider's own Developer API page.\n  fetched: '2026-08-29'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/swiftconnect/refs/heads/main/authentication/swiftconnect-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Access Control
- Physical Security
- Identity
- Credentials
- Mobile Wallet
- Workplace
- Commercial Real Estate
- Provisioning
- Internet of Things
---
