---
api_key_in:
- header
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: searched
name: Fatora Authentication
name_suffix: Authentication
oauth_flows: []
overview: Fatora secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Fatora
provider_slug: fatora
scheme_count: 2
schemes:
- applies_to:
  - POST /v1/payments/checkout
  - refund
  - recurring
  - verify
  description: Static merchant API key sent in the api_key request header. Used for payment-related endpoints (checkout, refund, recurring, verify). Found in the merchant dashboard under Integration in the sidebar.
  in: header
  name: api_key
  parameter_name: api_key
  sources:
  - https://fatora.io/api/authentication.php
  type: apiKey
- applies_to:
  - invoices
  - clients
  - products
  bearer_format: JWT
  description: Bearer JWT required for invoice, client and product endpoints. Obtained by POSTing to the Authorization endpoint with the api_key header; the response returns a bearer_token JWT that is then sent as Authorization Bearer on subsequent calls.
  name: bearerAuth
  scheme: bearer
  sources:
  - https://fatora.io/api/authentication.php
  token_endpoint: https://api.fatora.io/v1/Authorization/Authorize
  type: http
slug: fatora-authentication
source_filename: fatora-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://fatora.io/api/authentication.php\ndocs: https://fatora.io/api/authentication.php\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\n  http_schemes:\n  - bearer\n  note: >-\n    Two coexisting mechanisms. Payment endpoints (checkout, refund, recurring, verify) take a\n    static merchant API key in an api_key header. Invoice/client/product endpoints require a\n    short-lived Bearer JWT that is first minted by calling the Authorization endpoint with the\n    api_key.\nschemes:\n- name: api_key\n  type: apiKey\n  in: header\n  parameter_name: api_key\n  description: >-\n    Static merchant API key sent in the api_key request header. Used for payment-related\n    endpoints (checkout, refund, recurring, verify). Found in the merchant dashboard under\n    Integration in the sidebar.\n  applies_to:\n  - POST /v1/payments/checkout\n  - refund\n  - recurring\n  - verify\n  sources:\n  - https://fatora.io/api/authentication.php\n\
  - name: bearerAuth\n  type: http\n  scheme: bearer\n  bearer_format: JWT\n  description: >-\n    Bearer JWT required for invoice, client and product endpoints. Obtained by POSTing to the\n    Authorization endpoint with the api_key header; the response returns a bearer_token JWT that\n    is then sent as Authorization Bearer on subsequent calls.\n  token_endpoint: https://api.fatora.io/v1/Authorization/Authorize\n  applies_to:\n  - invoices\n  - clients\n  - products\n  sources:\n  - https://fatora.io/api/authentication.php\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fatora/refs/heads/main/authentication/fatora-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Payments
- Invoicing
- Payment Gateway
- E-commerce
- Billing
- Fintech
- Checkout
- MENA
- Qatar
- SaaS
---
