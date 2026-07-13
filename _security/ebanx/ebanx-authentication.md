---
api_key_in:
- header
api_specs:
- filename: ebanx-pay-in-direct-api-openapi.yml
  format: yaml
  label: EBANX Pay-in Direct API
  slug: ebanx-pay-in-direct-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ebanx/refs/heads/main/openapi/ebanx-pay-in-direct-api-openapi.yml
- filename: ebanx-payment-page-api-openapi.yml
  format: yaml
  label: EBANX Payment Page API
  slug: ebanx-payment-page-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ebanx/refs/heads/main/openapi/ebanx-payment-page-api-openapi.yml
- filename: ebanx-tokenization-api-openapi.yml
  format: yaml
  label: EBANX Tokenization API
  slug: ebanx-tokenization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ebanx/refs/heads/main/openapi/ebanx-tokenization-api-openapi.yml
- filename: ebanx-fx-api-openapi.yml
  format: yaml
  label: EBANX FX API
  slug: ebanx-fx-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ebanx/refs/heads/main/openapi/ebanx-fx-api-openapi.yml
- filename: ebanx-payout-api-openapi.yml
  format: yaml
  label: EBANX Payout API
  slug: ebanx-payout-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ebanx/refs/heads/main/openapi/ebanx-payout-api-openapi.yml
- filename: ebanx-notifications-asyncapi.yml
  format: yaml
  label: EBANX Payment Notifications
  slug: ebanx-notifications
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/ebanx/refs/heads/main/asyncapi/ebanx-notifications-asyncapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Ebanx Authentication
name_suffix: Authentication
oauth_flows: []
overview: EBANX secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: EBANX
provider_slug: ebanx
scheme_count: 1
schemes:
- in: header
  name: integrationKey
  parameter: x-ebanx-integration-key
  sources:
  - openapi/ebanx-fx-api-openapi.yml
  - openapi/ebanx-pay-in-direct-api-openapi.yml
  - openapi/ebanx-payment-page-api-openapi.yml
  - openapi/ebanx-payout-api-openapi.yml
  - openapi/ebanx-tokenization-api-openapi.yml
  type: apiKey
slug: ebanx-authentication
source_filename: ebanx-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/ebanx-fx-api-openapi.yml, openapi/ebanx-pay-in-direct-api-openapi.yml, openapi/ebanx-payment-page-api-openapi.yml,\n  openapi/ebanx-payout-api-openapi.yml, openapi/ebanx-tokenization-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: integrationKey\n  type: apiKey\n  in: header\n  parameter: x-ebanx-integration-key\n  sources:\n  - openapi/ebanx-fx-api-openapi.yml\n  - openapi/ebanx-pay-in-direct-api-openapi.yml\n  - openapi/ebanx-payment-page-api-openapi.yml\n  - openapi/ebanx-payout-api-openapi.yml\n  - openapi/ebanx-tokenization-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ebanx/refs/heads/main/authentication/ebanx-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Payments
- Pay-in
- Payouts
- Foreign Exchange
- Tokenization
- LATAM
- Emerging Markets
- Pix
- Boleto
- OXXO
- SPEI
- PSE
- Cross-Border
- Webhooks
---
