---
api_key_in: []
api_specs:
- filename: rhino-partner-api-openapi.json
  format: json
  label: SayRhino Partner API
  slug: sayrhino-partner-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rhino/refs/heads/main/openapi/rhino-partner-api-openapi.json
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Rhino Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Rhino secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Rhino
provider_slug: rhino
scheme_count: 2
schemes:
- applied: global
  bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/rhino-partner-api-openapi.json
  type: http
- flow: clientCredentials
  name: partnerTokenEndpoint
  request:
    audience: API identifier provided during partner onboarding
    content_type: application/json
    grant_type: client_credentials
    required:
    - client_id
    - client_secret
    - grant_type
    - audience
  response:
    access_token: string
    expires_in: integer (token lifetime in seconds)
    scope: string
    token_type: Bearer
  security: []
  sources:
  - openapi/rhino-partner-api-openapi.json#/paths/~1token/post
  token_url: https://api.prod.sayrhino.com/token
  type: oauth2
slug: rhino-authentication
source_filename: rhino-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: searched\nsource: openapi/rhino-partner-api-openapi.json\ndocs: https://api.prod.sayrhino.com/docs\nsummary:\n  types:\n  - http\n  - oauth2\n  api_key_in: []\n  oauth2_flows:\n  - clientCredentials\n  notes: >-\n    The OpenAPI declares a single securityScheme (http bearer, JWT) applied globally,\n    but the token is minted by a first-class OAuth 2.0 client-credentials endpoint\n    documented in the same spec (POST /token). The spec does not model that endpoint\n    as an oauth2 securityScheme, so the mechanical derive saw only the bearer half —\n    this file records both halves of the real contract.\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  applied: global\n  sources:\n  - openapi/rhino-partner-api-openapi.json\n- name: partnerTokenEndpoint\n  type: oauth2\n  flow: clientCredentials\n  token_url: https://api.prod.sayrhino.com/token\n  security: []\n  request:\n    content_type: application/json\n\
  \    grant_type: client_credentials\n    required:\n    - client_id\n    - client_secret\n    - grant_type\n    - audience\n    audience: API identifier provided during partner onboarding\n  response:\n    access_token: string\n    token_type: Bearer\n    expires_in: integer (token lifetime in seconds)\n    scope: string\n  sources:\n  - openapi/rhino-partner-api-openapi.json#/paths/~1token/post\nonboarding:\n  self_service: false\n  notes: >-\n    Credentials (client_id, client_secret, audience, and the partner owner_slug that\n    appears in every resource path) are issued by Rhino during partner onboarding via a\n    Partner Success representative. There is no public developer sign-up for the\n    Partner API.\n  portal: https://portal.sayrhino.com/users/sign_in\nobserved:\n- request: POST https://api.prod.sayrhino.com/token (empty body, unauthenticated)\n  http_status: 401\n  body: '{\"error\":\"access_denied\",\"error_description\":\"Unauthorized\"}'\n- request: GET https://api.prod.sayrhino.com/partners/{owner_slug}/prospects/{source}/{id}\n\
  \    (unauthenticated)\n  http_status: 401\n  body: '{\"message\":\"Unauthorized\"}'\nx-evidence:\n  fetched: '2026-08-02'\n  url: https://api.prod.sayrhino.com/openapi.json\n  http_status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rhino/refs/heads/main/authentication/rhino-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Insurance
- Insurtech
- Real Estate
- Property Management
- Rentals
- Security Deposits
- Renters Insurance
- Webhooks
- Partner API
---
