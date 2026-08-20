---
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Booksy Authentication
name_suffix: Authentication
oauth_flows: []
overview: Booksy secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Booksy
provider_slug: booksy
scheme_count: 2
schemes:
- algorithm: RS256
  description: Before calling the API a partner signs a JWT with its own RSA private key (separate private keys are issued for sandbox and for production). The claim set is iss (https://public-api.booksy.com), iat, exp and aud (the partner UUID); the JOSE header carries typ JWT and alg RS256. The signed assertion is POSTed to {base_url}/token/ together with partner_name.
  name: partnerJwtAssertion
  sources:
  - https://docs.booksy.com/v01.html
  token_endpoint: '{base_url}/token/'
  type: assertion
- bearerFormat: JWT
  description: All API requests carry the access token in an Authorization header of the form "Bearer <access>". Anonymous requests to the production host return HTTP 401 with body {"detail":"Authentication credentials were not provided."}.
  name: bearerAuth
  scheme: bearer
  sources:
  - https://docs.booksy.com/v01.html
  - https://us.booksy.com/public-api/us/business/
  type: http
slug: booksy-authentication
source_filename: booksy-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-31'\nmethod: searched\nsource: https://docs.booksy.com/v01.html\ndocs: https://docs.booksy.com/\nnote: >-\n  The live Booksy Public API docs host (docs.booksy.com) is served behind HTTP Basic\n  authentication (CloudFront returns 401 with WWW-Authenticate: Basic to anonymous\n  clients), so the authentication model below was captured from the identical\n  publicly archived rendering of the same documentation at\n  https://web.archive.org/web/20220706184310/https://alpha.docs.booksy.net/ and\n  corroborated against live 401 challenges from the production API host.\nsummary:\n  types:\n  - http\n  api_key_in: []\n  oauth2_flows: []\n  model: partner-issued RSA key pair signs an RS256 JWT assertion which is exchanged\n    for a short-lived bearer access token\nschemes:\n- name: partnerJwtAssertion\n  type: assertion\n  algorithm: RS256\n  description: >-\n    Before calling the API a partner signs a JWT with its own RSA private key\n    (separate private keys\
  \ are issued for sandbox and for production). The claim set\n    is iss (https://public-api.booksy.com), iat, exp and aud (the partner UUID); the\n    JOSE header carries typ JWT and alg RS256. The signed assertion is POSTed to\n    {base_url}/token/ together with partner_name.\n  token_endpoint: \"{base_url}/token/\"\n  sources:\n  - https://docs.booksy.com/v01.html\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: >-\n    All API requests carry the access token in an Authorization header of the form\n    \"Bearer <access>\". Anonymous requests to the production host return HTTP 401\n    with body {\"detail\":\"Authentication credentials were not provided.\"}.\n  sources:\n  - https://docs.booksy.com/v01.html\n  - https://us.booksy.com/public-api/us/business/\ntokens:\n  access_token_lifetime: 5 minutes\n  refresh_token_lifetime: 3 days\n  refresh:\n    description: >-\n      A refresh token is exchanged for a new access token so credentials are\
  \ not\n      re-sent on every expiry. Documented under \"Refresh token\".\ncredentials:\n  issuance: partner onboarding — Booksy issues a partner UUID, a partner name and an\n    RSA private key per environment\n  self_service: false\n  public_signup: false\nunverified_claims:\n- claim: >-\n    Third-party indexes of the current docs.booksy.com pages also describe an OAuth2\n    authorization-code flow with redirect_uri/state and refresh tokens for\n    user-approved requests.\n  status: unverified\n  reason: docs.booksy.com is HTTP Basic gated; no anonymous fetch could confirm an\n    oauth2 scheme, so no OAuth2 scheme or scope set is asserted here.\nx-evidence:\n- fetched: '2026-07-31'\n  url: https://docs.booksy.com/\n  http_status: 401\n  note: WWW-Authenticate Basic\n- fetched: '2026-07-31'\n  url: https://us.booksy.com/public-api/us/business/\n  http_status: 401\n  body: '{\"detail\":\"Authentication credentials were not provided.\"}'\n- fetched: '2026-07-31'\n  url: https://us.booksy.com/public-api/us/token/\n\
  \  http_status: 405\n  body: '{\"detail\":\"Method \\\"get\\\" not allowed.\"}'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/booksy/refs/heads/main/authentication/booksy-authentication.yml
summary_line: http · 2 schemes
tags:
- Beauty
- Wellness
- Booking
- Appointments
- Scheduling
- Marketplace
- Salons
- Barbershops
- Spas
- Payments
- Small Business
- Webhook
---
