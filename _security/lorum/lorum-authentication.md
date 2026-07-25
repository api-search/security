---
api_key_in: []
api_specs:
- filename: lorum-accounts-api-openapi.yml
  format: yaml
  label: Lorum Accounts API
  slug: lorum-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lorum/refs/heads/main/openapi/lorum-accounts-api-openapi.yml
- filename: lorum-customers-api-openapi.yml
  format: yaml
  label: Lorum Customers API
  slug: lorum-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lorum/refs/heads/main/openapi/lorum-customers-api-openapi.yml
- filename: lorum-customers-v2-api-openapi.yml
  format: yaml
  label: Lorum Customers V2 API
  slug: lorum-customers-v2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lorum/refs/heads/main/openapi/lorum-customers-v2-api-openapi.yml
- filename: lorum-documents-api-openapi.yml
  format: yaml
  label: Lorum Documents API
  slug: lorum-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lorum/refs/heads/main/openapi/lorum-documents-api-openapi.yml
- filename: lorum-exchange-api-openapi.yml
  format: yaml
  label: Lorum Exchange API
  slug: lorum-exchange-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lorum/refs/heads/main/openapi/lorum-exchange-api-openapi.yml
- filename: lorum-internal-transfers-api-openapi.yml
  format: yaml
  label: Lorum Internal Transfers API
  slug: lorum-internal-transfers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lorum/refs/heads/main/openapi/lorum-internal-transfers-api-openapi.yml
- filename: lorum-oauth-api-openapi.yml
  format: yaml
  label: Lorum Oauth API
  slug: lorum-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lorum/refs/heads/main/openapi/lorum-oauth-api-openapi.yml
- filename: lorum-payments-api-openapi.yml
  format: yaml
  label: Lorum Payments API
  slug: lorum-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lorum/refs/heads/main/openapi/lorum-payments-api-openapi.yml
- filename: lorum-simulation-api-openapi.yml
  format: yaml
  label: Lorum Simulation API
  slug: lorum-simulation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lorum/refs/heads/main/openapi/lorum-simulation-api-openapi.yml
- filename: lorum-transactions-api-openapi.yml
  format: yaml
  label: Lorum Transactions API
  slug: lorum-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lorum/refs/heads/main/openapi/lorum-transactions-api-openapi.yml
auth_types:
- oauth2
- http
description: ''
kind: authentication
layout: security
method: searched
name: Lorum Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Lorum secures its APIs with oauth2 and http across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Lorum
provider_slug: lorum
scheme_count: 2
schemes:
- bearerFormat: JWT
  name: OAuth2
  scheme: bearer
  sources:
  - openapi/lorum-openapi-original.json
  type: http
- audience_default: https://api.fuse.me
  flow: clientCredentials
  issuer: https://auth.fuse.me/
  name: ClientCredentials
  provider: auth0
  source: https://docs.lorum.com/docs/authenticating-to-the-api
  token_lifetime_seconds: 10800
  token_url_production: https://auth.fuse.me/oauth/token
  token_url_sandbox: https://auth-sandbox.fuse.me/oauth/token
  type: oauth2
slug: lorum-authentication
source_filename: lorum-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: openapi/lorum-openapi-original.json\ndocs: https://docs.lorum.com/docs/authenticating-to-the-api\nsummary:\n  types:\n  - oauth2\n  - http\n  oauth2_flows:\n  - clientCredentials\n  api_key_in: []\n  notes: >-\n    Lorum (Fuse) uses the OAuth 2.0 client credentials grant to mint a JWT\n    bearer access_token, which is then presented as `Authorization: Bearer\n    <token>` on every API call. Tokens are valid for 3 hours and MUST be cached\n    and reused - integrations that request a new token per call are not\n    certified for production. The authorization server is Auth0-backed.\nschemes:\n- name: OAuth2\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/lorum-openapi-original.json\n- name: ClientCredentials\n  type: oauth2\n  flow: clientCredentials\n  token_url_production: https://auth.fuse.me/oauth/token\n  token_url_sandbox: https://auth-sandbox.fuse.me/oauth/token\n  audience_default: https://api.fuse.me\n\
  \  token_lifetime_seconds: 10800\n  issuer: https://auth.fuse.me/\n  provider: auth0\n  source: https://docs.lorum.com/docs/authenticating-to-the-api\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lorum/refs/heads/main/authentication/lorum-authentication.yml
summary_line: oauth2/http · 2 schemes
tags:
- Company
- Fintech
- Payments
- Banking
- Clearing
- Settlement
- Treasury
- Multi-Currency
- Accounts
- Foreign Exchange
- Webhooks
---
