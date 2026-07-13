---
api_key_in: []
api_specs:
- filename: pismo-openapi.yml
  format: yaml
  label: Pismo Accounts API
  slug: pismo-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pismo/refs/heads/main/openapi/pismo-openapi.yml
- filename: pismo-openapi.yml
  format: yaml
  label: Pismo Customers API
  slug: pismo-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pismo/refs/heads/main/openapi/pismo-openapi.yml
- filename: pismo-openapi.yml
  format: yaml
  label: Pismo Cards API
  slug: pismo-cards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pismo/refs/heads/main/openapi/pismo-openapi.yml
- filename: pismo-openapi.yml
  format: yaml
  label: Pismo Authorizations API
  slug: pismo-authorizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pismo/refs/heads/main/openapi/pismo-openapi.yml
- filename: pismo-openapi.yml
  format: yaml
  label: Pismo Transactions and Statements API
  slug: pismo-transactions-statements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pismo/refs/heads/main/openapi/pismo-openapi.yml
- filename: pismo-openapi.yml
  format: yaml
  label: Pismo Programs API
  slug: pismo-programs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pismo/refs/heads/main/openapi/pismo-openapi.yml
- filename: pismo-openapi.yml
  format: yaml
  label: Pismo Events API
  slug: pismo-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pismo/refs/heads/main/openapi/pismo-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Pismo Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Pismo secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Pismo
provider_slug: pismo
scheme_count: 2
schemes:
- bearerFormat: JWT
  description: 'OAuth2 client-credentials access token obtained from POST /passport/v2/oauth/token. Pass as `Authorization: Bearer <token>`. Account-scoped endpoints require an account-specific token encoded with a Pismo account ID.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/pismo-openapi.yml
  type: http
- flows:
  - flow: clientCredentials
    scopes: 0
    tokenUrl: https://api.pismo.io/passport/v2/oauth/token
  name: oauth2
  sources:
  - openapi/pismo-openapi.yml
  type: oauth2
slug: pismo-authentication
source_filename: pismo-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/pismo-openapi.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: 'OAuth2 client-credentials access token obtained from POST /passport/v2/oauth/token.\n    Pass as `Authorization: Bearer <token>`. Account-scoped endpoints require an account-specific\n    token encoded with a Pismo account ID.'\n  sources:\n  - openapi/pismo-openapi.yml\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.pismo.io/passport/v2/oauth/token\n    scopes: 0\n  sources:\n  - openapi/pismo-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pismo/refs/heads/main/authentication/pismo-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Banking
- Card Issuing
- Payments
- Fintech
- Core Banking
- Cloud Native
---
