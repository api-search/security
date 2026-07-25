---
api_key_in: []
api_specs:
- filename: gocardless-billing-request-flows-api-openapi.yml
  format: yaml
  label: GoCardless billing_request_flows API
  slug: gocardless-billing-request-flows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gocardless/refs/heads/main/openapi/gocardless-billing-request-flows-api-openapi.yml
- filename: gocardless-billing-requests-api-openapi.yml
  format: yaml
  label: GoCardless billing_requests API
  slug: gocardless-billing-requests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gocardless/refs/heads/main/openapi/gocardless-billing-requests-api-openapi.yml
- filename: gocardless-blocks-api-openapi.yml
  format: yaml
  label: GoCardless blocks API
  slug: gocardless-blocks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gocardless/refs/heads/main/openapi/gocardless-blocks-api-openapi.yml
- filename: gocardless-creditor-bank-accounts-api-openapi.yml
  format: yaml
  label: GoCardless creditor_bank_accounts API
  slug: gocardless-creditor-bank-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gocardless/refs/heads/main/openapi/gocardless-creditor-bank-accounts-api-openapi.yml
- filename: gocardless-creditors-api-openapi.yml
  format: yaml
  label: GoCardless creditors API
  slug: gocardless-creditors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gocardless/refs/heads/main/openapi/gocardless-creditors-api-openapi.yml
- filename: gocardless-customer-bank-accounts-api-openapi.yml
  format: yaml
  label: GoCardless customer_bank_accounts API
  slug: gocardless-customer-bank-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gocardless/refs/heads/main/openapi/gocardless-customer-bank-accounts-api-openapi.yml
- filename: gocardless-customers-api-openapi.yml
  format: yaml
  label: GoCardless customers API
  slug: gocardless-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gocardless/refs/heads/main/openapi/gocardless-customers-api-openapi.yml
- filename: gocardless-events-api-openapi.yml
  format: yaml
  label: GoCardless events API
  slug: gocardless-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gocardless/refs/heads/main/openapi/gocardless-events-api-openapi.yml
- filename: gocardless-instalment-schedules-api-openapi.yml
  format: yaml
  label: GoCardless instalment_schedules API
  slug: gocardless-instalment-schedules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gocardless/refs/heads/main/openapi/gocardless-instalment-schedules-api-openapi.yml
- filename: gocardless-institutions-api-openapi.yml
  format: yaml
  label: GoCardless institutions API
  slug: gocardless-institutions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gocardless/refs/heads/main/openapi/gocardless-institutions-api-openapi.yml
- filename: gocardless-mandates-api-openapi.yml
  format: yaml
  label: GoCardless mandates API
  slug: gocardless-mandates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gocardless/refs/heads/main/openapi/gocardless-mandates-api-openapi.yml
- filename: gocardless-payer-authorisations-api-openapi.yml
  format: yaml
  label: GoCardless payer_authorisations API
  slug: gocardless-payer-authorisations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gocardless/refs/heads/main/openapi/gocardless-payer-authorisations-api-openapi.yml
- filename: gocardless-payments-api-openapi.yml
  format: yaml
  label: GoCardless payments API
  slug: gocardless-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gocardless/refs/heads/main/openapi/gocardless-payments-api-openapi.yml
- filename: gocardless-payouts-api-openapi.yml
  format: yaml
  label: GoCardless payouts API
  slug: gocardless-payouts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gocardless/refs/heads/main/openapi/gocardless-payouts-api-openapi.yml
- filename: gocardless-refunds-api-openapi.yml
  format: yaml
  label: GoCardless refunds API
  slug: gocardless-refunds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gocardless/refs/heads/main/openapi/gocardless-refunds-api-openapi.yml
- filename: gocardless-subscriptions-api-openapi.yml
  format: yaml
  label: GoCardless subscriptions API
  slug: gocardless-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gocardless/refs/heads/main/openapi/gocardless-subscriptions-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Gocardless Authentication
name_suffix: Authentication
oauth_flows: []
overview: GoCardless secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: GoCardless
provider_slug: gocardless
scheme_count: 1
schemes:
- description: GoCardless access token from the dashboard
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/gocardless-openapi.yml
  type: http
slug: gocardless-authentication
source_filename: gocardless-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/gocardless-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: GoCardless access token from the dashboard\n  sources:\n  - openapi/gocardless-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gocardless/refs/heads/main/authentication/gocardless-authentication.yml
summary_line: http · 1 scheme
tags:
- Payments
- Direct Debit
- Bank Debit
- Recurring Payments
- Subscriptions
- SEPA
- Bacs
- ACH
- Open Banking
- Fintech
---
