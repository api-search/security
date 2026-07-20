---
api_key_in: []
api_specs:
- filename: fin-openapi-original.yml
  format: yaml
  label: Fin.com Orchestration API
  slug: fincom-orchestration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fin/refs/heads/main/openapi/fin-openapi-original.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Fin Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Fin secures its APIs with http and oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Fin
provider_slug: fin
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: Bearer token authentication. Obtain token from the Issue a Token endpoint.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/fin-openapi-original.yml
  type: http
slug: fin-authentication
source_filename: fin-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: openapi/fin-openapi-original.yml\ndocs: https://developer.fin.com/api-reference/authentication/issue-a-token\nsummary:\n  types:\n  - http\n  - oauth2\n  api_key_in: []\n  oauth2_flows:\n  - clientCredentials\n  notes: >-\n    The OpenAPI declares a single http bearer (JWT) security scheme applied to\n    all operations. Per the docs the bearer token is obtained via an OAuth 2.0\n    client-credentials flow with an enhanced refresh mechanism: exchange client\n    credentials at POST /v1/oauth/token to receive an access token + refresh\n    token, then renew via POST /v1/oauth/refresh-token without re-authenticating.\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: Bearer token authentication. Obtain token from the Issue a Token endpoint.\n  sources:\n  - openapi/fin-openapi-original.yml\nflows:\n- flow: clientCredentials\n  token_endpoint: https://api.fin.com/v1/oauth/token\n\
  \  refresh_endpoint: https://api.fin.com/v1/oauth/refresh-token\n  sandbox_token_endpoint: https://sandbox.api.fin.com/v1/oauth/token\n  docs: https://developer.fin.com/api-reference/authentication/issue-a-token\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fin/refs/heads/main/authentication/fin-authentication.yml
summary_line: http/oauth2 · 1 scheme
tags:
- Company
- Payments
- Cross-Border Payments
- Stablecoins
- Fintech
- Money Movement
- Foreign Exchange
- Virtual Accounts
- Crypto
---
