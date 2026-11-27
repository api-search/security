---
anonymous_access: false
api_key_in: []
api_specs:
- filename: countersignatory-com-openapi-generated.yml
  format: yaml
  label: Countersignatory API
  slug: countersignatory-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/countersignatory-com/openapi/_ae-authored/countersignatory-com-openapi-generated.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Countersignatory Authentication
name_suffix: Authentication
oauth_flows: []
overview: Countersignatory declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: Countersignatory
provider_slug: countersignatory-com
scheme_count: 3
schemes:
- description: '"API keys are free, instant and unapproved, and an order needs no key." Keys are taken via POST /v1/keys; the route index says "Keys exist so distinct callers can be counted honestly."'
  issuance: https://countersignatory.com/v1/keys
  name: api-key
  required: false
  type: apiKey
- description: x402 payment headers gate order placement. POST /v1/orders accepts an X-PAYMENT header (x402 version 1); POST /v1/x402/check accepts a PAYMENT-SIGNATURE header (x402 version 2). Scheme exact, USDC on Base.
  headers:
  - X-PAYMENT
  - PAYMENT-SIGNATURE
  name: x402-payment
  response_headers:
  - X-PAYMENT-RESPONSE
  - PAYMENT-RESPONSE
  - PAYMENT-REQUIRED
  type: payment
- description: '"The order id is the only credential, so keep it." GET /v1/orders/{id} returns the order to whoever holds the id.'
  name: order-id-bearer
  type: capability-url
slug: countersignatory-com-authentication
source_filename: countersignatory-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://countersignatory.com/llms.txt\ndocs: https://countersignatory.com/llms.txt\nnote: The generated OpenAPI declares no securitySchemes. The docs state API keys are free, instant and unapproved, and that an order needs no key; payment (x402 or card checkout) is the gate on orders, and the order id is the only credential for reading an order. The header used to present a key is not documented in llms.txt.\nschemes:\n- name: api-key\n  type: apiKey\n  description: '\"API keys are free, instant and unapproved, and an order needs no key.\" Keys are taken via POST /v1/keys; the route index says \"Keys exist so distinct callers can be counted honestly.\"'\n  issuance: https://countersignatory.com/v1/keys\n  required: false\n- name: x402-payment\n  type: payment\n  description: x402 payment headers gate order placement. POST /v1/orders accepts an X-PAYMENT header (x402 version 1); POST /v1/x402/check accepts a PAYMENT-SIGNATURE\
  \ header (x402 version 2). Scheme exact, USDC on Base.\n  headers: [X-PAYMENT, PAYMENT-SIGNATURE]\n  response_headers: [X-PAYMENT-RESPONSE, PAYMENT-RESPONSE, PAYMENT-REQUIRED]\n- name: order-id-bearer\n  type: capability-url\n  description: '\"The order id is the only credential, so keep it.\" GET /v1/orders/{id} returns the order to whoever holds the id.'\n"
source_yaml_url: https://artifacts.apis.io/countersignatory-com/authentication/countersignatory-com-authentication.yml
summary_line: 3 schemes
tags:
- Company
- Human-in-the-Loop
- AI Agents
- Human Verification
- Marketplace
- Pricing Index
- x402
- MCP
---
