---
api_key_in: []
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Fama Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Fama secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Fama
provider_slug: fama
scheme_count: 2
schemes:
- applies_to:
  - v1
  - v2
  description: 'Present the Fama access/API token as `Authorization: Bearer <YOUR_ACCESS_TOKEN>`. Used by the v2 public API (public-api.fama.io) and by v1 once an access token is obtained.'
  name: bearerAuth
  scheme: bearer
  source: https://developer.fama.io/reference/authentication
  type: http
- description: 'v1 access-token retrieval. POST to the token endpoint with grant_type=client_credentials and an `Authorization: Basic base64(username:password)` header (admin credentials from the deprecated v1 portal). Response returns the bearer token plus an `expires_in` field. No public scope catalog is documented.'
  flows:
  - flow: clientCredentials
    scopes: {}
    tokenUrl: https://api.sandbox.service.fama.io/api/oauth/token
  name: oauth2ClientCredentials
  source: https://developer.fama.io/docs/access-token
  type: oauth2
slug: fama-authentication
source_filename: fama-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://developer.fama.io/reference/authentication\ndocs: https://developer.fama.io/reference/authentication\nsummary:\n  types: [http, oauth2]\n  http_scheme: bearer\n  oauth2_flows: [clientCredentials]\n  notes: >-\n    The Fama REST API authenticates every request with a bearer token in the\n    Authorization header. New customers use the v2 \"API Token\" onboarding; customers\n    migrating from the deprecated v1 portal mint an access token via an OAuth 2.0\n    client-credentials exchange (HTTP Basic of username:password against the v1 token\n    endpoint) and then present the resulting token as a bearer credential.\nschemes:\n  - name: bearerAuth\n    type: http\n    scheme: bearer\n    description: >-\n      Present the Fama access/API token as `Authorization: Bearer <YOUR_ACCESS_TOKEN>`.\n      Used by the v2 public API (public-api.fama.io) and by v1 once an access token\n      is obtained.\n    applies_to: [v1, v2]\n\
  \    source: https://developer.fama.io/reference/authentication\n  - name: oauth2ClientCredentials\n    type: oauth2\n    description: >-\n      v1 access-token retrieval. POST to the token endpoint with\n      grant_type=client_credentials and an `Authorization: Basic base64(username:password)`\n      header (admin credentials from the deprecated v1 portal). Response returns the\n      bearer token plus an `expires_in` field. No public scope catalog is documented.\n    flows:\n      - flow: clientCredentials\n        tokenUrl: https://api.sandbox.service.fama.io/api/oauth/token\n        scopes: {}\n    source: https://developer.fama.io/docs/access-token\ntoken_delivery: header\nheader_example: 'Authorization: Bearer <YOUR_ACCESS_TOKEN>'\nonboarding:\n  - guide: API Token (v2, new customers)\n    url: https://developer.fama.io/reference/api-token\n  - guide: Access Token (v1 migration)\n    url: https://developer.fama.io/docs/access-token\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fama/refs/heads/main/authentication/fama-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Company
- Employment Screening
- Background Checks
- Human Resources
- Social Media
- Risk
- Compliance
- Artificial Intelligence
---
