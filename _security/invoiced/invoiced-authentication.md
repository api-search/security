---
api_key_in: []
api_specs:
- filename: invoiced-credit-notes-api-openapi.yml
  format: yaml
  label: Invoiced Credit Notes API
  slug: invoiced-credit-notes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/invoiced/refs/heads/main/openapi/invoiced-credit-notes-api-openapi.yml
- filename: invoiced-customers-api-openapi.yml
  format: yaml
  label: Invoiced Customers API
  slug: invoiced-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/invoiced/refs/heads/main/openapi/invoiced-customers-api-openapi.yml
- filename: invoiced-estimates-api-openapi.yml
  format: yaml
  label: Invoiced Estimates API
  slug: invoiced-estimates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/invoiced/refs/heads/main/openapi/invoiced-estimates-api-openapi.yml
- filename: invoiced-events-api-openapi.yml
  format: yaml
  label: Invoiced Events API
  slug: invoiced-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/invoiced/refs/heads/main/openapi/invoiced-events-api-openapi.yml
- filename: invoiced-invoices-api-openapi.yml
  format: yaml
  label: Invoiced Invoices API
  slug: invoiced-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/invoiced/refs/heads/main/openapi/invoiced-invoices-api-openapi.yml
- filename: invoiced-items-api-openapi.yml
  format: yaml
  label: Invoiced Items API
  slug: invoiced-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/invoiced/refs/heads/main/openapi/invoiced-items-api-openapi.yml
- filename: invoiced-payments-api-openapi.yml
  format: yaml
  label: Invoiced Payments API
  slug: invoiced-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/invoiced/refs/heads/main/openapi/invoiced-payments-api-openapi.yml
- filename: invoiced-plans-api-openapi.yml
  format: yaml
  label: Invoiced Plans API
  slug: invoiced-plans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/invoiced/refs/heads/main/openapi/invoiced-plans-api-openapi.yml
- filename: invoiced-subscriptions-api-openapi.yml
  format: yaml
  label: Invoiced Subscriptions API
  slug: invoiced-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/invoiced/refs/heads/main/openapi/invoiced-subscriptions-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Invoiced Authentication
name_suffix: Authentication
oauth_flows: []
overview: Invoiced secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Invoiced
provider_slug: invoiced
scheme_count: 1
schemes:
- description: HTTP Basic authentication. Use your Invoiced API key as the username and leave the password blank. API keys are created under Settings -> Developers -> API Keys.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/invoiced-openapi.yml
  type: http
slug: invoiced-authentication
source_filename: invoiced-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/invoiced-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic authentication. Use your Invoiced API key as the username and leave\n    the password blank. API keys are created under Settings -> Developers -> API Keys.\n  sources:\n  - openapi/invoiced-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/invoiced/refs/heads/main/authentication/invoiced-authentication.yml
summary_line: http · 1 scheme
tags:
- Accounts Receivable
- Billing
- Invoicing
- Payments
- Subscriptions
---
