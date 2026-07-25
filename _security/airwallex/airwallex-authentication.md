---
api_key_in:
- header
api_specs:
- filename: airwallex-authentication-api-openapi.yml
  format: yaml
  label: Airwallex Authentication API
  slug: airwallex-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airwallex/refs/heads/main/openapi/airwallex-authentication-api-openapi.yml
- filename: airwallex-balances-api-openapi.yml
  format: yaml
  label: Airwallex Balances API
  slug: airwallex-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airwallex/refs/heads/main/openapi/airwallex-balances-api-openapi.yml
- filename: airwallex-beneficiaries-api-openapi.yml
  format: yaml
  label: Airwallex Beneficiaries API
  slug: airwallex-beneficiaries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airwallex/refs/heads/main/openapi/airwallex-beneficiaries-api-openapi.yml
- filename: airwallex-customers-api-openapi.yml
  format: yaml
  label: Airwallex Customers API
  slug: airwallex-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airwallex/refs/heads/main/openapi/airwallex-customers-api-openapi.yml
- filename: airwallex-payment-intents-api-openapi.yml
  format: yaml
  label: Airwallex Payment Intents API
  slug: airwallex-payment-intents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airwallex/refs/heads/main/openapi/airwallex-payment-intents-api-openapi.yml
- filename: airwallex-payouts-api-openapi.yml
  format: yaml
  label: Airwallex Payouts API
  slug: airwallex-payouts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airwallex/refs/heads/main/openapi/airwallex-payouts-api-openapi.yml
- filename: airwallex-refunds-api-openapi.yml
  format: yaml
  label: Airwallex Refunds API
  slug: airwallex-refunds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airwallex/refs/heads/main/openapi/airwallex-refunds-api-openapi.yml
- filename: airwallex-transfers-api-openapi.yml
  format: yaml
  label: Airwallex Transfers API
  slug: airwallex-transfers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airwallex/refs/heads/main/openapi/airwallex-transfers-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Airwallex Authentication
name_suffix: Authentication
oauth_flows: []
overview: Airwallex secures its APIs with apiKey and http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Airwallex
provider_slug: airwallex
scheme_count: 3
schemes:
- description: 'Bearer access token obtained via POST /api/v1/authentication/login using

    `x-client-id` and `x-api-key` request headers.'
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/airwallex-openapi.yml
  type: http
- in: header
  name: ClientIdHeader
  parameter: x-client-id
  sources:
  - openapi/airwallex-openapi.yml
  type: apiKey
- in: header
  name: ApiKeyHeader
  parameter: x-api-key
  sources:
  - openapi/airwallex-openapi.yml
  type: apiKey
slug: airwallex-authentication
source_filename: airwallex-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/airwallex-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: |-\n    Bearer access token obtained via POST /api/v1/authentication/login using\n    `x-client-id` and `x-api-key` request headers.\n  sources:\n  - openapi/airwallex-openapi.yml\n- name: ClientIdHeader\n  type: apiKey\n  in: header\n  parameter: x-client-id\n  sources:\n  - openapi/airwallex-openapi.yml\n- name: ApiKeyHeader\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  sources:\n  - openapi/airwallex-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/airwallex/refs/heads/main/authentication/airwallex-authentication.yml
summary_line: apiKey/http · 3 schemes
tags:
- Cross-Border Payments
- FinTech
- Foreign Exchange
- Payments
- Global
- Embedded Finance
- Multi-Currency
---
