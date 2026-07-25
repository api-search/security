---
api_key_in: []
api_specs:
- filename: komoju-barcodes-api-openapi.yml
  format: yaml
  label: KOMOJU Barcodes API
  slug: komoju-barcodes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/komoju/refs/heads/main/openapi/komoju-barcodes-api-openapi.yml
- filename: komoju-customers-api-openapi.yml
  format: yaml
  label: KOMOJU Customers API
  slug: komoju-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/komoju/refs/heads/main/openapi/komoju-customers-api-openapi.yml
- filename: komoju-events-api-openapi.yml
  format: yaml
  label: KOMOJU Events API
  slug: komoju-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/komoju/refs/heads/main/openapi/komoju-events-api-openapi.yml
- filename: komoju-payment-methods-api-openapi.yml
  format: yaml
  label: KOMOJU Payment Methods API
  slug: komoju-payment-methods-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/komoju/refs/heads/main/openapi/komoju-payment-methods-api-openapi.yml
- filename: komoju-payments-api-openapi.yml
  format: yaml
  label: KOMOJU Payments API
  slug: komoju-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/komoju/refs/heads/main/openapi/komoju-payments-api-openapi.yml
- filename: komoju-sessions-api-openapi.yml
  format: yaml
  label: KOMOJU Sessions API
  slug: komoju-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/komoju/refs/heads/main/openapi/komoju-sessions-api-openapi.yml
- filename: komoju-subscriptions-api-openapi.yml
  format: yaml
  label: KOMOJU Subscriptions API
  slug: komoju-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/komoju/refs/heads/main/openapi/komoju-subscriptions-api-openapi.yml
- filename: komoju-tokens-api-openapi.yml
  format: yaml
  label: KOMOJU Tokens API
  slug: komoju-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/komoju/refs/heads/main/openapi/komoju-tokens-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Komoju Authentication
name_suffix: Authentication
oauth_flows: []
overview: KOMOJU secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: KOMOJU
provider_slug: komoju
scheme_count: 1
schemes:
- description: 'HTTP Basic Authentication. Use your KOMOJU API key as the username and leave the password empty (for example `curl -u secret_key: "https://komoju.com/api/v1/payments"`). Secret keys grant full access to all API resources and must stay server-side; publishable keys are safe to expose client-side but are limited to creating tokens and paying for sessions. Each merchant account has separate test and live key pairs. An optional `X-KOMOJU-API-VERSION` header pins the API version.'
  name: basicAuth
  scheme: basic
  sources:
  - openapi/komoju-openapi.yml
  - https://doc.komoju.com/docs/authentication
  type: http
slug: komoju-authentication
source_filename: komoju-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-12'\nmethod: derived\nsource: openapi/komoju-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: 'HTTP Basic Authentication. Use your KOMOJU API key as the username and\n    leave the password empty (for example `curl -u secret_key: \"https://komoju.com/api/v1/payments\"`).\n    Secret keys grant full access to all API resources and must stay server-side;\n    publishable keys are safe to expose client-side but are limited to creating tokens\n    and paying for sessions. Each merchant account has separate test and live key\n    pairs. An optional `X-KOMOJU-API-VERSION` header pins the API version.'\n  sources:\n  - openapi/komoju-openapi.yml\n  - https://doc.komoju.com/docs/authentication\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/komoju/refs/heads/main/authentication/komoju-authentication.yml
summary_line: http · 1 scheme
tags:
- Payments
- Payment Gateway
- Japan
- Konbini
- Cards
- PayPay
- Bank Transfer
- E-Money
- Checkout
- Fintech
---
