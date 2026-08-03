---
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
method: probed
name: Shiftsmart Authentication
name_suffix: Authentication
oauth_flows: []
overview: Shiftsmart secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Shiftsmart
provider_slug: shiftsmart
scheme_count: 1
schemes:
- bearerFormat: JWT
  confidence: medium
  endpoint: https://api.shiftsmart.com/authentication
  method: POST
  name: feathersAuthentication
  note: POST /authentication with an empty JSON body returns 401 NotAuthenticated with the message "Invalid authentication information (no `strategy` set)" — the FeathersJS authentication service contract, which issues a JWT access token in exchange for a named strategy (commonly `local` or `jwt`). The exact strategies Shiftsmart enables are not published and were not probed further.
  requires:
  - strategy
  scheme: bearer
  type: http
slug: shiftsmart-authentication
source_filename: shiftsmart-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: probed\nsource: https://api.shiftsmart.com/authentication\nnote: >-\n  Shiftsmart publishes no OpenAPI, so no securitySchemes could be derived. This profile\n  is built entirely from observed live responses at api.shiftsmart.com. Shiftsmart\n  publishes no public authentication documentation; third-party developers cannot\n  self-serve credentials.\nsummary:\n  types:\n  - http\n  documented: false\n  public_signup: false\n  spec_derived: false\n  framework: FeathersJS\nschemes:\n- name: feathersAuthentication\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  endpoint: https://api.shiftsmart.com/authentication\n  method: POST\n  requires:\n  - strategy\n  confidence: medium\n  note: >-\n    POST /authentication with an empty JSON body returns 401 NotAuthenticated with\n    the message \"Invalid authentication information (no `strategy` set)\" — the FeathersJS\n    authentication service contract, which issues a JWT access token in exchange\
  \ for\n    a named strategy (commonly `local` or `jwt`). The exact strategies Shiftsmart\n    enables are not published and were not probed further.\nobservations:\n- path: /authentication\n  method: POST\n  status: 401\n  body: '{\"name\":\"NotAuthenticated\",\"message\":\"Invalid authentication information (no\n    `strategy` set)\",\"code\":401,\"className\":\"not-authenticated\"}'\n- path: /authentication\n  method: GET\n  status: 405\n  body: '{\"name\":\"MethodNotAllowed\",\"message\":\"Method `find` is not supported by this\n    endpoint.\",\"code\":405,\"className\":\"method-not-allowed\"}'\n- path: /shifts\n  method: GET\n  status: 401\n  body: '{\"name\":\"NotAuthenticated\",\"message\":\"Not authenticated\",\"code\":401,\"className\":\"not-authenticated\"}'\n- path: /health\n  method: GET\n  status: 200\n  body: '{\"status\":200}'\n  note: the only unauthenticated endpoint discovered\noauth2: false\nopenid_connect: false\napi_keys_documented: false\nx-evidence:\n  fetched: '2026-08-02'\n\
  \  host: api.shiftsmart.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/shiftsmart/refs/heads/main/authentication/shiftsmart-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Workforce Management
- Staffing
- Scheduling
- Labor Marketplace
- Human Resources
- Gig Economy
- Workforce
- Payments
- Field Services
---
