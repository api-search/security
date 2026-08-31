---
api_key_in:
- header
api_specs:
- filename: rotessa-customers-api-openapi.yml
  format: yaml
  label: Rotessa Customers API
  slug: rotessa-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rotessa/refs/heads/main/openapi/rotessa-customers-api-openapi.yml
- filename: rotessa-transaction-schedules-api-openapi.yml
  format: yaml
  label: Rotessa Transaction Schedules API
  slug: rotessa-transaction-schedules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rotessa/refs/heads/main/openapi/rotessa-transaction-schedules-api-openapi.yml
- filename: rotessa-transaction-report-api-openapi.yml
  format: yaml
  label: Rotessa Transaction Report API
  slug: rotessa-transaction-report-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rotessa/refs/heads/main/openapi/rotessa-transaction-report-api-openapi.yml
- filename: rotessa-customers-api-openapi.yml
  format: yaml
  label: Rotessa Customers API
  slug: rotessa-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rotessa/refs/heads/main/openapi/rotessa-customers-api-openapi.yml
- filename: rotessa-transaction-report-api-openapi.yml
  format: yaml
  label: Rotessa Transaction Report API
  slug: rotessa-transaction-report-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rotessa/refs/heads/main/openapi/rotessa-transaction-report-api-openapi.yml
- filename: rotessa-transaction-schedules-api-openapi.yml
  format: yaml
  label: Rotessa Transaction Schedules API
  slug: rotessa-transaction-schedules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rotessa/refs/heads/main/openapi/rotessa-transaction-schedules-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Rotessa Authentication
name_suffix: Authentication
oauth_flows: []
overview: Rotessa secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Rotessa
provider_slug: rotessa
scheme_count: 1
schemes:
- description: 'API key placed in the Authorization header in the form `Authorization: Token token="<your_api_key>"`. Keys are created and revoked in the Rotessa admin portal.'
  in: header
  name: apiKeyAuth
  parameter: Authorization
  sources:
  - openapi/rotessa-openapi.yml
  type: apiKey
slug: rotessa-authentication
source_filename: rotessa-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-24'\nmethod: derived\nsource: openapi/rotessa-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: 'API key placed in the Authorization header in the form `Authorization: Token\n    token=\"<your_api_key>\"`. Keys are created and revoked in the Rotessa admin portal.'\n  sources:\n  - openapi/rotessa-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rotessa/refs/heads/main/authentication/rotessa-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Payments
- Canada
- Pre-Authorized Debit
- ACH
- Account-to-Account
- Bank Payments
- Recurring Payments
- Subscription
- Direct Debit
- Money Movement
- Open Banking
---
