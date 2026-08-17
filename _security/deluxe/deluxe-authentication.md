---
api_key_in: []
api_specs:
- filename: deluxe-dpp-gateway-openapi.yml
  format: yaml
  label: Deluxe Payments Platform — Gateway Experience API
  slug: deluxe-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deluxe/refs/heads/main/openapi/deluxe-dpp-gateway-openapi.yml
- filename: deluxe-dpp-reports-openapi.yml
  format: yaml
  label: Deluxe Payments Platform — Reports Experience API
  slug: dpp-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deluxe/refs/heads/main/openapi/deluxe-dpp-reports-openapi.yml
- filename: deluxe-dpp-invoices-openapi.yml
  format: yaml
  label: Deluxe Payments Platform — Invoice Experience API
  slug: dpp-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deluxe/refs/heads/main/openapi/deluxe-dpp-invoices-openapi.yml
- filename: deluxe-postman-sandbox-openapi.yml
  format: yaml
  label: Deluxe Payments Platform — Sandbox API (Deluxe-published OpenAPI)
  slug: dpp-sandbox-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deluxe/refs/heads/main/openapi/deluxe-postman-sandbox-openapi.yml
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
- Subscriptions
- Tokenization
- Webhooks
- Reporting
- Data Analytics
- Marketing
- Small Business
---
