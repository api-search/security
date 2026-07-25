---
api_key_in: []
api_specs:
- filename: fat-zebra-gateway.json
  format: json
  label: Fat Zebra Gateway API
  slug: fat-zebra-gateway-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fat-zebra/refs/heads/main/openapi/fat-zebra-gateway.json
- filename: fat-zebra-partner.json
  format: json
  label: Fat Zebra Partner API
  slug: fat-zebra-partner-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fat-zebra/refs/heads/main/openapi/fat-zebra-partner.json
- filename: fat-zebra-billing.json
  format: json
  label: Fat Zebra Billing API
  slug: fat-zebra-billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fat-zebra/refs/heads/main/openapi/fat-zebra-billing.json
- filename: fat-zebra-fdms-tpp-merchant-onboarding.json
  format: json
  label: Fat Zebra FDMS TPP Merchant Onboarding API
  slug: fat-zebra-fdms-tpp-merchant-onboarding-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fat-zebra/refs/heads/main/openapi/fat-zebra-fdms-tpp-merchant-onboarding.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Fat Zebra Authentication
name_suffix: Authentication
oauth_flows: []
overview: Fat Zebra secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Fat Zebra
provider_slug: fat-zebra
scheme_count: 1
schemes:
- name: sec0
  scheme: basic
  sources:
  - openapi/fat-zebra-billing.json
  - openapi/fat-zebra-fdms-tpp-merchant-onboarding.json
  - openapi/fat-zebra-gateway.json
  - openapi/fat-zebra-partner.json
  type: http
slug: fat-zebra-authentication
source_filename: fat-zebra-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-24'\nmethod: derived\nsource: openapi/fat-zebra-billing.json, openapi/fat-zebra-fdms-tpp-merchant-onboarding.json,\n  openapi/fat-zebra-gateway.json, openapi/fat-zebra-partner.json\nsummary:\n  types:\n  - http\nschemes:\n- name: sec0\n  type: http\n  scheme: basic\n  sources:\n  - openapi/fat-zebra-billing.json\n  - openapi/fat-zebra-fdms-tpp-merchant-onboarding.json\n  - openapi/fat-zebra-gateway.json\n  - openapi/fat-zebra-partner.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fat-zebra/refs/heads/main/authentication/fat-zebra-authentication.yml
summary_line: http · 1 scheme
tags:
- Payments
- Australia
- Payment Gateway
- Payment Processing
- Acquiring
- Card Payments
- Tokenization
- Recurring Billing
- Direct Debit
- Hosted Payment Pages
- Merchant Onboarding
---
