---
api_key_in: []
api_specs:
- filename: openapi
  format: yaml
  label: Worldpay Card Payments API
  slug: worldpay-card-payments-api
  spec_type: OpenAPI
  url: https://docs.worldpay.com/access/products/payments/openapi
- filename: openapi
  format: yaml
  label: Worldpay Payment Queries API
  slug: worldpay-payment-queries-api
  spec_type: OpenAPI
  url: https://developer.worldpay.com/products/access/payment-queries/openapi
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Worldpay Authentication
name_suffix: Authentication
oauth_flows: []
overview: Worldpay secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Worldpay
provider_slug: worldpay
scheme_count: 2
schemes:
- name: BasicAuth
  scheme: basic
  sources:
  - openapi/worldpay-3ds-openapi.yaml
  - openapi/worldpay-account-payouts-openapi.yaml
  - openapi/worldpay-apms-openapi.yaml
  - openapi/worldpay-balance-openapi.yaml
  - openapi/worldpay-card-payments-openapi.yaml
  - openapi/worldpay-card-payouts-openapi.yaml
  - openapi/worldpay-card-verifications-openapi.yaml
  - openapi/worldpay-fraudsight-openapi.yaml
  - openapi/worldpay-fx-openapi.yaml
  - openapi/worldpay-money-transfers-openapi.yaml
  - openapi/worldpay-parties-openapi.yaml
  - openapi/worldpay-payment-queries-openapi.yaml
  - openapi/worldpay-payments-openapi.yaml
  - openapi/worldpay-sca-exemptions-openapi.yaml
  - openapi/worldpay-split-payments-openapi.yaml
  - openapi/worldpay-statements-openapi.yaml
  - openapi/worldpay-tokens-openapi.yaml
  - openapi/worldpay-transfers-openapi.yaml
  - openapi/worldpay-verified-tokens-openapi.yaml
  type: http
- name: BasicAuth
  scheme: BasicAuth
  sources:
  - openapi/worldpay-hosted-payment-pages-openapi.yaml
  type: http
slug: worldpay-authentication
source_filename: worldpay-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/worldpay-3ds-openapi.yaml, openapi/worldpay-account-payouts-openapi.yaml, openapi/worldpay-apms-openapi.yaml,\n  openapi/worldpay-balance-openapi.yaml, openapi/worldpay-card-payments-openapi.yaml, openapi/worldpay-card-payouts-openapi.yaml,\n  openapi/worldpay-card-verifications-openapi.yaml, openapi/worldpay-fraudsight-openapi.yaml,\n  openapi/worldpay-fx-openapi.yaml, openapi/worldpay-hosted-payment-pages-openapi.yaml, openapi/worldpay-money-transfers-openapi.yaml,\n  openapi/worldpay-parties-openapi.yaml ...\nsummary:\n  types:\n  - http\nschemes:\n- name: BasicAuth\n  type: http\n  scheme: basic\n  sources:\n  - openapi/worldpay-3ds-openapi.yaml\n  - openapi/worldpay-account-payouts-openapi.yaml\n  - openapi/worldpay-apms-openapi.yaml\n  - openapi/worldpay-balance-openapi.yaml\n  - openapi/worldpay-card-payments-openapi.yaml\n  - openapi/worldpay-card-payouts-openapi.yaml\n  - openapi/worldpay-card-verifications-openapi.yaml\n\
  \  - openapi/worldpay-fraudsight-openapi.yaml\n  - openapi/worldpay-fx-openapi.yaml\n  - openapi/worldpay-money-transfers-openapi.yaml\n  - openapi/worldpay-parties-openapi.yaml\n  - openapi/worldpay-payment-queries-openapi.yaml\n  - openapi/worldpay-payments-openapi.yaml\n  - openapi/worldpay-sca-exemptions-openapi.yaml\n  - openapi/worldpay-split-payments-openapi.yaml\n  - openapi/worldpay-statements-openapi.yaml\n  - openapi/worldpay-tokens-openapi.yaml\n  - openapi/worldpay-transfers-openapi.yaml\n  - openapi/worldpay-verified-tokens-openapi.yaml\n- name: BasicAuth\n  type: http\n  scheme: BasicAuth\n  sources:\n  - openapi/worldpay-hosted-payment-pages-openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/worldpay/refs/heads/main/authentication/worldpay-authentication.yml
summary_line: http · 2 schemes
tags:
- Payments
- Payment Processing
- Payment Gateway
- Tokenization
- Fraud Prevention
- Recurring Billing
- Payouts
- Foreign Exchange
- Financial Services
- Fintech
---
