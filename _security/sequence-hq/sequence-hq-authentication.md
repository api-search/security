---
api_key_in: []
api_specs:
- filename: sequence-hq-openapi.yml
  format: yaml
  label: Sequence Customers API
  slug: sequence-hq-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sequence-hq/refs/heads/main/openapi/sequence-hq-openapi.yml
- filename: sequence-hq-openapi.yml
  format: yaml
  label: Sequence Usage & Metering API
  slug: sequence-hq-usage-metering-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sequence-hq/refs/heads/main/openapi/sequence-hq-openapi.yml
- filename: sequence-hq-openapi.yml
  format: yaml
  label: Sequence Billing Schedules API
  slug: sequence-hq-billing-schedules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sequence-hq/refs/heads/main/openapi/sequence-hq-openapi.yml
- filename: sequence-hq-openapi.yml
  format: yaml
  label: Sequence Invoices & Credit Notes API
  slug: sequence-hq-invoices-credit-notes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sequence-hq/refs/heads/main/openapi/sequence-hq-openapi.yml
- filename: sequence-hq-openapi.yml
  format: yaml
  label: Sequence Products & Prices API
  slug: sequence-hq-products-prices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sequence-hq/refs/heads/main/openapi/sequence-hq-openapi.yml
- filename: sequence-hq-openapi.yml
  format: yaml
  label: Sequence Quotes API
  slug: sequence-hq-quotes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sequence-hq/refs/heads/main/openapi/sequence-hq-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: documented
name: Sequence Hq Authentication
name_suffix: Authentication
oauth_flows: []
overview: Sequence secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Sequence
provider_slug: sequence-hq
scheme_count: 1
schemes:
- description: 'HTTP Basic authentication. When you create an API client in the Sequence Dashboard you receive a Client ID and a Client Secret. The Client ID is used as the Basic auth username and the Client Secret as the password, sent as `Authorization: Basic base64(clientId:clientSecret)`. The Client Secret is shown only once and cannot be retrieved later. Requests also accept a `sequence-version` header to pin the date-based API version (for example 2024-07-30). Two environments are available - Production and Sandbox - each with its own credentials.'
  name: basicAuth
  scheme: basic
  sources:
  - https://docs.sequencehq.com/reference/authentication
  - https://docs.sequencehq.com/reference/gettingStarted
  type: http
slug: sequence-hq-authentication
source_filename: sequence-hq-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-12'\nmethod: documented\nsource: https://docs.sequencehq.com/reference/authentication\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: >-\n    HTTP Basic authentication. When you create an API client in the Sequence\n    Dashboard you receive a Client ID and a Client Secret. The Client ID is used\n    as the Basic auth username and the Client Secret as the password, sent as\n    `Authorization: Basic base64(clientId:clientSecret)`. The Client Secret is\n    shown only once and cannot be retrieved later. Requests also accept a\n    `sequence-version` header to pin the date-based API version (for example\n    2024-07-30). Two environments are available - Production and Sandbox - each\n    with its own credentials.\n  sources:\n  - https://docs.sequencehq.com/reference/authentication\n  - https://docs.sequencehq.com/reference/gettingStarted\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sequence-hq/refs/heads/main/authentication/sequence-hq-authentication.yml
summary_line: http · 1 scheme
tags:
- Billing
- Usage-Based Billing
- Revenue Recognition
- Metering
- Invoicing
- Pricing
- Revenue Orchestration
- FinOps
---
