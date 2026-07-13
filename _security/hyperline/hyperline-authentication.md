---
api_key_in: []
api_specs:
- filename: hyperline-openapi.yml
  format: yaml
  label: Hyperline Customers API
  slug: hyperline-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hyperline/refs/heads/main/openapi/hyperline-openapi.yml
- filename: hyperline-openapi.yml
  format: yaml
  label: Hyperline Products & Plans API
  slug: hyperline-products-plans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hyperline/refs/heads/main/openapi/hyperline-openapi.yml
- filename: hyperline-openapi.yml
  format: yaml
  label: Hyperline Subscriptions API
  slug: hyperline-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hyperline/refs/heads/main/openapi/hyperline-openapi.yml
- filename: hyperline-openapi.yml
  format: yaml
  label: Hyperline Usage & Events API
  slug: hyperline-usage-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hyperline/refs/heads/main/openapi/hyperline-openapi.yml
- filename: hyperline-openapi.yml
  format: yaml
  label: Hyperline Invoices API
  slug: hyperline-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hyperline/refs/heads/main/openapi/hyperline-openapi.yml
- filename: hyperline-openapi.yml
  format: yaml
  label: Hyperline Payments API
  slug: hyperline-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hyperline/refs/heads/main/openapi/hyperline-openapi.yml
- filename: hyperline-openapi.yml
  format: yaml
  label: Hyperline Webhooks API
  slug: hyperline-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hyperline/refs/heads/main/openapi/hyperline-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Hyperline Authentication
name_suffix: Authentication
oauth_flows: []
overview: Hyperline secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Hyperline
provider_slug: hyperline
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: 'Authenticate with your Hyperline API key passed as a bearer token in the Authorization header - `Authorization: Bearer <API_KEY>`.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/hyperline-openapi.yml
  type: http
slug: hyperline-authentication
source_filename: hyperline-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/hyperline-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: 'Authenticate with your Hyperline API key passed as a bearer token in the Authorization\n    header - `Authorization: Bearer <API_KEY>`.'\n  sources:\n  - openapi/hyperline-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hyperline/refs/heads/main/authentication/hyperline-authentication.yml
summary_line: http · 1 scheme
tags:
- Billing
- Subscriptions
- Usage-Based
- Metering
- Payments
- Invoicing
- FinOps
---
