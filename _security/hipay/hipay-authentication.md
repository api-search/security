---
api_key_in:
- header
api_specs:
- filename: hipay-balance-api-openapi.yml
  format: yaml
  label: HiPay balance API
  slug: hipay-balance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hipay/refs/heads/main/openapi/hipay-balance-api-openapi.yml
- filename: hipay-bank-info-api-openapi.yml
  format: yaml
  label: HiPay bank-info API
  slug: hipay-bank-info-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hipay/refs/heads/main/openapi/hipay-bank-info-api-openapi.yml
- filename: hipay-captcha-generation-api-openapi.yml
  format: yaml
  label: HiPay captcha-generation API
  slug: hipay-captcha-generation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hipay/refs/heads/main/openapi/hipay-captcha-generation-api-openapi.yml
- filename: hipay-connector-api-openapi.yml
  format: yaml
  label: HiPay Connector API
  slug: hipay-connector-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hipay/refs/heads/main/openapi/hipay-connector-api-openapi.yml
- filename: hipay-constants-api-openapi.yml
  format: yaml
  label: HiPay constants API
  slug: hipay-constants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hipay/refs/heads/main/openapi/hipay-constants-api-openapi.yml
- filename: hipay-identification-api-openapi.yml
  format: yaml
  label: HiPay identification API
  slug: hipay-identification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hipay/refs/heads/main/openapi/hipay-identification-api-openapi.yml
- filename: hipay-invoice-api-openapi.yml
  format: yaml
  label: HiPay invoice API
  slug: hipay-invoice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hipay/refs/heads/main/openapi/hipay-invoice-api-openapi.yml
- filename: hipay-maintenance-api-openapi.yml
  format: yaml
  label: HiPay maintenance API
  slug: hipay-maintenance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hipay/refs/heads/main/openapi/hipay-maintenance-api-openapi.yml
- filename: hipay-merchant-group-api-openapi.yml
  format: yaml
  label: HiPay merchant-group API
  slug: hipay-merchant-group-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hipay/refs/heads/main/openapi/hipay-merchant-group-api-openapi.yml
- filename: hipay-order-api-openapi.yml
  format: yaml
  label: HiPay Order API
  slug: hipay-order-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hipay/refs/heads/main/openapi/hipay-order-api-openapi.yml
- filename: hipay-payments-api-openapi.yml
  format: yaml
  label: HiPay payments API
  slug: hipay-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hipay/refs/heads/main/openapi/hipay-payments-api-openapi.yml
- filename: hipay-routing-api-openapi.yml
  format: yaml
  label: HiPay Routing API
  slug: hipay-routing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hipay/refs/heads/main/openapi/hipay-routing-api-openapi.yml
- filename: hipay-sessions-api-openapi.yml
  format: yaml
  label: HiPay Sessions API
  slug: hipay-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hipay/refs/heads/main/openapi/hipay-sessions-api-openapi.yml
- filename: hipay-settlement-api-openapi.yml
  format: yaml
  label: HiPay settlement API
  slug: hipay-settlement-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hipay/refs/heads/main/openapi/hipay-settlement-api-openapi.yml
- filename: hipay-tokenization-api-openapi.yml
  format: yaml
  label: HiPay tokenization API
  slug: hipay-tokenization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hipay/refs/heads/main/openapi/hipay-tokenization-api-openapi.yml
- filename: hipay-transaction-api-openapi.yml
  format: yaml
  label: HiPay Transaction API
  slug: hipay-transaction-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hipay/refs/heads/main/openapi/hipay-transaction-api-openapi.yml
- filename: hipay-transfer-api-openapi.yml
  format: yaml
  label: HiPay transfer API
  slug: hipay-transfer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hipay/refs/heads/main/openapi/hipay-transfer-api-openapi.yml
- filename: hipay-ubo-api-openapi.yml
  format: yaml
  label: HiPay ubo API
  slug: hipay-ubo-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hipay/refs/heads/main/openapi/hipay-ubo-api-openapi.yml
- filename: hipay-user-account-api-openapi.yml
  format: yaml
  label: HiPay user-account API
  slug: hipay-user-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hipay/refs/heads/main/openapi/hipay-user-account-api-openapi.yml
- filename: hipay-withdrawal-api-openapi.yml
  format: yaml
  label: HiPay withdrawal API
  slug: hipay-withdrawal-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hipay/refs/heads/main/openapi/hipay-withdrawal-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Hipay Authentication
name_suffix: Authentication
oauth_flows: []
overview: HiPay secures its APIs with apiKey and http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: HiPay
provider_slug: hipay
scheme_count: 3
schemes:
- name: BasicAuth
  scheme: basic
  sources:
  - openapi/api-gateway.yml
  - openapi/gateway.yaml
  - openapi/hpayment.yaml
  - openapi/marketplace.yaml
  - openapi/omnichannel.yaml
  - openapi/pos-api.yaml
  - openapi/settlement.yaml
  - openapi/tokenization.yaml
  type: http
- in: header
  name: ApiKeyAuth
  parameter: X-API-KEY
  sources:
  - openapi/api-gateway.yml
  type: apiKey
- in: header
  name: apiKey
  parameter: X-Api-Key
  sources:
  - openapi/gateway.yaml
  type: apiKey
slug: hipay-authentication
source_filename: hipay-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/api-gateway.yml, openapi/gateway.yaml, openapi/hpayment.yaml, openapi/marketplace.yaml,\n  openapi/omnichannel.yaml, openapi/pos-api.yaml, openapi/settlement.yaml, openapi/tokenization.yaml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: BasicAuth\n  type: http\n  scheme: basic\n  sources:\n  - openapi/api-gateway.yml\n  - openapi/gateway.yaml\n  - openapi/hpayment.yaml\n  - openapi/marketplace.yaml\n  - openapi/omnichannel.yaml\n  - openapi/pos-api.yaml\n  - openapi/settlement.yaml\n  - openapi/tokenization.yaml\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-KEY\n  sources:\n  - openapi/api-gateway.yml\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: X-Api-Key\n  sources:\n  - openapi/gateway.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hipay/refs/heads/main/authentication/hipay-authentication.yml
summary_line: apiKey/http · 3 schemes
tags:
- Payments
- Fintech
- Europe
- Omnichannel
- Point-of-Sale
- Fraud Prevention
- Tokenization
- Marketplace
---
