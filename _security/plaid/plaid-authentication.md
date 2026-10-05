---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: plaid-plaid-api-openapi.yml
  format: yaml
  label: Plaid API
  slug: plaid-plaid-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plaid/refs/heads/main/openapi/plaid-plaid-api-openapi.yml
- filename: plaid-account-information-api-openapi.yml
  format: yaml
  label: Plaid Account Information API
  slug: plaid-account-information-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plaid/refs/heads/main/openapi/plaid-account-information-api-openapi.yml
- filename: plaid-account-statements-api-openapi.yml
  format: yaml
  label: Plaid Account Statements API
  slug: plaid-account-statements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plaid/refs/heads/main/openapi/plaid-account-statements-api-openapi.yml
- filename: plaid-account-transactions-api-openapi.yml
  format: yaml
  label: Plaid Account Transactions API
  slug: plaid-account-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plaid/refs/heads/main/openapi/plaid-account-transactions-api-openapi.yml
- filename: plaid-asset-transfer-networks-information-api-openapi.yml
  format: yaml
  label: Plaid Asset Transfer Networks Information API
  slug: plaid-asset-transfer-networks-information-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plaid/refs/heads/main/openapi/plaid-asset-transfer-networks-information-api-openapi.yml
- filename: plaid-payment-networks-information-api-openapi.yml
  format: yaml
  label: Plaid Payment Networks Information API
  slug: plaid-payment-networks-information-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plaid/refs/heads/main/openapi/plaid-payment-networks-information-api-openapi.yml
- filename: plaid-personal-information-api-openapi.yml
  format: yaml
  label: Plaid Personal Information API
  slug: plaid-personal-information-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plaid/refs/heads/main/openapi/plaid-personal-information-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: derived
name: Plaid Authentication
name_suffix: Authentication
oauth_flows: []
overview: Plaid secures its APIs with apiKey across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Plaid
provider_slug: plaid
scheme_count: 3
schemes:
- in: header
  name: clientId
  parameter: PLAID-CLIENT-ID
  sources:
  - openapi/plaid-openapi-original.yml
  type: apiKey
- in: header
  name: secret
  parameter: PLAID-SECRET
  sources:
  - openapi/plaid-openapi-original.yml
  type: apiKey
- in: header
  name: plaidVersion
  parameter: Plaid-Version
  sources:
  - openapi/plaid-openapi-original.yml
  type: apiKey
slug: plaid-authentication
source_filename: plaid-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/plaid-openapi-original.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: clientId\n  type: apiKey\n  in: header\n  parameter: PLAID-CLIENT-ID\n  sources:\n  - openapi/plaid-openapi-original.yml\n- name: secret\n  type: apiKey\n  in: header\n  parameter: PLAID-SECRET\n  sources:\n  - openapi/plaid-openapi-original.yml\n- name: plaidVersion\n  type: apiKey\n  in: header\n  parameter: Plaid-Version\n  sources:\n  - openapi/plaid-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/plaid/refs/heads/main/authentication/plaid-authentication.yml
summary_line: apiKey · 3 schemes
tags:
- Finance
- Fintech
- Open Banking
- Bank Accounts
- Data Aggregation
- Payments
- United States
---
