---
api_key_in:
- header
api_specs:
- filename: tribe-payments-trb-cc-api-merchant-api-credit-card-v3.json
  format: json
  label: Payment Gateway - Credit Card API
  slug: gateway-credit-card-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tribe-payments/refs/heads/main/openapi/tribe-payments-trb-cc-api-merchant-api-credit-card-v3.json
- filename: tribe-payments-trb-hpp-api-merchant-api-hpp-v3.json
  format: json
  label: Payment Gateway - Hosted Payments API (HPP)
  slug: gateway-hosted-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tribe-payments/refs/heads/main/openapi/tribe-payments-trb-hpp-api-merchant-api-hpp-v3.json
- filename: tribe-payments-trb-cc-token-api-merchant-api-credit-card-token-v3.json
  format: json
  label: Payment Gateway - Credit Card Token API
  slug: gateway-credit-card-token-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tribe-payments/refs/heads/main/openapi/tribe-payments-trb-cc-token-api-merchant-api-credit-card-token-v3.json
- filename: tribe-payments-trb-report-api-merchant-api-report-v3.json
  format: json
  label: Payment Gateway - Reports API
  slug: gateway-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tribe-payments/refs/heads/main/openapi/tribe-payments-trb-report-api-merchant-api-report-v3.json
- filename: tribe-payments-trb-isac-pos-tdd-device-api-openapi-device-directory-api-v3.json
  format: json
  label: Point of Sale - Device Directory API
  slug: pos-device-directory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tribe-payments/refs/heads/main/openapi/tribe-payments-trb-isac-pos-tdd-device-api-openapi-device-directory-api-v3.json
- filename: tribe-payments-trb-risk-monitor-client-api-openapi.json
  format: json
  label: Risk Monitor - Client API
  slug: risk-monitor-client-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tribe-payments/refs/heads/main/openapi/tribe-payments-trb-risk-monitor-client-api-openapi.json
- filename: tribe-payments-obb-bank-api-openapi.json
  format: json
  label: Open Banking - Bank API
  slug: open-banking-bank-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tribe-payments/refs/heads/main/openapi/tribe-payments-obb-bank-api-openapi.json
- filename: tribe-payments-obb-tpp-api-openapi.json
  format: json
  label: Open Banking - Third-Party Providers API (TPP)
  slug: open-banking-tpp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tribe-payments/refs/heads/main/openapi/tribe-payments-obb-tpp-api-openapi.json
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Tribe Payments Authentication
name_suffix: Authentication
oauth_flows: []
overview: Tribe Payments secures its APIs with apiKey and http across 8 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Tribe Payments
provider_slug: tribe-payments
scheme_count: 8
schemes:
- name: tokenAuth
  scheme: bearer
  sources:
  - openapi/tribe-payments-obb-tpp-api-openapi.json
  type: http
- in: header
  name: clientId
  parameter: X-Client-ID
  sources:
  - openapi/tribe-payments-obb-tpp-api-openapi.json
  type: apiKey
- in: header
  name: accountId
  parameter: x-auth-account-id
  sources:
  - openapi/tribe-payments-trb-cc-api-merchant-api-credit-card-callback-v3.json
  - openapi/tribe-payments-trb-cc-api-merchant-api-credit-card-v3.json
  - openapi/tribe-payments-trb-cc-token-api-merchant-api-credit-card-token-v3.json
  - openapi/tribe-payments-trb-cc-token-api-merchant-api-credit-card-token-webhook-v3.json
  - openapi/tribe-payments-trb-hpp-api-merchant-api-hpp-v3.json
  - openapi/tribe-payments-trb-hpp-api-merchant-api-hpp-webhook-v3.json
  type: apiKey
- in: header
  name: accountPassword
  parameter: x-auth-account-password
  sources:
  - openapi/tribe-payments-trb-cc-api-merchant-api-credit-card-callback-v3.json
  - openapi/tribe-payments-trb-cc-api-merchant-api-credit-card-v3.json
  - openapi/tribe-payments-trb-cc-token-api-merchant-api-credit-card-token-v3.json
  - openapi/tribe-payments-trb-cc-token-api-merchant-api-credit-card-token-webhook-v3.json
  - openapi/tribe-payments-trb-hpp-api-merchant-api-hpp-v3.json
  - openapi/tribe-payments-trb-hpp-api-merchant-api-hpp-webhook-v3.json
  type: apiKey
- in: header
  name: apiKey
  parameter: x-auth-report-api-key
  sources:
  - openapi/tribe-payments-trb-report-api-merchant-api-report-callback-v3.json
  - openapi/tribe-payments-trb-report-api-merchant-api-report-v3.json
  type: apiKey
