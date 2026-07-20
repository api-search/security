---
api_key_in: []
api_specs:
- filename: bcb-group-payments-openapi.json
  format: json
  label: BCB Group Payments API
  slug: bcb-group-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bcb-group/refs/heads/main/openapi/bcb-group-payments-openapi.json
auth_types:
- oauth2
- http
description: ''
kind: authentication
layout: security
method: searched
name: Bcb Group Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: BCB Group secures its APIs with oauth2 and http across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: BCB Group
provider_slug: bcb-group
scheme_count: 2
schemes:
- flow: clientCredentials
  name: OAuth2ClientCredentials
  request: 'POST application/json {"client_id": "...", "client_secret": "..."}'
  source: https://docs.bcb.group/reference/get-token
  token_url: https://api.bcb.group/v1/auth/oauth/token
  token_url_sandbox: https://api.uat.bcb.group/v1/auth/oauth/token
  type: oauth2
- bearer_format: JWT
  header: Authorization
  in: header
  name: BearerAuth
  note: Access token returned by the token endpoint (access_token, expires_in unix timestamp). The `scope` and `token_type` fields are documented as deprecated.
  scheme: bearer
  type: http
slug: bcb-group-authentication
source_filename: bcb-group-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://docs.bcb.group/docs/api-authentication.md\ndocs: https://docs.bcb.group/docs/api-authentication\nsummary:\n  types: [oauth2, http]\n  oauth2_flows: [clientCredentials]\n  bearer: true\nmodel: >-\n  All BCB Group Payments API calls require OAuth 2.0 Client Credentials Grant.\n  The application exchanges a Client ID and Client Secret at the token endpoint\n  for a short-lived Access Token, then presents it as a Bearer token in the\n  Authorization header of every request. Credentials are environment-specific\n  (separate Sandbox and Production Client ID/Secret).\nschemes:\n  - name: OAuth2ClientCredentials\n    type: oauth2\n    flow: clientCredentials\n    token_url: https://api.bcb.group/v1/auth/oauth/token\n    token_url_sandbox: https://api.uat.bcb.group/v1/auth/oauth/token\n    request: 'POST application/json {\"client_id\": \"...\", \"client_secret\": \"...\"}'\n    source: https://docs.bcb.group/reference/get-token\n\
  \  - name: BearerAuth\n    type: http\n    scheme: bearer\n    bearer_format: JWT\n    in: header\n    header: Authorization\n    note: >-\n      Access token returned by the token endpoint (access_token, expires_in unix\n      timestamp). The `scope` and `token_type` fields are documented as deprecated.\ncredentials_source: Provided by BCB Group on successful registration/onboarding; distinct per environment.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bcb-group/refs/heads/main/authentication/bcb-group-authentication.yml
summary_line: oauth2/http · 2 schemes
tags:
- Company
- Crypto
- Payments
- Banking
- Digital Assets
- Stablecoins
- Financial Services
- Fintech
---
