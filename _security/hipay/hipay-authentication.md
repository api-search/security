---
api_key_in:
- header
api_specs:
- filename: api-gateway.yml
  format: yaml
  label: HiPay Payment Gateway API
  slug: hipay-payment-gateway-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/hipay/openapi-hipay/master/enterprise/api-gateway.yml
- filename: gateway.yaml
  format: yaml
  label: HiPay Enterprise Gateway API
  slug: hipay-enterprise-gateway-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/hipay/openapi-hipay/master/enterprise/gateway.yaml
- filename: hpayment.yaml
  format: yaml
  label: HiPay Enterprise HostedPage API
  slug: hipay-enterprise-hostedpage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/hipay/openapi-hipay/master/enterprise/hpayment.yaml
- filename: settlement.yaml
  format: yaml
  label: HiPay Enterprise Finance API
  slug: hipay-enterprise-finance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/hipay/openapi-hipay/master/enterprise/settlement.yaml
- filename: tokenization.yaml
  format: yaml
  label: HiPay Enterprise Tokenization API
  slug: hipay-enterprise-tokenization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/hipay/openapi-hipay/master/enterprise/tokenization.yaml
- filename: applepay-web.yaml
  format: yaml
  label: HiPay Apple Pay Web API
  slug: hipay-apple-pay-web-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/hipay/openapi-hipay/master/enterprise/applepay-web.yaml
- filename: pos_api.yaml
  format: yaml
  label: HiPay POS API
  slug: hipay-pos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/hipay/openapi-hipay/master/omnichannel/pos_api.yaml
- filename: omnichannel.yaml
  format: yaml
  label: HiPay Omnichannel Gateway API
  slug: hipay-omnichannel-gateway-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/hipay/openapi-hipay/master/omnichannel/omnichannel.yaml
- filename: marketplace.yaml
  format: yaml
  label: HiPay Marketplace API
  slug: hipay-marketplace-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/hipay/openapi-hipay/master/marketplace/marketplace.yaml
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
- Point of Sale
- Fraud Prevention
- Tokenization
- Marketplace
---
