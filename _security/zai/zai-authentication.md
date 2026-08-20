---
api_key_in: []
api_specs:
- filename: zai-assembly-api.json
  format: json
  label: Zai Assembly API
  slug: zai-assembly-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zai/refs/heads/main/openapi/zai-assembly-api.json
- filename: zai-virtual-accounts-payid.json
  format: json
  label: Zai Virtual Accounts and PayIDs API
  slug: zai-virtual-accounts-payid-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zai/refs/heads/main/openapi/zai-virtual-accounts-payid.json
- filename: zai-payto.json
  format: json
  label: Zai PayTo API
  slug: zai-payto-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zai/refs/heads/main/openapi/zai-payto.json
- filename: zai-async-api.json
  format: json
  label: Zai Asynchronous API
  slug: zai-async-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zai/refs/heads/main/openapi/zai-async-api.json
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Zai Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Zai secures its APIs with http and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Zai
provider_slug: zai
scheme_count: 3
schemes:
- description: Please refer to Authentication section within https://developer.assemblypayments.com/reference#authentication
  flows:
  - flow: clientCredentials
    scopes: 0
    tokenUrl: https://au-0000.sandbox.auth.assemblypay.com/tokens
  name: oAuth2ClientCredentials
  sources:
  - openapi/zai-assembly-api.json
  - openapi/zai-async-api.json
  type: oauth2
- name: basicAuth
  scheme: basic
  sources:
  - openapi/zai-async-api.json
  type: http
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/zai-payto.json
  type: http
slug: zai-authentication
source_filename: zai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-24'\nmethod: derived\nsource: openapi/zai-assembly-api.json, openapi/zai-async-api.json, openapi/zai-payto.json\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: oAuth2ClientCredentials\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://au-0000.sandbox.auth.assemblypay.com/tokens\n    scopes: 0\n  description: Please refer to Authentication section within https://developer.assemblypayments.com/reference#authentication\n  sources:\n  - openapi/zai-assembly-api.json\n  - openapi/zai-async-api.json\n- name: basicAuth\n  type: http\n  scheme: basic\n  sources:\n  - openapi/zai-async-api.json\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/zai-payto.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zai/refs/heads/main/authentication/zai-authentication.yml
summary_line: http/oauth2 · 3 schemes
tags:
- Payments
- Australia
- Payment Gateway
- Payment Processing
- Marketplace Payments
- Payments-as-a-Service
- Real-Time Payments
- Account-to-Account
- Open Banking
- PayTo
- PayID
- NPP
- Direct Debit
- Digital Wallet
- Payouts
---
