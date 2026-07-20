---
api_key_in:
- header
api_specs:
- filename: apurata-acuotaz-pos-openapi.yml
  format: yaml
  label: Apurata aCuotaz POS REST API
  slug: apurata-acuotaz-pos-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apurata/refs/heads/main/openapi/apurata-acuotaz-pos-openapi.yml
auth_types:
- http
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Apurata Authentication
name_suffix: Authentication
oauth_flows: []
overview: Apurata secures its APIs with http and apiKey across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Apurata
provider_slug: apurata
scheme_count: 4
schemes:
- applies_to: all /pos/order and /pos/client operations
  description: 'Merchant secret token issued by Apurata, sent as Authorization: Bearer <secret_token>. HTTPS is mandatory.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/apurata-acuotaz-pos-openapi.yml
  type: http
- description: Merchant client id used to authenticate the checkout widget endpoints (pay-with-apurata-add-on, info-steps).
  in: header
  name: clientIdHeader
  parameter_name: Client_id
  sources:
  - openapi/apurata-acuotaz-pos-openapi.yml
  type: apiKey
- description: Caller-generated idempotency token required on total-refund and partial-refund to prevent duplicate refunds.
  in: header
  name: uniqueTokenHeader
  parameter_name: X-Unique-Token
  sources:
  - openapi/apurata-acuotaz-pos-openapi.yml
  type: apiKey
- description: 'Bearer credential Apurata includes on outbound webhook POSTs (header "Apurata-Auth: Bearer <secret_token>"); merchant validation is optional but recommended.'
  direction: inbound-to-merchant
  name: webhookAuth
  parameter_name: Apurata-Auth
  scheme: bearer
  sources:
  - https://docs.apurata.com/POS/webhooks/
  type: http
slug: apurata-authentication
source_filename: apurata-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: openapi/apurata-acuotaz-pos-openapi.yml\ndocs: https://docs.apurata.com/POS/rest_api/authentication/\nsummary:\n  types:\n  - http\n  - apiKey\n  api_key_in:\n  - header\n  notes: >-\n    aCuotaz uses a per-merchant secret token as an HTTP Bearer credential over\n    mandatory HTTPS. Two additional header credentials appear on specific\n    operations: Client_id (identifies the merchant for the checkout widget\n    endpoints) and X-Unique-Token (an idempotency token required on refunds).\n    Webhooks delivered by Apurata carry their own Apurata-Auth Bearer header that\n    the merchant validates. There is no OAuth surface.\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'Merchant secret token issued by Apurata, sent as Authorization: Bearer <secret_token>. HTTPS is mandatory.'\n  applies_to: all /pos/order and /pos/client operations\n  sources:\n  - openapi/apurata-acuotaz-pos-openapi.yml\n- name:\
  \ clientIdHeader\n  type: apiKey\n  in: header\n  parameter_name: Client_id\n  description: Merchant client id used to authenticate the checkout widget endpoints (pay-with-apurata-add-on, info-steps).\n  sources:\n  - openapi/apurata-acuotaz-pos-openapi.yml\n- name: uniqueTokenHeader\n  type: apiKey\n  in: header\n  parameter_name: X-Unique-Token\n  description: Caller-generated idempotency token required on total-refund and partial-refund to prevent duplicate refunds.\n  sources:\n  - openapi/apurata-acuotaz-pos-openapi.yml\n- name: webhookAuth\n  type: http\n  scheme: bearer\n  parameter_name: Apurata-Auth\n  description: >-\n    Bearer credential Apurata includes on outbound webhook POSTs\n    (header \"Apurata-Auth: Bearer <secret_token>\"); merchant validation is\n    optional but recommended.\n  direction: inbound-to-merchant\n  sources:\n  - https://docs.apurata.com/POS/webhooks/\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apurata/refs/heads/main/authentication/apurata-authentication.yml
summary_line: http/apiKey · 4 schemes
tags:
- Company
- Financial Services
- Fintech
- Lending
- Buy Now Pay Later
- Installment Payments
- Consumer Credit
- Payments
- E-commerce
- Peru
- Latin America
---
