---
api_key_in:
- header
api_specs:
- filename: ravelin-3d-secure-api-openapi.yml
  format: yaml
  label: Ravelin 3D Secure API
  slug: ravelin-3d-secure-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ravelin/refs/heads/main/openapi/ravelin-3d-secure-api-openapi.yml
- filename: ravelin-authentication-api-openapi.yml
  format: yaml
  label: Ravelin Authentication API
  slug: ravelin-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ravelin/refs/heads/main/openapi/ravelin-authentication-api-openapi.yml
- filename: ravelin-checkout-api-openapi.yml
  format: yaml
  label: Ravelin Checkout API
  slug: ravelin-checkout-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ravelin/refs/heads/main/openapi/ravelin-checkout-api-openapi.yml
- filename: ravelin-connect-api-openapi.yml
  format: yaml
  label: Ravelin Connect API
  slug: ravelin-connect-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ravelin/refs/heads/main/openapi/ravelin-connect-api-openapi.yml
- filename: ravelin-customer-api-openapi.yml
  format: yaml
  label: Ravelin Customer API
  slug: ravelin-customer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ravelin/refs/heads/main/openapi/ravelin-customer-api-openapi.yml
- filename: ravelin-disputes-api-openapi.yml
  format: yaml
  label: Ravelin Disputes API
  slug: ravelin-disputes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ravelin/refs/heads/main/openapi/ravelin-disputes-api-openapi.yml
- filename: ravelin-payouts-api-openapi.yml
  format: yaml
  label: Ravelin Payouts API
  slug: ravelin-payouts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ravelin/refs/heads/main/openapi/ravelin-payouts-api-openapi.yml
- filename: ravelin-refunds-api-openapi.yml
  format: yaml
  label: Ravelin Refunds API
  slug: ravelin-refunds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ravelin/refs/heads/main/openapi/ravelin-refunds-api-openapi.yml
- filename: ravelin-supplier-api-openapi.yml
  format: yaml
  label: Ravelin Supplier API
  slug: ravelin-supplier-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ravelin/refs/heads/main/openapi/ravelin-supplier-api-openapi.yml
- filename: ravelin-transactions-api-openapi.yml
  format: yaml
  label: Ravelin Transactions API
  slug: ravelin-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ravelin/refs/heads/main/openapi/ravelin-transactions-api-openapi.yml
- filename: ravelin-vouchers-api-openapi.yml
  format: yaml
  label: Ravelin Vouchers API
  slug: ravelin-vouchers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ravelin/refs/heads/main/openapi/ravelin-vouchers-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Ravelin Authentication
name_suffix: Authentication
oauth_flows: []
overview: Ravelin secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Ravelin
provider_slug: ravelin
scheme_count: 1
schemes:
- description: Secret API key prefixed with `token`.
  in: header
  name: secretApiKey
  parameter: Authorization
  sources:
  - openapi/ravelin-3ds-server-api-openapi.yml
  - openapi/ravelin-merchant-api-openapi.yml
  type: apiKey
slug: ravelin-authentication
source_filename: ravelin-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/ravelin-3ds-server-api-openapi.yml, openapi/ravelin-merchant-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: secretApiKey\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Secret API key prefixed with `token`.\n  sources:\n  - openapi/ravelin-3ds-server-api-openapi.yml\n  - openapi/ravelin-merchant-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ravelin/refs/heads/main/authentication/ravelin-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Fraud Prevention
- Fraud Detection
- Chargeback Prevention
- Account Takeover
- 3D Secure
- Risk Scoring
- Payments
- Machine-Learning
---
