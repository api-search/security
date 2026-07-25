---
api_key_in:
- header
api_specs:
- filename: newline-platform-api.json
  format: json
  label: Newline Auth API
  slug: newline-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fifth-third-bancorp/refs/heads/main/openapi/newline-platform-api.json
- filename: newline-platform-api.json
  format: json
  label: Newline Customers API
  slug: newline-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fifth-third-bancorp/refs/heads/main/openapi/newline-platform-api.json
- filename: newline-platform-api.json
  format: json
  label: Newline Customer Products API
  slug: newline-customer-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fifth-third-bancorp/refs/heads/main/openapi/newline-platform-api.json
- filename: newline-platform-api.json
  format: json
  label: Newline Products API
  slug: newline-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fifth-third-bancorp/refs/heads/main/openapi/newline-platform-api.json
- filename: newline-platform-api.json
  format: json
  label: Newline Pools API
  slug: newline-pools-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fifth-third-bancorp/refs/heads/main/openapi/newline-platform-api.json
- filename: newline-platform-api.json
  format: json
  label: Newline Custodial Accounts API
  slug: newline-custodial-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fifth-third-bancorp/refs/heads/main/openapi/newline-platform-api.json
- filename: newline-platform-api.json
  format: json
  label: Newline Synthetic Accounts API
  slug: newline-synthetic-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fifth-third-bancorp/refs/heads/main/openapi/newline-platform-api.json
- filename: newline-platform-api.json
  format: json
  label: Newline Transfers API
  slug: newline-transfers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fifth-third-bancorp/refs/heads/main/openapi/newline-platform-api.json
- filename: newline-platform-api.json
  format: json
  label: Newline Combined Transfers API
  slug: newline-combined-transfers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fifth-third-bancorp/refs/heads/main/openapi/newline-platform-api.json
- filename: newline-platform-api.json
  format: json
  label: Newline Transactions API
  slug: newline-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fifth-third-bancorp/refs/heads/main/openapi/newline-platform-api.json
- filename: newline-platform-api.json
  format: json
  label: Newline Returns API
  slug: newline-returns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fifth-third-bancorp/refs/heads/main/openapi/newline-platform-api.json
- filename: newline-platform-api.json
  format: json
  label: Newline Virtual Reference Numbers API
  slug: newline-virtual-reference-numbers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fifth-third-bancorp/refs/heads/main/openapi/newline-platform-api.json
- filename: newline-platform-api.json
  format: json
  label: Newline Sandbox API
  slug: newline-sandbox-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fifth-third-bancorp/refs/heads/main/openapi/newline-platform-api.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Fifth Third Bancorp Authentication
name_suffix: Authentication
oauth_flows: []
overview: Fifth Third Bancorp secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Fifth Third Bancorp
provider_slug: fifth-third-bancorp
scheme_count: 1
schemes:
- description: Access token (auth- prefixed) obtained from POST /auth by signing a JWS with the shared HMAC (HS512); supplied in the Authorization header.
  in: header
  name: ApiKeyAuth
  parameter: Authorization
  sources:
  - openapi/newline-platform-api.json
  type: apiKey
slug: fifth-third-bancorp-authentication
source_filename: fifth-third-bancorp-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-23'\nmethod: searched\nsource: openapi/newline-platform-api.json\ndocs: https://developers.newline53.com/docs/api-authentication\ndocs_pages:\n  - https://developers.newline53.com/docs/authentication-guide\n  - https://developers.newline53.com/docs/api-authentication\n  - https://developers.newline53.com/docs/authorization-guide\n  - https://developers.newline53.com/docs/sdk-authentication\nsummary:\n  types:\n    - apiKey\n  api_key_in:\n    - header\n  oauth2_flows: []\nmodel: jws-hmac-bearer\nnotes: >-\n  The Newline Platform API uses a JWT/JWS-based bearer strategy. A client\n  exchanges a refresh token for an access token by POSTing to /auth a JWS whose\n  payload carries the Program UID (sub) and current epoch time (iat), signed\n  with a previously shared HMAC secret using HS512. The returned access token\n  (prefixed \"auth-\") is valid up to 8 hours and is supplied in the Authorization\n  header of every subsequent request. The sandbox uses an identical\
  \ token\n  strategy to production. HMAC secrets/Program IDs are provisioned by the\n  Newline Relationship team over secure email (no self-service signup at this time).\nschemes:\n  - name: ApiKeyAuth\n    type: apiKey\n    in: header\n    parameter: Authorization\n    description: >-\n      Access token (auth- prefixed) obtained from POST /auth by signing a JWS\n      with the shared HMAC (HS512); supplied in the Authorization header.\n    sources:\n      - openapi/newline-platform-api.json\nsigning:\n  algorithm: HS512\n  jws_payload:\n    sub: Program UID\n    iat: current epoch time\n  token_prefix: auth-\n  token_ttl: up to 8 hours\nprovisioning: Relationship-team issued (secure email); no self-service signup\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fifth-third-bancorp/refs/heads/main/authentication/fifth-third-bancorp-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Banking
- United States
- Embedded Finance
- Banking as a Service
- Payments
- ACH
- Real-Time Payments
- Deposits
- Card Issuing
- Commercial Banking
- Consumer Lending
- Wealth Management
- Treasury Management
- Super-Regional Bank
- Fortune 500
---
