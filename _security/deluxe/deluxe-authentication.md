---
api_key_in: []
api_specs:
- filename: deluxe-american-api-openapi.yml
  format: yaml
  label: Deluxe Corporation American API
  slug: deluxe-american-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deluxe/refs/heads/main/openapi/deluxe-american-api-openapi.yml
- filename: deluxe-batches-api-openapi.yml
  format: yaml
  label: Deluxe Corporation Batches API
  slug: deluxe-batches-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deluxe/refs/heads/main/openapi/deluxe-batches-api-openapi.yml
- filename: deluxe-customers-api-openapi.yml
  format: yaml
  label: Deluxe Corporation Customers API
  slug: deluxe-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deluxe/refs/heads/main/openapi/deluxe-customers-api-openapi.yml
- filename: deluxe-emv-api-openapi.yml
  format: yaml
  label: Deluxe Corporation Emv API
  slug: deluxe-emv-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deluxe/refs/heads/main/openapi/deluxe-emv-api-openapi.yml
- filename: deluxe-events-api-openapi.yml
  format: yaml
  label: Deluxe Corporation Events API
  slug: deluxe-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deluxe/refs/heads/main/openapi/deluxe-events-api-openapi.yml
- filename: deluxe-invoices-api-openapi.yml
  format: yaml
  label: Deluxe Corporation Invoices API
  slug: deluxe-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deluxe/refs/heads/main/openapi/deluxe-invoices-api-openapi.yml
- filename: deluxe-paymentlinks-api-openapi.yml
  format: yaml
  label: Deluxe Corporation Paymentlinks API
  slug: deluxe-paymentlinks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deluxe/refs/heads/main/openapi/deluxe-paymentlinks-api-openapi.yml
- filename: deluxe-paymentmethods-api-openapi.yml
  format: yaml
  label: Deluxe Corporation Paymentmethods API
  slug: deluxe-paymentmethods-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deluxe/refs/heads/main/openapi/deluxe-paymentmethods-api-openapi.yml
- filename: deluxe-payments-api-openapi.yml
  format: yaml
  label: Deluxe Corporation Payments API
  slug: deluxe-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deluxe/refs/heads/main/openapi/deluxe-payments-api-openapi.yml
- filename: deluxe-refunds-api-openapi.yml
  format: yaml
  label: Deluxe Corporation Refunds API
  slug: deluxe-refunds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deluxe/refs/heads/main/openapi/deluxe-refunds-api-openapi.yml
- filename: deluxe-reports-api-openapi.yml
  format: yaml
  label: Deluxe Corporation Reports API
  slug: deluxe-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deluxe/refs/heads/main/openapi/deluxe-reports-api-openapi.yml
- filename: deluxe-secservices-api-openapi.yml
  format: yaml
  label: Deluxe Corporation Secservices API
  slug: deluxe-secservices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deluxe/refs/heads/main/openapi/deluxe-secservices-api-openapi.yml
- filename: deluxe-subscriptions-api-openapi.yml
  format: yaml
  label: Deluxe Corporation Subscriptions API
  slug: deluxe-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deluxe/refs/heads/main/openapi/deluxe-subscriptions-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Deluxe Authentication
name_suffix: Authentication
oauth_flows: []
overview: Deluxe Corporation secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Deluxe Corporation
provider_slug: deluxe
scheme_count: 2
schemes:
- bearerFormat: JWT
  description: 'This API supports OpenID Connect OAuth 2.0 for authenticating all API requests.

    Bearer tokens are obtained from the Deluxe security service token endpoint using client credentials and expire after 60 minutes.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/deluxe-dpp-gateway-openapi.yml
  - openapi/deluxe-dpp-invoices-openapi.yml
  - openapi/deluxe-dpp-reports-openapi.yml
  type: http
- description: This API supports Anypoint's Client ID Enforcement authentication policy.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/deluxe-dpp-gateway-openapi.yml
  - openapi/deluxe-dpp-invoices-openapi.yml
  - openapi/deluxe-dpp-reports-openapi.yml
  - openapi/deluxe-postman-sandbox-openapi.yml
  type: http
slug: deluxe-authentication
source_filename: deluxe-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: derived\nsource: openapi/deluxe-dpp-gateway-openapi.yml, openapi/deluxe-dpp-invoices-openapi.yml, openapi/deluxe-dpp-reports-openapi.yml,\n  openapi/deluxe-postman-sandbox-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: |-\n    This API supports OpenID Connect OAuth 2.0 for authenticating all API requests.\n    Bearer tokens are obtained from the Deluxe security service token endpoint using client credentials and expire after 60 minutes.\n  sources:\n  - openapi/deluxe-dpp-gateway-openapi.yml\n  - openapi/deluxe-dpp-invoices-openapi.yml\n  - openapi/deluxe-dpp-reports-openapi.yml\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: This API supports Anypoint's Client ID Enforcement authentication policy.\n  sources:\n  - openapi/deluxe-dpp-gateway-openapi.yml\n  - openapi/deluxe-dpp-invoices-openapi.yml\n  - openapi/deluxe-dpp-reports-openapi.yml\n\
  \  - openapi/deluxe-postman-sandbox-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/deluxe/refs/heads/main/authentication/deluxe-authentication.yml
summary_line: http · 2 schemes
tags:
- Payments
- Merchant Services
- Card Processing
- ACH
- Invoicing
- Subscription
- Tokenization
- Webhook
- Reporting
- Data Analytics
- Marketing
- Small Business
---
