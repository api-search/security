---
api_key_in:
- header
api_specs:
- filename: kushki-card-payments-api-openapi.yml
  format: yaml
  label: Kushki Card Payments API
  slug: kushki-card-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kushki/refs/heads/main/openapi/kushki-card-payments-api-openapi.yml
- filename: kushki-subscriptions-api-openapi.yml
  format: yaml
  label: Kushki Subscriptions API
  slug: kushki-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kushki/refs/heads/main/openapi/kushki-subscriptions-api-openapi.yml
- filename: kushki-transfer-payments-api-openapi.yml
  format: yaml
  label: Kushki Transfer Payments API
  slug: kushki-transfer-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kushki/refs/heads/main/openapi/kushki-transfer-payments-api-openapi.yml
- filename: kushki-cash-payments-api-openapi.yml
  format: yaml
  label: Kushki Cash Payments API
  slug: kushki-cash-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kushki/refs/heads/main/openapi/kushki-cash-payments-api-openapi.yml
- filename: kushki-payouts-api-openapi.yml
  format: yaml
  label: Kushki Payouts API
  slug: kushki-payouts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kushki/refs/heads/main/openapi/kushki-payouts-api-openapi.yml
- filename: kushki-card-present-api-openapi.yml
  format: yaml
  label: Kushki Card Present API
  slug: kushki-card-present-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kushki/refs/heads/main/openapi/kushki-card-present-api-openapi.yml
- filename: kushki-merchants-api-openapi.yml
  format: yaml
  label: Kushki Merchants and Branches API
  slug: kushki-merchants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kushki/refs/heads/main/openapi/kushki-merchants-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Kushki Authentication
name_suffix: Authentication
oauth_flows: []
overview: Kushki secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Kushki
provider_slug: kushki
scheme_count: 2
schemes:
- description: Client-side merchant key. Used by Kushki.js and mobile SDKs to tokenize cards. Never use server-side for charging.
  in: header
  name: PublicMerchantId
  parameter: Public-Merchant-Id
  sources:
  - openapi/kushki-card-payments-api-openapi.yml
  - openapi/kushki-transfer-payments-api-openapi.yml
  type: apiKey
- description: Server-side merchant key. Required for charge, capture, void, refund, subscription, and payout calls.
  in: header
  name: PrivateMerchantId
  parameter: Private-Merchant-Id
  sources:
  - openapi/kushki-card-payments-api-openapi.yml
  - openapi/kushki-card-present-api-openapi.yml
  - openapi/kushki-cash-payments-api-openapi.yml
  - openapi/kushki-merchants-api-openapi.yml
  - openapi/kushki-payouts-api-openapi.yml
  - openapi/kushki-subscriptions-api-openapi.yml
  - openapi/kushki-transfer-payments-api-openapi.yml
  type: apiKey
slug: kushki-authentication
source_filename: kushki-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/kushki-card-payments-api-openapi.yml, openapi/kushki-card-present-api-openapi.yml,\n  openapi/kushki-cash-payments-api-openapi.yml, openapi/kushki-merchants-api-openapi.yml, openapi/kushki-payouts-api-openapi.yml,\n  openapi/kushki-subscriptions-api-openapi.yml, openapi/kushki-transfer-payments-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: PublicMerchantId\n  type: apiKey\n  in: header\n  parameter: Public-Merchant-Id\n  description: Client-side merchant key. Used by Kushki.js and mobile SDKs to tokenize cards.\n    Never use server-side for charging.\n  sources:\n  - openapi/kushki-card-payments-api-openapi.yml\n  - openapi/kushki-transfer-payments-api-openapi.yml\n- name: PrivateMerchantId\n  type: apiKey\n  in: header\n  parameter: Private-Merchant-Id\n  description: Server-side merchant key. Required for charge, capture, void, refund, subscription,\n    and payout calls.\n\
  \  sources:\n  - openapi/kushki-card-payments-api-openapi.yml\n  - openapi/kushki-card-present-api-openapi.yml\n  - openapi/kushki-cash-payments-api-openapi.yml\n  - openapi/kushki-merchants-api-openapi.yml\n  - openapi/kushki-payouts-api-openapi.yml\n  - openapi/kushki-subscriptions-api-openapi.yml\n  - openapi/kushki-transfer-payments-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kushki/refs/heads/main/authentication/kushki-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Payments
- LatAm
- Andean Region
- Card Payments
- Subscriptions
- Cash
- Bank Transfers
- Payouts
- PSE
- Webpay
- SPEI
- PIX
- OXXO
- PagoEfectivo
- Fintech
- Ecuador
- Colombia
- Peru
- Chile
- Mexico
- Brazil
---
