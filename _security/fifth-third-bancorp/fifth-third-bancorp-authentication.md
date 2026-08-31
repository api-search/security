---
api_key_in:
- header
api_specs:
- filename: fifth-third-bancorp-auth-api-openapi.yml
  format: yaml
  label: Fifth Third Bancorp Auth API
  slug: fifth-third-bancorp-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fifth-third-bancorp/refs/heads/main/openapi/fifth-third-bancorp-auth-api-openapi.yml
- filename: fifth-third-bancorp-combined-transfers-api-openapi.yml
  format: yaml
  label: Fifth Third Bancorp Combined Transfers API
  slug: fifth-third-bancorp-combined-transfers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fifth-third-bancorp/refs/heads/main/openapi/fifth-third-bancorp-combined-transfers-api-openapi.yml
- filename: fifth-third-bancorp-custodial-accounts-api-openapi.yml
  format: yaml
  label: Fifth Third Bancorp Custodial Accounts API
  slug: fifth-third-bancorp-custodial-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fifth-third-bancorp/refs/heads/main/openapi/fifth-third-bancorp-custodial-accounts-api-openapi.yml
- filename: fifth-third-bancorp-customer-products-api-openapi.yml
  format: yaml
  label: Fifth Third Bancorp Customer Products API
  slug: fifth-third-bancorp-customer-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fifth-third-bancorp/refs/heads/main/openapi/fifth-third-bancorp-customer-products-api-openapi.yml
- filename: fifth-third-bancorp-customers-api-openapi.yml
  format: yaml
  label: Fifth Third Bancorp Customers API
  slug: fifth-third-bancorp-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fifth-third-bancorp/refs/heads/main/openapi/fifth-third-bancorp-customers-api-openapi.yml
- filename: fifth-third-bancorp-pools-api-openapi.yml
  format: yaml
  label: Fifth Third Bancorp Pools API
  slug: fifth-third-bancorp-pools-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fifth-third-bancorp/refs/heads/main/openapi/fifth-third-bancorp-pools-api-openapi.yml
- filename: fifth-third-bancorp-products-api-openapi.yml
  format: yaml
  label: Fifth Third Bancorp Products API
  slug: fifth-third-bancorp-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fifth-third-bancorp/refs/heads/main/openapi/fifth-third-bancorp-products-api-openapi.yml
- filename: fifth-third-bancorp-returns-api-openapi.yml
  format: yaml
  label: Fifth Third Bancorp Returns API
  slug: fifth-third-bancorp-returns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fifth-third-bancorp/refs/heads/main/openapi/fifth-third-bancorp-returns-api-openapi.yml
- filename: fifth-third-bancorp-sandbox-api-openapi.yml
  format: yaml
  label: Fifth Third Bancorp Sandbox API
  slug: fifth-third-bancorp-sandbox-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fifth-third-bancorp/refs/heads/main/openapi/fifth-third-bancorp-sandbox-api-openapi.yml
- filename: fifth-third-bancorp-synthetic-accounts-api-openapi.yml
  format: yaml
  label: Fifth Third Bancorp Synthetic Accounts API
  slug: fifth-third-bancorp-synthetic-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fifth-third-bancorp/refs/heads/main/openapi/fifth-third-bancorp-synthetic-accounts-api-openapi.yml
- filename: fifth-third-bancorp-transactions-api-openapi.yml
  format: yaml
  label: Fifth Third Bancorp Transactions API
  slug: fifth-third-bancorp-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fifth-third-bancorp/refs/heads/main/openapi/fifth-third-bancorp-transactions-api-openapi.yml
- filename: fifth-third-bancorp-transfers-api-openapi.yml
  format: yaml
  label: Fifth Third Bancorp Transfers API
  slug: fifth-third-bancorp-transfers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fifth-third-bancorp/refs/heads/main/openapi/fifth-third-bancorp-transfers-api-openapi.yml
- filename: fifth-third-bancorp-virtual-reference-numbers-api-openapi.yml
  format: yaml
  label: Fifth Third Bancorp Virtual Reference Numbers API
  slug: fifth-third-bancorp-virtual-reference-numbers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fifth-third-bancorp/refs/heads/main/openapi/fifth-third-bancorp-virtual-reference-numbers-api-openapi.yml
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
