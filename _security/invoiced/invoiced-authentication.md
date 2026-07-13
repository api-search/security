---
api_key_in: []
api_specs:
- filename: invoiced-openapi.yml
  format: yaml
  label: Invoiced Customers API
  slug: customers
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/invoiced/refs/heads/main/openapi/invoiced-openapi.yml
- filename: invoiced-openapi.yml
  format: yaml
  label: Invoiced Invoices API
  slug: invoices
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/invoiced/refs/heads/main/openapi/invoiced-openapi.yml
- filename: invoiced-openapi.yml
  format: yaml
  label: Invoiced Estimates API
  slug: estimates
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/invoiced/refs/heads/main/openapi/invoiced-openapi.yml
- filename: invoiced-openapi.yml
  format: yaml
  label: Invoiced Credit Notes API
  slug: credit-notes
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/invoiced/refs/heads/main/openapi/invoiced-openapi.yml
- filename: invoiced-openapi.yml
  format: yaml
  label: Invoiced Payments API
  slug: payments
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/invoiced/refs/heads/main/openapi/invoiced-openapi.yml
- filename: invoiced-openapi.yml
  format: yaml
  label: Invoiced Subscriptions & Plans API
  slug: subscriptions
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/invoiced/refs/heads/main/openapi/invoiced-openapi.yml
- filename: invoiced-openapi.yml
  format: yaml
  label: Invoiced Items API
  slug: items
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/invoiced/refs/heads/main/openapi/invoiced-openapi.yml
- filename: invoiced-openapi.yml
  format: yaml
  label: Invoiced Events & Webhooks API
  slug: webhooks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/invoiced/refs/heads/main/openapi/invoiced-openapi.yml
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
