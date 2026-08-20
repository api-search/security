---
api_key_in: []
api_specs:
- filename: payu-authorize-api-openapi.yml
  format: yaml
  label: PayU Authorize API
  slug: payu-authorize-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payu/refs/heads/main/openapi/payu-authorize-api-openapi.yml
- filename: payu-card-installments-api-openapi.yml
  format: yaml
  label: PayU Card Installments API
  slug: payu-card-installments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payu/refs/heads/main/openapi/payu-card-installments-api-openapi.yml
- filename: payu-fx-reference-api-openapi.yml
  format: yaml
  label: PayU FX-Reference API
  slug: payu-fx-reference-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payu/refs/heads/main/openapi/payu-fx-reference-api-openapi.yml
- filename: payu-marketplace-seller-api-openapi.yml
  format: yaml
  label: PayU Marketplace-Seller API
  slug: payu-marketplace-seller-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payu/refs/heads/main/openapi/payu-marketplace-seller-api-openapi.yml
- filename: payu-marketplace-verification-api-openapi.yml
  format: yaml
  label: PayU Marketplace-Verification API
  slug: payu-marketplace-verification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payu/refs/heads/main/openapi/payu-marketplace-verification-api-openapi.yml
- filename: payu-mcp-api-openapi.yml
  format: yaml
  label: PayU MCP API
  slug: payu-mcp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payu/refs/heads/main/openapi/payu-mcp-api-openapi.yml
- filename: payu-order-api-openapi.yml
  format: yaml
  label: PayU Order API
  slug: payu-order-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payu/refs/heads/main/openapi/payu-order-api-openapi.yml
- filename: payu-partner-merchant-registration-api-openapi.yml
  format: yaml
  label: PayU Partner-Merchant-Registration API
  slug: payu-partner-merchant-registration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payu/refs/heads/main/openapi/payu-partner-merchant-registration-api-openapi.yml
- filename: payu-payment-methods-api-openapi.yml
  format: yaml
  label: PayU Payment-Methods API
  slug: payu-payment-methods-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payu/refs/heads/main/openapi/payu-payment-methods-api-openapi.yml
- filename: payu-payout-api-openapi.yml
  format: yaml
  label: PayU Payout API
  slug: payu-payout-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payu/refs/heads/main/openapi/payu-payout-api-openapi.yml
- filename: payu-pf-submerchant-registration-api-openapi.yml
  format: yaml
  label: PayU PF-Submerchant-Registration API
  slug: payu-pf-submerchant-registration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payu/refs/heads/main/openapi/payu-pf-submerchant-registration-api-openapi.yml
- filename: payu-refund-api-openapi.yml
  format: yaml
  label: PayU Refund API
  slug: payu-refund-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payu/refs/heads/main/openapi/payu-refund-api-openapi.yml
- filename: payu-shop-api-openapi.yml
  format: yaml
  label: PayU Shop API
  slug: payu-shop-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payu/refs/heads/main/openapi/payu-shop-api-openapi.yml
- filename: payu-statements-api-openapi.yml
  format: yaml
  label: PayU Statements API
  slug: payu-statements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payu/refs/heads/main/openapi/payu-statements-api-openapi.yml
- filename: payu-token-api-openapi.yml
  format: yaml
  label: PayU Token API
  slug: payu-token-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payu/refs/heads/main/openapi/payu-token-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Payu Authentication
name_suffix: Authentication
oauth_flows: []
overview: PayU secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: PayU
provider_slug: payu
scheme_count: 2
schemes:
- name: Bearer
  scheme: bearer
  sources:
  - openapi/payu-europe-rest-api.yaml
  type: http
- name: Basic
  scheme: basic
  sources:
  - openapi/payu-europe-rest-api.yaml
  type: http
slug: payu-authentication
source_filename: payu-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/payu-europe-rest-api.yaml\nsummary:\n  types:\n  - http\nschemes:\n- name: Bearer\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/payu-europe-rest-api.yaml\n- name: Basic\n  type: http\n  scheme: basic\n  sources:\n  - openapi/payu-europe-rest-api.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/payu/refs/heads/main/authentication/payu-authentication.yml
summary_line: http · 2 schemes
tags:
- Payments
- Payment Processing
- Fintech
- Financial-Services
- Subscription
- Fraud Detection
- Checkout
- Marketplace
- Tokenization
- Emerging Markets
---
