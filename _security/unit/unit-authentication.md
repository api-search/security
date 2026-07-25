---
api_key_in: []
api_specs:
- filename: unit-applications-openapi.json
  format: json
  label: Unit Applications API
  slug: applications
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unit/refs/heads/main/openapi/unit-applications-openapi.json
- filename: unit-customers-openapi.json
  format: json
  label: Unit Customers API
  slug: customers
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unit/refs/heads/main/openapi/unit-customers-openapi.json
- filename: unit-accounts-openapi.json
  format: json
  label: Unit Accounts API
  slug: accounts
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unit/refs/heads/main/openapi/unit-accounts-openapi.json
- filename: unit-cards-openapi.json
  format: json
  label: Unit Cards API
  slug: cards
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unit/refs/heads/main/openapi/unit-cards-openapi.json
- filename: unit-payments-openapi.json
  format: json
  label: Unit Payments API
  slug: payments
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unit/refs/heads/main/openapi/unit-payments-openapi.json
- filename: unit-checks-openapi.json
  format: json
  label: Unit Checks API
  slug: checks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unit/refs/heads/main/openapi/unit-checks-openapi.json
- filename: unit-authorizations-openapi.json
  format: json
  label: Unit Card Authorizations API
  slug: authorizations
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unit/refs/heads/main/openapi/unit-authorizations-openapi.json
- filename: unit-disputes-openapi.json
  format: json
  label: Unit Disputes API
  slug: disputes
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unit/refs/heads/main/openapi/unit-disputes-openapi.json
- filename: unit-transactions-openapi.json
  format: json
  label: Unit Transactions API
  slug: transactions
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unit/refs/heads/main/openapi/unit-transactions-openapi.json
- filename: unit-statements-openapi.json
  format: json
  label: Unit Statements API
  slug: statements
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unit/refs/heads/main/openapi/unit-statements-openapi.json
- filename: unit-tax-forms-openapi.json
  format: json
  label: Unit Tax Forms API
  slug: tax-forms
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unit/refs/heads/main/openapi/unit-tax-forms-openapi.json
- filename: unit-fees-rewards-openapi.json
  format: json
  label: Unit Fees and Rewards API
  slug: fees-rewards
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unit/refs/heads/main/openapi/unit-fees-rewards-openapi.json
- filename: unit-credit-openapi.json
  format: json
  label: Unit Credit and Repayments API
  slug: credit
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unit/refs/heads/main/openapi/unit-credit-openapi.json
- filename: unit-stop-payments-openapi.json
  format: json
  label: Unit Stop Payments API
  slug: stop-payments
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unit/refs/heads/main/openapi/unit-stop-payments-openapi.json
- filename: unit-webhooks-openapi.json
  format: json
  label: Unit Webhooks and Events API
  slug: webhooks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unit/refs/heads/main/openapi/unit-webhooks-openapi.json
- filename: unit-sandbox-openapi.json
  format: json
  label: Unit Sandbox and Reference API
  slug: sandbox
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unit/refs/heads/main/openapi/unit-sandbox-openapi.json
auth_types:
- http
- oauth2-bearer
description: ''
kind: authentication
layout: security
method: searched
name: Unit Authentication
name_suffix: Authentication
oauth_flows: []
overview: Unit secures its APIs with http and oauth2-bearer across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Unit
provider_slug: unit
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/unit-openapi-source.json
  type: http
slug: unit-authentication
source_filename: unit-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-23'\nmethod: searched\nsource: openapi/ securitySchemes + https://www.unit.co/docs/api/using-the-api\ndocs: https://www.unit.co/docs/api/using-the-api#authentication\nsummary:\n  types: [http, oauth2-bearer]\n  scheme: bearer\n  bearer_format: JWT (PASETO v2.public tokens)\n  token_types: [org, customer, cardholder]\n  scopes: true\n  two_factor: true\noverview: >-\n  Unit's API uses OAuth 2.0 Bearer tokens. Every request must carry an\n  Authorization: Bearer <token> header; an invalid, missing, or expired token\n  returns HTTP 401 Unauthorized. Tokens are issued with a set of scopes (see\n  scopes/unit-scopes.yml) that define per-resource read/write access. The OpenAPI\n  declares this as an http bearer (JWT) scheme; the token/scope/2FA model is\n  documented in the Using the API guide.\ntoken_types:\n  - name: Org API token\n    role: org\n    description: Broad system-level token, not restricted to a specific end customer. Can be used without 2FA for\
  \ sensitive server-side operations.\n    docs: https://www.unit.co/docs/api/org-api-tokens\n  - name: Customer token\n    role: customer\n    description: >-\n      Short-lived, end-customer-scoped bearer token with built-in OTP Two-Factor\n      Authentication and a customizable expiry up to 24 hours. Recommended default\n      for all end-customer actions and required for PCI-sensitive card data.\n    docs: https://www.unit.co/docs/api/customer-api-tokens\n    created_via:\n      - createCustomerTokenVerification  # POST /customers/{customerId}/token/verification\n      - createCustomerToken              # POST /customers/{customerId}/token\n    custom_authentication: https://www.unit.co/docs/custom-authentication\n  - name: Cardholder token\n    role: cardholder\n    description: Single-card-scoped token granting a non-account-holder user sensitive card actions (view card details, manage PIN) after an OTP verification.\n    docs: https://www.unit.co/docs/api/card-holder-api-tokens/overview\n\
  two_factor:\n  required_for:\n    - Applications (customer phone verified via OTP before submission)\n    - Sensitive (fund-movement) scopes — 2FA within the prior 24 hours\n    - PCI-sensitive card data and actions (requires a Customer token)\n  methods: [OTP via SMS or call, biometric, other industry-recognized methods]\n  validity: A successful 2FA is valid for up to 24 hours.\n  identity_endpoint: GET /identity  # returns decoded token info\nschemes:\n  - name: bearerAuth\n    type: http\n    scheme: bearer\n    bearerFormat: JWT\n    sources: [openapi/unit-openapi-source.json]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/unit/refs/heads/main/authentication/unit-authentication.yml
summary_line: http/oauth2-bearer · 1 scheme
tags:
- FinTech
- BaaS
- Banking
- Payments
- Card Issuing
- ACH
- United States
- Embedded Finance
- Deposit Accounts
- Open Finance
---
