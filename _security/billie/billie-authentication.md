---
api_key_in: []
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Billie Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Billie secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Billie
provider_slug: billie
scheme_count: 1
schemes:
- flow: clientCredentials
  grant_type: client_credentials
  header: 'Authorization: Bearer <access_token>'
  name: OAuth2
  revoke_endpoint: DELETE /api/v2/oauth/token
  scopes: []
  source: https://docs.billie.io/reference/authentication
  token_format: JWT
  token_ttl_seconds: 28800
  token_url: https://paella.billie.io/api/v2/oauth/token
  token_url_sandbox: https://paella-sandbox.billie.io/api/v2/oauth/token
  type: oauth2
  validate_endpoint: GET /api/v2/oauth/token
slug: billie-authentication
source_filename: billie-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://docs.billie.io/reference/authentication.md\ndocs: https://docs.billie.io/reference/authentication\nnotes: >-\n  Billie's Payment API uses OAuth 2.0 client_credentials. Merchants receive a\n  Client ID and Client Secret at onboarding and exchange them at the token\n  endpoint for a Bearer JWT, presented on every request as\n  `Authorization: Bearer <jwt>`. Tokens expire after 8 hours (default TTL);\n  on HTTP 401 the client requests a fresh token and retries. Tokens can be\n  validated and revoked via dedicated OAuth endpoints. No user-delegated\n  authorization-code flow and no granular OAuth scopes are documented — the\n  client-credentials grant conveys the merchant's full API entitlement.\nsummary:\n  types: [oauth2]\n  oauth2_flows: [clientCredentials]\n  api_key_in: []\nschemes:\n  - name: OAuth2\n    type: oauth2\n    flow: clientCredentials\n    grant_type: client_credentials\n    token_url: https://paella.billie.io/api/v2/oauth/token\n\
  \    token_url_sandbox: https://paella-sandbox.billie.io/api/v2/oauth/token\n    token_ttl_seconds: 28800\n    token_format: JWT\n    header: 'Authorization: Bearer <access_token>'\n    validate_endpoint: GET /api/v2/oauth/token\n    revoke_endpoint: DELETE /api/v2/oauth/token\n    scopes: []\n    source: https://docs.billie.io/reference/authentication\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/billie/refs/heads/main/authentication/billie-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Fintech
- Payments
- BNPL
- Buy Now Pay Later
- B2B
- Invoicing
- Checkout
- Germany
---
