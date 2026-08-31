---
api_key_in: []
api_specs:
- filename: volt-io-account-holder-verification-api-openapi.yml
  format: yaml
  label: Volt Account Holder Verification API
  slug: volt-io-account-holder-verification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/volt-io/refs/heads/main/openapi/volt-io-account-holder-verification-api-openapi.yml
- filename: volt-io-accounts-api-openapi.yml
  format: yaml
  label: Volt Accounts API
  slug: volt-io-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/volt-io/refs/heads/main/openapi/volt-io-accounts-api-openapi.yml
- filename: volt-io-aliases-api-openapi.yml
  format: yaml
  label: Volt Aliases API
  slug: volt-io-aliases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/volt-io/refs/heads/main/openapi/volt-io-aliases-api-openapi.yml
- filename: volt-io-named-accounts-api-openapi.yml
  format: yaml
  label: Volt Named Accounts API
  slug: volt-io-named-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/volt-io/refs/heads/main/openapi/volt-io-named-accounts-api-openapi.yml
- filename: volt-io-sandbox-api-openapi.yml
  format: yaml
  label: Volt Sandbox API
  slug: volt-io-sandbox-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/volt-io/refs/heads/main/openapi/volt-io-sandbox-api-openapi.yml
- filename: volt-io-transactions-api-openapi.yml
  format: yaml
  label: Volt Transactions API
  slug: volt-io-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/volt-io/refs/heads/main/openapi/volt-io-transactions-api-openapi.yml
- filename: volt-io-trusted-accounts-api-openapi.yml
  format: yaml
  label: Volt Trusted accounts API
  slug: volt-io-trusted-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/volt-io/refs/heads/main/openapi/volt-io-trusted-accounts-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Volt Io Authentication
name_suffix: Authentication
oauth_flows:
- password
overview: Volt secures its APIs with http and oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the password flow(s).
provider_name: Volt
provider_slug: volt-io
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/volt-io-accounts-openapi-original.yaml
  type: http
slug: volt-io-authentication
source_filename: volt-io-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-24'\nmethod: searched\nsource: openapi/volt-io-accounts-openapi-original.yaml\ndocs: https://docs.volt.io/implementation/essentials/authentication\nsummary:\n  types:\n  - http\n  - oauth2\n  api_key_in: []\n  oauth2_flows:\n  - password\ntoken_flow:\n  grant: resource-owner-password (OAuth2)\n  token_endpoint: POST https://gateway.volt.io/oauth\n  inputs: [client_id, client_secret, username, password]\n  credential_source: Fuzebox (application registration + API credentials)\n  returns: Bearer access_token (JWT)\n  usage: 'Authorization: Bearer <access_token> on all API calls'\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/volt-io-accounts-openapi-original.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/volt-io/refs/heads/main/authentication/volt-io-authentication.yml
summary_line: http/oauth2 · 1 scheme
tags:
- Payments
- United Kingdom
- Open Banking
- Account-to-Account
- Real-Time Payments
- Payment Initiation
- Payouts
- Recurring Payments
- Cross-Border
- Pay by Bank
---
