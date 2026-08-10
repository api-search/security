---
api_key_in: []
api_specs:
- filename: niural-authentication-api-openapi.yml
  format: yaml
  label: Niural Authentication API
  slug: niural-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/niural/refs/heads/main/openapi/niural-authentication-api-openapi.yml
- filename: niural-contracts-api-openapi.yml
  format: yaml
  label: Niural Contracts API
  slug: niural-contracts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/niural/refs/heads/main/openapi/niural-contracts-api-openapi.yml
- filename: niural-invoices-api-openapi.yml
  format: yaml
  label: Niural Invoices API
  slug: niural-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/niural/refs/heads/main/openapi/niural-invoices-api-openapi.yml
- filename: niural-transactions-api-openapi.yml
  format: yaml
  label: Niural Transactions API
  slug: niural-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/niural/refs/heads/main/openapi/niural-transactions-api-openapi.yml
auth_types:
- http
description: Niural uses a bespoke two-step credential exchange. Client credentials created in the dashboard are POSTed to /authenticate, which returns a JWT access token (3600s), a refresh token, and expires_in. That token is presented as an HTTP bearer credential on every other operation. It is client-credentials shaped but is NOT OAuth 2.0 — there is no grant_type, no token_type, no scope, no /.well-known/oauth-authorization-server, and therefore no scope surface.
kind: authentication
layout: security
method: searched
name: Niural Authentication
name_suffix: Authentication
oauth_flows: []
overview: Niural secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Niural
provider_slug: niural
scheme_count: 1
schemes:
- applied: global (root-level security), exempted only on POST /authenticate
  bearerFormat: JWT
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/niural-public-api-openapi.yml
  type: http
slug: niural-authentication
source_filename: niural-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: searched\nsource: openapi/niural-public-api-openapi.yml\ndocs: https://docs.niural.com/docs/authentications\ndescription: >-\n  Niural uses a bespoke two-step credential exchange. Client credentials created\n  in the dashboard are POSTed to /authenticate, which returns a JWT access token\n  (3600s), a refresh token, and expires_in. That token is presented as an HTTP\n  bearer credential on every other operation. It is client-credentials shaped but\n  is NOT OAuth 2.0 — there is no grant_type, no token_type, no scope, no\n  /.well-known/oauth-authorization-server, and therefore no scope surface.\nsummary:\n  types:\n  - http\n  api_key_in: []\n  oauth2_flows: []\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/niural-public-api-openapi.yml\n  applied: global (root-level security), exempted only on POST /authenticate\ncredential_exchange:\n  endpoint: POST /authenticate\n  hosts:\n  -\
  \ https://api-sandbox.niural.com\n  - https://api-live.niural.com\n  request: {client_id: uuid, client_secret: string}\n  response: {access_token: JWT, refresh_token: string, expires_in: 3600}\n  errors: [400 Invalid Request, 422 Validation error, 500 Server Error]\n  docs: https://docs.niural.com/docs/authentications\ncredential_management:\n  created_in: Niural dashboard — Organization > Developer > API Keys\n  naming: Keys are named by the operator (e.g. \"staging\", \"production\").\n  secret_visibility: Shown once at creation; recoverable only by rotating the key.\n  rotation: Rotating invalidates the previous client secret immediately.\n  docs: https://docs.niural.com/docs/auth-keys\nrequired_headers:\n- {name: Authorization, value: 'Bearer <access_token>'}\n- {name: Accept, value: application/json}\n- {name: Content-Type, value: application/json}\nscopes:\n  supported: false\n  note: >-\n    No scope, permission or role model is published. A Niural API key is\n    all-or-nothing\
  \ across contracts, invoices and money movement — there is no way\n    to issue a read-only credential to an agent or a third party.\ngaps:\n- No OAuth 2.0 / OIDC discovery document on any host.\n- No scoped or restricted keys, so least-privilege delegation is impossible.\n- Token lifetime is fixed at 3600s with no documented refresh-token lifetime or\n  revocation endpoint.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/niural/refs/heads/main/authentication/niural-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Payroll
- Human Resources
- Employer of Record
- Contractor Management
- Global Payments
- Invoicing
- Compliance
- Fintech
---