- in: header
  name: apiPassword
  parameter: x-auth-report-api-password
  sources:
  - openapi/tribe-payments-trb-report-api-merchant-api-report-callback-v3.json
  - openapi/tribe-payments-trb-report-api-merchant-api-report-v3.json
  type: apiKey
- description: Value for the bearer header parameter.
  in: header
  name: Bearer
  parameter: bearer
  sources:
  - openapi/tribe-payments-trb-risk-monitor-client-api-openapi.json
  type: apiKey
- description: Value for the X-AUTH-TOKEN header parameter.
  in: header
  name: Token
  parameter: X-AUTH-TOKEN
  sources:
  - openapi/tribe-payments-trb-risk-monitor-client-api-openapi.json
  type: apiKey
slug: tribe-payments-authentication
source_filename: tribe-payments-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-24'\nmethod: derived\nsource: openapi/tribe-payments-obb-tpp-api-openapi.json, openapi/tribe-payments-trb-cc-api-merchant-api-credit-card-callback-v3.json,\n  openapi/tribe-payments-trb-cc-api-merchant-api-credit-card-v3.json, openapi/tribe-payments-trb-cc-token-api-merchant-api-credit-card-token-v3.json,\n  openapi/tribe-payments-trb-cc-token-api-merchant-api-credit-card-token-webhook-v3.json, openapi/tribe-payments-trb-hpp-api-merchant-api-hpp-v3.json,\n  openapi/tribe-payments-trb-hpp-api-merchant-api-hpp-webhook-v3.json, openapi/tribe-payments-trb-report-api-merchant-api-report-callback-v3.json,\n  openapi/tribe-payments-trb-report-api-merchant-api-report-v3.json, openapi/tribe-payments-trb-risk-monitor-client-api-openapi.json\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: tokenAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/tribe-payments-obb-tpp-api-openapi.json\n- name: clientId\n  type: apiKey\n\
  \  in: header\n  parameter: X-Client-ID\n  sources:\n  - openapi/tribe-payments-obb-tpp-api-openapi.json\n- name: accountId\n  type: apiKey\n  in: header\n  parameter: x-auth-account-id\n  sources:\n  - openapi/tribe-payments-trb-cc-api-merchant-api-credit-card-callback-v3.json\n  - openapi/tribe-payments-trb-cc-api-merchant-api-credit-card-v3.json\n  - openapi/tribe-payments-trb-cc-token-api-merchant-api-credit-card-token-v3.json\n  - openapi/tribe-payments-trb-cc-token-api-merchant-api-credit-card-token-webhook-v3.json\n  - openapi/tribe-payments-trb-hpp-api-merchant-api-hpp-v3.json\n  - openapi/tribe-payments-trb-hpp-api-merchant-api-hpp-webhook-v3.json\n- name: accountPassword\n  type: apiKey\n  in: header\n  parameter: x-auth-account-password\n  sources:\n  - openapi/tribe-payments-trb-cc-api-merchant-api-credit-card-callback-v3.json\n  - openapi/tribe-payments-trb-cc-api-merchant-api-credit-card-v3.json\n  - openapi/tribe-payments-trb-cc-token-api-merchant-api-credit-card-token-v3.json\n\
  \  - openapi/tribe-payments-trb-cc-token-api-merchant-api-credit-card-token-webhook-v3.json\n  - openapi/tribe-payments-trb-hpp-api-merchant-api-hpp-v3.json\n  - openapi/tribe-payments-trb-hpp-api-merchant-api-hpp-webhook-v3.json\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: x-auth-report-api-key\n  sources:\n  - openapi/tribe-payments-trb-report-api-merchant-api-report-callback-v3.json\n  - openapi/tribe-payments-trb-report-api-merchant-api-report-v3.json\n- name: apiPassword\n  type: apiKey\n  in: header\n  parameter: x-auth-report-api-password\n  sources:\n  - openapi/tribe-payments-trb-report-api-merchant-api-report-callback-v3.json\n  - openapi/tribe-payments-trb-report-api-merchant-api-report-v3.json\n- name: Bearer\n  type: apiKey\n  in: header\n  parameter: bearer\n  description: Value for the bearer header parameter.\n  sources:\n  - openapi/tribe-payments-trb-risk-monitor-client-api-openapi.json\n- name: Token\n  type: apiKey\n  in: header\n  parameter: X-AUTH-TOKEN\n\
  \  description: Value for the X-AUTH-TOKEN header parameter.\n  sources:\n  - openapi/tribe-payments-trb-risk-monitor-client-api-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tribe-payments/refs/heads/main/authentication/tribe-payments-authentication.yml
summary_line: apiKey/http · 8 schemes
tags:
- Payments
- United Kingdom
- Issuer Processor
- Card Issuing
- Acquiring
- Payment Gateway
- Payment Processing
- Open Banking
- Account-to-Account
- Banking-as-a-Service
- Fraud
- Point of Sale
---
