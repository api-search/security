---
api_key_in:
- header
api_specs:
- filename: ansa-add-incentive-api-openapi.yml
  format: yaml
  label: Ansa Add Incentive API
  slug: ansa-add-incentive-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ansa/refs/heads/main/openapi/ansa-add-incentive-api-openapi.yml
- filename: ansa-customer-segments-api-openapi.yml
  format: yaml
  label: Ansa Customer Segments API
  slug: ansa-customer-segments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ansa/refs/heads/main/openapi/ansa-customer-segments-api-openapi.yml
- filename: ansa-customers-api-openapi.yml
  format: yaml
  label: Ansa Customers API
  slug: ansa-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ansa/refs/heads/main/openapi/ansa-customers-api-openapi.yml
- filename: ansa-initialize-payment-session-api-openapi.yml
  format: yaml
  label: Ansa Initialize Payment Session API
  slug: ansa-initialize-payment-session-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ansa/refs/heads/main/openapi/ansa-initialize-payment-session-api-openapi.yml
- filename: ansa-merchants-api-openapi.yml
  format: yaml
  label: Ansa Merchants API
  slug: ansa-merchants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ansa/refs/heads/main/openapi/ansa-merchants-api-openapi.yml
- filename: ansa-refunds-api-openapi.yml
  format: yaml
  label: Ansa Refunds API
  slug: ansa-refunds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ansa/refs/heads/main/openapi/ansa-refunds-api-openapi.yml
- filename: ansa-transactions-api-openapi.yml
  format: yaml
  label: Ansa Transactions API
  slug: ansa-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ansa/refs/heads/main/openapi/ansa-transactions-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Ansa Authentication
name_suffix: Authentication
oauth_flows: []
overview: Ansa secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Ansa
provider_slug: ansa
scheme_count: 1
schemes:
- description: API key in the Authorization header. Keys are prefixed ansa_sk_live_/ansa_sk_sandbox_ (merchant secret), ansa_cs_live_/ansa_cs_sandbox_ (client secret).
  in: header
  name: sec0
  parameter: Authorization
  sources:
  - openapi/ansa-openapi-original.yml
  type: apiKey
slug: ansa-authentication
source_filename: ansa-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: derived\nsource: openapi/ansa-openapi-original.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: sec0\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: API key in the Authorization header. Keys are prefixed ansa_sk_live_/ansa_sk_sandbox_\n    (merchant secret), ansa_cs_live_/ansa_cs_sandbox_ (client secret).\n  sources:\n  - openapi/ansa-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ansa/refs/heads/main/authentication/ansa-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Fintech
- Payments
- Stored Value
- Digital Wallet
- Loyalty
- Incentives
- API
---
