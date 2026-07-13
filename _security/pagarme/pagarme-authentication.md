---
api_key_in: []
api_specs:
- filename: pagarme-openapi.yml
  format: yaml
  label: Pagar.me Orders API
  slug: pagarme-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pagarme/refs/heads/main/openapi/pagarme-openapi.yml
- filename: pagarme-openapi.yml
  format: yaml
  label: Pagar.me Charges API
  slug: pagarme-charges-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pagarme/refs/heads/main/openapi/pagarme-openapi.yml
- filename: pagarme-openapi.yml
  format: yaml
  label: Pagar.me Customers and Cards API
  slug: pagarme-customers-cards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pagarme/refs/heads/main/openapi/pagarme-openapi.yml
- filename: pagarme-openapi.yml
  format: yaml
  label: Pagar.me Subscriptions and Plans API
  slug: pagarme-subscriptions-plans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pagarme/refs/heads/main/openapi/pagarme-openapi.yml
- filename: pagarme-openapi.yml
  format: yaml
  label: Pagar.me Invoices API
  slug: pagarme-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pagarme/refs/heads/main/openapi/pagarme-openapi.yml
- filename: pagarme-openapi.yml
  format: yaml
  label: Pagar.me Recipients and Split API
  slug: pagarme-recipients-split-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pagarme/refs/heads/main/openapi/pagarme-openapi.yml
- filename: pagarme-openapi.yml
  format: yaml
  label: Pagar.me Transfers API
  slug: pagarme-transfers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pagarme/refs/heads/main/openapi/pagarme-openapi.yml
- filename: pagarme-openapi.yml
  format: yaml
  label: Pagar.me Webhooks API
  slug: pagarme-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pagarme/refs/heads/main/openapi/pagarme-openapi.yml
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
