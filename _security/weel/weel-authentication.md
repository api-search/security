---
api_key_in: []
api_specs:
- filename: weel-accounting-codes-api-openapi.yml
  format: yaml
  label: Weel Accounting Codes API
  slug: weel-accounting-codes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weel/refs/heads/main/openapi/weel-accounting-codes-api-openapi.yml
- filename: weel-budget-members-api-openapi.yml
  format: yaml
  label: Weel Budget Members API
  slug: weel-budget-members-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weel/refs/heads/main/openapi/weel-budget-members-api-openapi.yml
- filename: weel-budget-owners-api-openapi.yml
  format: yaml
  label: Weel Budget Owners API
  slug: weel-budget-owners-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weel/refs/heads/main/openapi/weel-budget-owners-api-openapi.yml
- filename: weel-budget-topups-api-openapi.yml
  format: yaml
  label: Weel Budget Topups API
  slug: weel-budget-topups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weel/refs/heads/main/openapi/weel-budget-topups-api-openapi.yml
- filename: weel-budgets-api-openapi.yml
  format: yaml
  label: Weel Budgets API
  slug: weel-budgets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weel/refs/heads/main/openapi/weel-budgets-api-openapi.yml
- filename: weel-categories-api-openapi.yml
  format: yaml
  label: Weel Categories API
  slug: weel-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weel/refs/heads/main/openapi/weel-categories-api-openapi.yml
- filename: weel-custom-field-budgets-api-openapi.yml
  format: yaml
  label: Weel Custom Field Budgets API
  slug: weel-custom-field-budgets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weel/refs/heads/main/openapi/weel-custom-field-budgets-api-openapi.yml
- filename: weel-custom-field-options-api-openapi.yml
  format: yaml
  label: Weel Custom Field Options API
  slug: weel-custom-field-options-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weel/refs/heads/main/openapi/weel-custom-field-options-api-openapi.yml
- filename: weel-custom-fields-api-openapi.yml
  format: yaml
  label: Weel Custom Fields API
  slug: weel-custom-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weel/refs/heads/main/openapi/weel-custom-fields-api-openapi.yml
- filename: weel-invites-api-openapi.yml
  format: yaml
  label: Weel Invites API
  slug: weel-invites-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weel/refs/heads/main/openapi/weel-invites-api-openapi.yml
- filename: weel-roles-api-openapi.yml
  format: yaml
  label: Weel Roles API
  slug: weel-roles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weel/refs/heads/main/openapi/weel-roles-api-openapi.yml
- filename: weel-statements-api-openapi.yml
  format: yaml
  label: Weel Statements API
  slug: weel-statements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weel/refs/heads/main/openapi/weel-statements-api-openapi.yml
- filename: weel-tax-rates-api-openapi.yml
  format: yaml
  label: Weel Tax Rates API
  slug: weel-tax-rates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weel/refs/heads/main/openapi/weel-tax-rates-api-openapi.yml
- filename: weel-transactions-api-openapi.yml
  format: yaml
  label: Weel Transactions API
  slug: weel-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weel/refs/heads/main/openapi/weel-transactions-api-openapi.yml
- filename: weel-users-api-openapi.yml
  format: yaml
  label: Weel Users API
  slug: weel-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weel/refs/heads/main/openapi/weel-users-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Weel Authentication
name_suffix: Authentication
oauth_flows: []
overview: Weel secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Weel
provider_slug: weel
scheme_count: 1
schemes:
- name: BearerAuth
  scheme: bearer
  sources:
  - openapi/weel-openapi.yml
  type: http
slug: weel-authentication
source_filename: weel-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-24'\nmethod: searched\nsource: openapi/weel-openapi.yml\ndocs: https://developer.letsweel.com/getting-started/authentication\nsummary:\n  types:\n    - http\n  http_schemes:\n    - bearer\n  oauth2_flows: []\n  api_key_in: []\nschemes:\n  - name: BearerAuth\n    type: http\n    scheme: bearer\n    sources:\n      - openapi/weel-openapi.yml\ndetails:\n  token_type: API key (bearer)\n  header: 'Authorization: Bearer <token>'\n  creation: >-\n    Created in the Weel web app under Settings > API > Create New API Key\n    (https://app.letsweel.com/app/settings#api).\n  expiry: >-\n    Bearer tokens do not expire. They remain valid until revoked or replaced\n    (delete the token under Settings > API).\n  rotation: Manual — revoke and recreate in-app; no programmatic rotation endpoint.\n  oauth2: false\n  openid_connect: false\n  mtls: false\n  gating: API access is an Enterprise-plan capability.\nnotes: >-\n  Single security scheme across all operations: HTTP\
  \ bearer token. No OAuth2,\n  OpenID Connect, or mutual TLS is documented, and no OAuth/OIDC discovery\n  metadata is served — so there is no scope surface (hence no scopes/ artifact).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/weel/refs/heads/main/authentication/weel-authentication.yml
summary_line: http · 1 scheme
tags:
- Payments
- Australia
- Spend Management
- Expense Management
- Corporate Cards
- Accounts Payable
- Card Issuing
- Reimbursement
- Budgets
- Fintech
---
