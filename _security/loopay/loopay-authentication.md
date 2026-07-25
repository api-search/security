---
api_key_in:
- header
api_specs:
- filename: loopay-affiliate-api-openapi.yml
  format: yaml
  label: Loopay Affiliate API
  slug: loopay-affiliate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loopay/refs/heads/main/openapi/loopay-affiliate-api-openapi.yml
- filename: loopay-bank-api-openapi.yml
  format: yaml
  label: Loopay Bank API
  slug: loopay-bank-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loopay/refs/heads/main/openapi/loopay-bank-api-openapi.yml
- filename: loopay-company-api-openapi.yml
  format: yaml
  label: Loopay Company API
  slug: loopay-company-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loopay/refs/heads/main/openapi/loopay-company-api-openapi.yml
- filename: loopay-companyproduct-api-openapi.yml
  format: yaml
  label: Loopay CompanyProduct API
  slug: loopay-companyproduct-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loopay/refs/heads/main/openapi/loopay-companyproduct-api-openapi.yml
- filename: loopay-country-api-openapi.yml
  format: yaml
  label: Loopay Country API
  slug: loopay-country-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loopay/refs/heads/main/openapi/loopay-country-api-openapi.yml
- filename: loopay-currency-api-openapi.yml
  format: yaml
  label: Loopay Currency API
  slug: loopay-currency-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loopay/refs/heads/main/openapi/loopay-currency-api-openapi.yml
- filename: loopay-documenttype-api-openapi.yml
  format: yaml
  label: Loopay DocumentType API
  slug: loopay-documenttype-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loopay/refs/heads/main/openapi/loopay-documenttype-api-openapi.yml
- filename: loopay-movements-api-openapi.yml
  format: yaml
  label: Loopay Movements API
  slug: loopay-movements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loopay/refs/heads/main/openapi/loopay-movements-api-openapi.yml
- filename: loopay-paidmethods-api-openapi.yml
  format: yaml
  label: Loopay PaidMethods API
  slug: loopay-paidmethods-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loopay/refs/heads/main/openapi/loopay-paidmethods-api-openapi.yml
- filename: loopay-payin-api-openapi.yml
  format: yaml
  label: Loopay PayIn API
  slug: loopay-payin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loopay/refs/heads/main/openapi/loopay-payin-api-openapi.yml
- filename: loopay-payout-api-openapi.yml
  format: yaml
  label: Loopay Payout API
  slug: loopay-payout-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loopay/refs/heads/main/openapi/loopay-payout-api-openapi.yml
- filename: loopay-physicalpoint-api-openapi.yml
  format: yaml
  label: Loopay PhysicalPoint API
  slug: loopay-physicalpoint-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loopay/refs/heads/main/openapi/loopay-physicalpoint-api-openapi.yml
- filename: loopay-sourcesofpayment-api-openapi.yml
  format: yaml
  label: Loopay SourcesOfPayment API
  slug: loopay-sourcesofpayment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loopay/refs/heads/main/openapi/loopay-sourcesofpayment-api-openapi.yml
- filename: loopay-sourcesofpaymentadmin-api-openapi.yml
  format: yaml
  label: Loopay SourcesOfPaymentAdmin API
  slug: loopay-sourcesofpaymentadmin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loopay/refs/heads/main/openapi/loopay-sourcesofpaymentadmin-api-openapi.yml
- filename: loopay-user-api-openapi.yml
  format: yaml
  label: Loopay User API
  slug: loopay-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loopay/refs/heads/main/openapi/loopay-user-api-openapi.yml
auth_types:
- token
description: ''
kind: authentication
layout: security
method: searched
name: Loopay Authentication
name_suffix: Authentication
oauth_flows: []
overview: Loopay secures its APIs with token across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Loopay
provider_slug: loopay
scheme_count: 1
schemes:
- documented_only: true
  name: bearerToken
  obtained_via: POST /login (User.login)
  scheme: bearer
  sources:
  - openapi/loopay-openapi-original.json
  - https://api.loopay.com/openapi.json
  type: http
slug: loopay-authentication
source_filename: loopay-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://api.loopay.com/openapi.json (info.description auth guide) + https://api.loopay.com/explorer\ndocs: https://api.loopay.com/explorer/#/User/User.login\nsummary:\n  types: [token]\n  api_key_in: [header]\n  oauth2_flows: []\n  notes: >-\n    Loopay uses a token-based authentication system. A bearer token is minted by\n    POSTing credentials to /login (operationId User.login); the token is then sent\n    on subsequent requests. The OpenAPI ships an empty components.securitySchemes\n    block, so the scheme is documented in prose (info.description) rather than\n    declared machine-readably — a gap worth filing with the provider.\nschemes:\n  - name: bearerToken\n    type: http\n    scheme: bearer\n    documented_only: true\n    obtained_via: POST /login (User.login)\n    sources: [openapi/loopay-openapi-original.json, https://api.loopay.com/openapi.json]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/loopay/refs/heads/main/authentication/loopay-authentication.yml
summary_line: token · 1 scheme
tags:
- Company
- Payments
- Fintech
- Banking as a Service
- Cross-Border Payments
- Payouts
- Treasury
- Latin America
---
