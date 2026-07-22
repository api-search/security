---
api_key_in: []
auth_types:
- oauth2
- http-bearer
description: 'Parafin''s API uses OAuth 2.0 client-credentials: a platform authenticates with its client credentials to redeem a short-lived bearer token, which is then used as a Bearer Authorization header on API calls and to initialize the embedded Parafin Elements widgets. The public embedded-demo implements a server-side proxy so client credentials never reach the browser — the backend exchanges credentials and hands the browser only a per-person, per-product short-lived token. The docs are login-gated so the full securityScheme detail is not machine-verifiable; this profile is derived from the public demo and the OAuth server metadata advertised on the docs host.'
kind: authentication
layout: security
method: searched
name: Parafin Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Parafin secures its APIs with oauth2 and http-bearer across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Parafin
provider_slug: parafin
scheme_count: 2
schemes:
- description: Platform client credentials are exchanged for a short-lived bearer token via POST /v1/auth/redeem_token; the token authorizes API calls and widget initialization.
  flow: clientCredentials
  name: OAuth2ClientCredentials
  sources:
  - https://github.com/buildparafin/embedded-demo
  token_operation: POST /v1/auth/redeem_token
  type: oauth2
- description: Redeemed bearer token presented in the Authorization header.
  name: BearerAuth
  scheme: bearer
  sources:
  - https://github.com/buildparafin/embedded-demo
  type: http
slug: parafin-authentication
source_filename: parafin-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://github.com/buildparafin/embedded-demo\ndocs: https://docs.parafin.com/\ndescription: >-\n  Parafin's API uses OAuth 2.0 client-credentials: a platform authenticates with\n  its client credentials to redeem a short-lived bearer token, which is then\n  used as a Bearer Authorization header on API calls and to initialize the\n  embedded Parafin Elements widgets. The public embedded-demo implements a\n  server-side proxy so client credentials never reach the browser — the backend\n  exchanges credentials and hands the browser only a per-person, per-product\n  short-lived token. The docs are login-gated so the full securityScheme detail\n  is not machine-verifiable; this profile is derived from the public demo and the\n  OAuth server metadata advertised on the docs host.\nsummary:\n  types: [oauth2, http-bearer]\n  oauth2_flows: [clientCredentials]\n  token_style: short-lived bearer\nschemes:\n  - name: OAuth2ClientCredentials\n\
  \    type: oauth2\n    flow: clientCredentials\n    token_operation: POST /v1/auth/redeem_token\n    description: >-\n      Platform client credentials are exchanged for a short-lived bearer token\n      via POST /v1/auth/redeem_token; the token authorizes API calls and widget\n      initialization.\n    sources: [https://github.com/buildparafin/embedded-demo]\n  - name: BearerAuth\n    type: http\n    scheme: bearer\n    description: Redeemed bearer token presented in the Authorization header.\n    sources: [https://github.com/buildparafin/embedded-demo]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/parafin/refs/heads/main/authentication/parafin-authentication.yml
summary_line: oauth2/http-bearer · 2 schemes
tags:
- Company
- Fintech
- Embedded Finance
- Lending
- Capital
- Payments
- Small Business
- Working Capital
- API
---
