---
api_key_in: []
api_specs:
- filename: treadio-horizon-openapi.json
  format: json
  label: Tread Horizon API V1
  slug: tread-horizon-api-v1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/treadio/refs/heads/main/openapi/treadio-horizon-openapi.json
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Treadio Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: tread.io secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: tread.io
provider_slug: treadio
scheme_count: 2
schemes:
- applied: global
  bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/treadio-horizon-openapi.json
  type: http
- documented_only: true
  flow: clientCredentials
  name: oauth2-client-credentials
  note: M2M flow documented in the API introduction but not declared as an OpenAPI securityScheme (the spec models the resulting bearer token as bearerAuth).
  sources:
  - https://docs.tread.ai/api-reference/introduction
  type: oauth2
slug: treadio-authentication
source_filename: treadio-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: openapi/treadio-horizon-openapi.json\ndocs: https://docs.tread.ai/api-reference/introduction\nsummary:\n  types: [http, oauth2]\n  scheme: bearer\n  bearer_format: JWT\n  oauth2_flows: [clientCredentials]\ndetail: >-\n  The Horizon API authenticates with bearer JWTs on every request\n  (Authorization: Bearer <token>). Two token-issuance flows exist:\n  (1) User session tokens — Stytch issues a short-lived JWT after a user logs in via\n  email+password, magic link, OTP over SMS, or SSO; use for tools acting on behalf of a\n  signed-in user. (2) Machine-to-machine (M2M) — Tread issues a Client ID and Client Secret\n  which are exchanged for an access token using the OAuth 2.0 client-credentials grant; use\n  for server-to-server integrations. M2M credentials are requested from developers@tread.io.\n  Tokens expire; on 401 unauthorized, fetch a new one.\nschemes:\n  - name: bearerAuth\n    type: http\n    scheme: bearer\n    bearerFormat:\
  \ JWT\n    applied: global\n    sources: [openapi/treadio-horizon-openapi.json]\n  - name: oauth2-client-credentials\n    type: oauth2\n    flow: clientCredentials\n    documented_only: true\n    note: >-\n      M2M flow documented in the API introduction but not declared as an OpenAPI\n      securityScheme (the spec models the resulting bearer token as bearerAuth).\n    sources: [https://docs.tread.ai/api-reference/introduction]\nlogin_flows: [email_password, magic_link, otp_sms, sso]\nscopes:\n  documented: false\n  note: >-\n    No OAuth scope/permission reference is published; access is governed by IAM roles and\n    permissions (Admin, Dispatcher, Foreman, Driver, Biller) rather than token scopes, so no\n    scopes/ artifact is emitted.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/treadio/refs/heads/main/authentication/treadio-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Company
- Construction
- Logistics
- Transportation Management
- Dispatch
- Fleet Management
- Bulk Materials
- Trucking
- Webhooks
- API
---
