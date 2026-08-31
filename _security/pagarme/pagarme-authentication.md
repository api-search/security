---
api_key_in: []
api_specs:
- filename: pagarme-anticipations-api-openapi.yml
  format: yaml
  label: Pagar.me Anticipations API
  slug: pagarme-anticipations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pagarme/refs/heads/main/openapi/pagarme-anticipations-api-openapi.yml
- filename: pagarme-cards-api-openapi.yml
  format: yaml
  label: Pagar.me Cards API
  slug: pagarme-cards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pagarme/refs/heads/main/openapi/pagarme-cards-api-openapi.yml
- filename: pagarme-charges-api-openapi.yml
  format: yaml
  label: Pagar.me Charges API
  slug: pagarme-charges-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pagarme/refs/heads/main/openapi/pagarme-charges-api-openapi.yml
- filename: pagarme-customers-api-openapi.yml
  format: yaml
  label: Pagar.me Customers API
  slug: pagarme-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pagarme/refs/heads/main/openapi/pagarme-customers-api-openapi.yml
- filename: pagarme-invoices-api-openapi.yml
  format: yaml
  label: Pagar.me Invoices API
  slug: pagarme-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pagarme/refs/heads/main/openapi/pagarme-invoices-api-openapi.yml
- filename: pagarme-orders-api-openapi.yml
  format: yaml
  label: Pagar.me Orders API
  slug: pagarme-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pagarme/refs/heads/main/openapi/pagarme-orders-api-openapi.yml
- filename: pagarme-plans-api-openapi.yml
  format: yaml
  label: Pagar.me Plans API
  slug: pagarme-plans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pagarme/refs/heads/main/openapi/pagarme-plans-api-openapi.yml
- filename: pagarme-recipients-api-openapi.yml
  format: yaml
  label: Pagar.me Recipients API
  slug: pagarme-recipients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pagarme/refs/heads/main/openapi/pagarme-recipients-api-openapi.yml
- filename: pagarme-subscriptions-api-openapi.yml
  format: yaml
  label: Pagar.me Subscriptions API
  slug: pagarme-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pagarme/refs/heads/main/openapi/pagarme-subscriptions-api-openapi.yml
- filename: pagarme-transfers-api-openapi.yml
  format: yaml
  label: Pagar.me Transfers API
  slug: pagarme-transfers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pagarme/refs/heads/main/openapi/pagarme-transfers-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Pagarme Authentication
name_suffix: Authentication
oauth_flows: []
overview: Pagar.me secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Pagar.me
provider_slug: pagarme
scheme_count: 1
schemes:
- description: HTTP Basic auth with the account secret key as the username and an empty password.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/pagarme-openapi.yml
  type: http
slug: pagarme-authentication
source_filename: pagarme-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/pagarme-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic auth with the account secret key as the username and an empty password.\n  sources:\n  - openapi/pagarme-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pagarme/refs/heads/main/authentication/pagarme-authentication.yml
summary_line: http · 1 scheme
tags:
- Payments
- Payment Gateway
- PIX
- Boleto
- Brazil
---
