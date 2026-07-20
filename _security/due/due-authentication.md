---
api_key_in: []
api_specs:
- filename: due-openapi-original.yml
  format: yaml
  label: Due API
  slug: due-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/due/refs/heads/main/openapi/due-openapi-original.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Due Authentication
name_suffix: Authentication
oauth_flows: []
overview: Due secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Due
provider_slug: due
scheme_count: 1
schemes:
- description: API key presented as a bearer token.
  header: Authorization
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/due-openapi-original.yml
  type: http
slug: due-authentication
source_filename: due-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: openapi/due-openapi-original.yml\ndocs: https://due.readme.io/docs/creating-customers\nsummary:\n  types:\n  - http\n  http_schemes:\n  - bearer\n  note: >-\n    Due authenticates with an API key presented as an HTTP bearer token (Authorization: Bearer <api_key>).\n    Per-account operations are additionally scoped by the Due-Account-Id header. Read-only FX/market\n    endpoints require no authentication. Sandbox and production use environment-specific keys/hosts.\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: API key presented as a bearer token.\n  header: Authorization\n  sources:\n  - openapi/due-openapi-original.yml\naccount_scoping:\n  header: Due-Account-Id\n  note: Scopes per-account requests (see webhook fetch/retry examples).\npublic_endpoints:\n  note: FX markets (getmarkets, getmarket, getmarkethistory) are public and require no authentication.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/due/refs/heads/main/authentication/due-authentication.yml
summary_line: http · 1 scheme
tags:
- Payments
- Cross-Border Payments
- Stablecoins
- Fintech
- Virtual Accounts
- Foreign Exchange
- KYC
- Wallets
- API
---
