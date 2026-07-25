---
api_key_in: []
api_specs:
- filename: chargebee-customers-api-openapi.yml
  format: yaml
  label: Chargebee Customers API
  slug: chargebee-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chargebee/refs/heads/main/openapi/chargebee-customers-api-openapi.yml
- filename: chargebee-invoices-api-openapi.yml
  format: yaml
  label: Chargebee Invoices API
  slug: chargebee-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chargebee/refs/heads/main/openapi/chargebee-invoices-api-openapi.yml
- filename: chargebee-items-api-openapi.yml
  format: yaml
  label: Chargebee Items API
  slug: chargebee-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chargebee/refs/heads/main/openapi/chargebee-items-api-openapi.yml
- filename: chargebee-orders-api-openapi.yml
  format: yaml
  label: Chargebee Orders API
  slug: chargebee-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chargebee/refs/heads/main/openapi/chargebee-orders-api-openapi.yml
- filename: chargebee-payments-api-openapi.yml
  format: yaml
  label: Chargebee Payments API
  slug: chargebee-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chargebee/refs/heads/main/openapi/chargebee-payments-api-openapi.yml
- filename: chargebee-plans-api-openapi.yml
  format: yaml
  label: Chargebee Plans API
  slug: chargebee-plans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chargebee/refs/heads/main/openapi/chargebee-plans-api-openapi.yml
- filename: chargebee-quotes-api-openapi.yml
  format: yaml
  label: Chargebee Quotes API
  slug: chargebee-quotes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chargebee/refs/heads/main/openapi/chargebee-quotes-api-openapi.yml
- filename: chargebee-subscriptions-api-openapi.yml
  format: yaml
  label: Chargebee Subscriptions API
  slug: chargebee-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chargebee/refs/heads/main/openapi/chargebee-subscriptions-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Chargebee Authentication
name_suffix: Authentication
oauth_flows: []
overview: Chargebee secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Chargebee
provider_slug: chargebee
scheme_count: 1
schemes:
- description: HTTP Basic Auth. Username is your Chargebee site API key; password is empty.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/chargebee-openapi.yml
  type: http
slug: chargebee-authentication
source_filename: chargebee-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/chargebee-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic Auth. Username is your Chargebee site API key; password is empty.\n  sources:\n  - openapi/chargebee-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chargebee/refs/heads/main/authentication/chargebee-authentication.yml
summary_line: http · 1 scheme
tags:
- Billing
- Subscriptions
- Recurring Billing
- Revenue
- Payments
- SaaS
---
