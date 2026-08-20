---
api_key_in: []
api_specs:
- filename: openpay-bankaccounts-api-openapi.yml
  format: yaml
  label: Openpay BankAccounts API
  slug: openpay-bankaccounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openpay/refs/heads/main/openapi/openpay-bankaccounts-api-openapi.yml
- filename: openpay-cards-api-openapi.yml
  format: yaml
  label: Openpay Cards API
  slug: openpay-cards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openpay/refs/heads/main/openapi/openpay-cards-api-openapi.yml
- filename: openpay-charges-api-openapi.yml
  format: yaml
  label: Openpay Charges API
  slug: openpay-charges-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openpay/refs/heads/main/openapi/openpay-charges-api-openapi.yml
- filename: openpay-customers-api-openapi.yml
  format: yaml
  label: Openpay Customers API
  slug: openpay-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openpay/refs/heads/main/openapi/openpay-customers-api-openapi.yml
- filename: openpay-fees-api-openapi.yml
  format: yaml
  label: Openpay Fees API
  slug: openpay-fees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openpay/refs/heads/main/openapi/openpay-fees-api-openapi.yml
- filename: openpay-payouts-api-openapi.yml
  format: yaml
  label: Openpay Payouts API
  slug: openpay-payouts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openpay/refs/heads/main/openapi/openpay-payouts-api-openapi.yml
- filename: openpay-plans-api-openapi.yml
  format: yaml
  label: Openpay Plans API
  slug: openpay-plans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openpay/refs/heads/main/openapi/openpay-plans-api-openapi.yml
- filename: openpay-subscriptions-api-openapi.yml
  format: yaml
  label: Openpay Subscriptions API
  slug: openpay-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openpay/refs/heads/main/openapi/openpay-subscriptions-api-openapi.yml
- filename: openpay-tokens-api-openapi.yml
  format: yaml
  label: Openpay Tokens API
  slug: openpay-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openpay/refs/heads/main/openapi/openpay-tokens-api-openapi.yml
- filename: openpay-transfers-api-openapi.yml
  format: yaml
  label: Openpay Transfers API
  slug: openpay-transfers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openpay/refs/heads/main/openapi/openpay-transfers-api-openapi.yml
- filename: openpay-webhooks-api-openapi.yml
  format: yaml
  label: Openpay Webhooks API
  slug: openpay-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openpay/refs/heads/main/openapi/openpay-webhooks-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Openpay Authentication
name_suffix: Authentication
oauth_flows: []
overview: Openpay secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Openpay
provider_slug: openpay
scheme_count: 1
schemes:
- description: HTTP Basic authentication. Use the merchant private API key as the username and leave the password empty.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/openpay-openapi.yml
  type: http
slug: openpay-authentication
source_filename: openpay-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/openpay-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic authentication. Use the merchant private API key as the username and\n    leave the password empty.\n  sources:\n  - openapi/openpay-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/openpay/refs/heads/main/authentication/openpay-authentication.yml
summary_line: http · 1 scheme
tags:
- Payments
- Fintech
- Cards
- SPEI
- Subscription
---
