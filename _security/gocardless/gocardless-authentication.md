---
api_key_in: []
api_specs:
- filename: openapi
  format: yaml
  label: GoCardless REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://developer.gocardless.com/api-reference/openapi
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
