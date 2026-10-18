---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: bond-cards-api-openapi.yml
  format: yaml
  label: Bond Cards API
  slug: bond-cards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bond/refs/heads/main/openapi/bond-cards-api-openapi.yml
- filename: bond-credit-api-openapi.yml
  format: yaml
  label: Bond Credit API
  slug: bond-credit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bond/refs/heads/main/openapi/bond-credit-api-openapi.yml
- filename: bond-webhooks-api-openapi.yml
  format: yaml
  label: Bond Webhooks API
  slug: bond-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bond/refs/heads/main/openapi/bond-webhooks-api-openapi.yml
- filename: bond-accounts-api-openapi.yml
  format: yaml
  label: Bond Accounts API
  slug: bond-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bond/refs/heads/main/openapi/bond-accounts-api-openapi.yml
- filename: bond-beneficial-owners-address-api-openapi.yml
  format: yaml
  label: Bond Beneficial owners address API
  slug: bond-beneficial-owners-address-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bond/refs/heads/main/openapi/bond-beneficial-owners-address-api-openapi.yml
- filename: bond-beneficial-owners-api-openapi.yml
  format: yaml
  label: Bond Beneficial owners API
  slug: bond-beneficial-owners-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bond/refs/heads/main/openapi/bond-beneficial-owners-api-openapi.yml
- filename: bond-business-address-api-openapi.yml
  format: yaml
  label: Bond Business address API
  slug: bond-business-address-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bond/refs/heads/main/openapi/bond-business-address-api-openapi.yml
- filename: bond-businesses-api-openapi.yml
  format: yaml
  label: Bond Businesses API
  slug: bond-businesses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bond/refs/heads/main/openapi/bond-businesses-api-openapi.yml
- filename: bond-card-restrictions-api-openapi.yml
  format: yaml
  label: Bond Card restrictions API
  slug: bond-card-restrictions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bond/refs/heads/main/openapi/bond-card-restrictions-api-openapi.yml
- filename: bond-cards-api-openapi.yml
  format: yaml
  label: Bond Cards API
  slug: bond-cards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bond/refs/heads/main/openapi/bond-cards-api-openapi.yml
- filename: bond-credit-api-openapi.yml
  format: yaml
  label: Bond Credit API
  slug: bond-credit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bond/refs/heads/main/openapi/bond-credit-api-openapi.yml
- filename: bond-customers-api-openapi.yml
  format: yaml
  label: Bond Customers API
  slug: bond-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bond/refs/heads/main/openapi/bond-customers-api-openapi.yml
- filename: bond-kyb-api-openapi.yml
  format: yaml
  label: Bond KYB API
  slug: bond-kyb-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bond/refs/heads/main/openapi/bond-kyb-api-openapi.yml
- filename: bond-kyc-api-openapi.yml
  format: yaml
  label: Bond KYC API
  slug: bond-kyc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bond/refs/heads/main/openapi/bond-kyc-api-openapi.yml
- filename: bond-simulate-api-openapi.yml
  format: yaml
  label: Bond Simulate API
  slug: bond-simulate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bond/refs/heads/main/openapi/bond-simulate-api-openapi.yml
- filename: bond-statements-api-openapi.yml
  format: yaml
  label: Bond Statements API
  slug: bond-statements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bond/refs/heads/main/openapi/bond-statements-api-openapi.yml
- filename: bond-transactions-api-openapi.yml
  format: yaml
  label: Bond Transactions API
  slug: bond-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bond/refs/heads/main/openapi/bond-transactions-api-openapi.yml
- filename: bond-transfer-api-openapi.yml
  format: yaml
  label: Bond Transfer API
  slug: bond-transfer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bond/refs/heads/main/openapi/bond-transfer-api-openapi.yml
- filename: bond-webhooks-api-openapi.yml
  format: yaml
  label: Bond Webhooks API
  slug: bond-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bond/refs/heads/main/openapi/bond-webhooks-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Bond Authentication
name_suffix: Authentication
oauth_flows: []
overview: Bond secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Bond
provider_slug: bond
scheme_count: 2
schemes:
- description: The Identity portion of the Bond API key (e.g. a UUID). Sent on every request alongside the Authorization header.
  in: header
  name: Identity
  parameter: Identity
  sources:
  - https://docs.bond.tech/reference/authentication
  type: apiKey
- description: The secret Authorization portion of the Bond API key. Sent on every request alongside the Identity header.
  in: header
  name: Authorization
  parameter: Authorization
  sources:
  - https://docs.bond.tech/reference/authentication
  type: apiKey
slug: bond-authentication
source_filename: bond-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://docs.bond.tech/reference/authentication\ndocs: https://docs.bond.tech/reference/authentication\nsummary:\n  types: [apiKey]\n  api_key_in: [header]\n  oauth2_flows: []\n  note: >-\n    Bond uses a two-part API key: an Identity value and an Authorization value,\n    both sent as request headers. The key identifies the Bond account (brand),\n    not an individual team member. Keys are created and managed in the Bond Portal.\nschemes:\n  - name: Identity\n    type: apiKey\n    in: header\n    parameter: Identity\n    description: >-\n      The Identity portion of the Bond API key (e.g. a UUID). Sent on every\n      request alongside the Authorization header.\n    sources: [https://docs.bond.tech/reference/authentication]\n  - name: Authorization\n    type: apiKey\n    in: header\n    parameter: Authorization\n    description: >-\n      The secret Authorization portion of the Bond API key. Sent on every request\n      alongside\
  \ the Identity header.\n    sources: [https://docs.bond.tech/reference/authentication]\nrequired_headers:\n  - name: Identity\n    required: true\n  - name: Authorization\n    required: true\n  - name: content-type\n    required: true\n    values: application/json\n    applies_to: [POST, PATCH, DELETE]\nkey_management:\n  portal: https://portal.bond.tech\n  notes: >-\n    An account may hold any number of API keys. All keys currently grant access\n    to every endpoint on the platform. Separate keys exist per environment\n    (sandbox vs production).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bond/refs/heads/main/authentication/bond-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Company
- United States
- Banking as a Service
- Embedded Finance
- Fintech
- Payments
- Card Issuing
- Deposit Accounts
- Money Movement
- ACH
- KYC
- KYB
- Credit
- Open Finance
---
