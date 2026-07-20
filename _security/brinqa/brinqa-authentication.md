---
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Brinqa Authentication
name_suffix: Authentication
oauth_flows: []
overview: Brinqa secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Brinqa
provider_slug: brinqa
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: 'Bearer access token obtained by POSTing user credentials to https://<your-brinqa-platform-url>/api/auth/login. Presented as "Authorization: Bearer <token>" on GraphQL requests to https://<your-brinqa-platform-url>/graphql/caasm.'
  mfa_supported: true
  name: bearerAuth
  scheme: bearer
  sources:
  - docs.brinqa.com/docs/brinqa-api
  token_endpoint: https://<your-brinqa-platform-url>/api/auth/login
  token_lifetime_seconds: 86400
  type: http
slug: brinqa-authentication
source_filename: brinqa-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://docs.brinqa.com/docs/brinqa-api\ndocs: https://docs.brinqa.com/docs/brinqa-api\nsummary:\n  types: [http]\n  http_schemes: [bearer]\n  api_key_in: []\n  oauth2_flows: []\n  notes: >-\n    The Brinqa Platform API uses bearer token authentication. A caller first\n    obtains an access token by POSTing credentials to the platform's login\n    endpoint, then presents the token as an Authorization: Bearer header on\n    subsequent GraphQL requests. Multi-factor authentication (MFA) is supported\n    during token generation. Tokens are valid for 86400 seconds (24 hours).\nschemes:\n  - name: bearerAuth\n    type: http\n    scheme: bearer\n    bearerFormat: JWT\n    description: >-\n      Bearer access token obtained by POSTing user credentials to\n      https://<your-brinqa-platform-url>/api/auth/login. Presented as\n      \"Authorization: Bearer <token>\" on GraphQL requests to\n      https://<your-brinqa-platform-url>/graphql/caasm.\n\
  \    token_endpoint: https://<your-brinqa-platform-url>/api/auth/login\n    token_lifetime_seconds: 86400\n    mfa_supported: true\n    sources: [docs.brinqa.com/docs/brinqa-api]\nnotes: >-\n  Brinqa is deployed per-tenant, so the token and GraphQL endpoints are relative\n  to each customer's platform URL rather than a single shared host. No OAuth2 /\n  OpenID Connect authorization-server metadata is published; there is no OAuth\n  scope surface (bearer-token model), so no scopes/ artifact is emitted.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/brinqa/refs/heads/main/authentication/brinqa-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Cybersecurity
- Vulnerability Management
- Exposure Management
- Cyber Risk
- Risk Management
- Security
- GraphQL
---
