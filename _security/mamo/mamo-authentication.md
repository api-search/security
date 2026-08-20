---
api_key_in: []
api_specs:
- filename: mamo-business-details-api-openapi.yml
  format: yaml
  label: Mamo Business Details API
  slug: mamo-business-details-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mamo/refs/heads/main/openapi/mamo-business-details-api-openapi.yml
- filename: mamo-cards-api-openapi.yml
  format: yaml
  label: Mamo Cards API
  slug: mamo-cards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mamo/refs/heads/main/openapi/mamo-cards-api-openapi.yml
- filename: mamo-expenses-api-openapi.yml
  format: yaml
  label: Mamo Expenses API
  slug: mamo-expenses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mamo/refs/heads/main/openapi/mamo-expenses-api-openapi.yml
- filename: mamo-getting-started-api-openapi.yml
  format: yaml
  label: Mamo Getting Started API
  slug: mamo-getting-started-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mamo/refs/heads/main/openapi/mamo-getting-started-api-openapi.yml
- filename: mamo-invoices-api-openapi.yml
  format: yaml
  label: Mamo Invoices API
  slug: mamo-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mamo/refs/heads/main/openapi/mamo-invoices-api-openapi.yml
- filename: mamo-payment-links-api-openapi.yml
  format: yaml
  label: Mamo Payment Links API
  slug: mamo-payment-links-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mamo/refs/heads/main/openapi/mamo-payment-links-api-openapi.yml
- filename: mamo-payouts-api-openapi.yml
  format: yaml
  label: Mamo Payouts API
  slug: mamo-payouts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mamo/refs/heads/main/openapi/mamo-payouts-api-openapi.yml
- filename: mamo-receipts-api-openapi.yml
  format: yaml
  label: Mamo Receipts API
  slug: mamo-receipts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mamo/refs/heads/main/openapi/mamo-receipts-api-openapi.yml
- filename: mamo-recipients-api-openapi.yml
  format: yaml
  label: Mamo Recipients API
  slug: mamo-recipients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mamo/refs/heads/main/openapi/mamo-recipients-api-openapi.yml
- filename: mamo-subscriptions-api-openapi.yml
  format: yaml
  label: Mamo Subscriptions API
  slug: mamo-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mamo/refs/heads/main/openapi/mamo-subscriptions-api-openapi.yml
- filename: mamo-transactions-api-openapi.yml
  format: yaml
  label: Mamo Transactions API
  slug: mamo-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mamo/refs/heads/main/openapi/mamo-transactions-api-openapi.yml
- filename: mamo-webhooks-api-openapi.yml
  format: yaml
  label: Mamo Webhooks API
  slug: mamo-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mamo/refs/heads/main/openapi/mamo-webhooks-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Mamo Authentication
name_suffix: Authentication
oauth_flows: []
overview: Mamo secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Mamo
provider_slug: mamo
scheme_count: 1
schemes:
- description: 'API key from the Mamo dashboard (Developer > Keys), passed as `Authorization: Bearer <api_key>`.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/mamo-openapi.yml
  type: http
slug: mamo-authentication
source_filename: mamo-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: derived\nsource: openapi/mamo-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'API key from the Mamo dashboard (Developer > Keys), passed as `Authorization:\n    Bearer <api_key>`.'\n  sources:\n  - openapi/mamo-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mamo/refs/heads/main/authentication/mamo-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Payments
- Fintech
- Payment Links
- Subscription
- Corporate Cards
- Payouts
- Expense Management
- UAE
- Middle East
---
