---
api_key_in:
- header
api_specs:
- filename: interswitch-web-checkout-api-openapi.yml
  format: yaml
  label: Interswitch Web Checkout API
  slug: interswitch-web-checkout-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/interswitch/refs/heads/main/openapi/interswitch-web-checkout-api-openapi.yml
- filename: interswitch-payment-gateway-api-openapi.yml
  format: yaml
  label: Interswitch Payment Gateway API
  slug: interswitch-payment-gateway-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/interswitch/refs/heads/main/openapi/interswitch-payment-gateway-api-openapi.yml
- filename: interswitch-transfers-api-openapi.yml
  format: yaml
  label: Interswitch Transfers API
  slug: interswitch-transfers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/interswitch/refs/heads/main/openapi/interswitch-transfers-api-openapi.yml
- filename: interswitch-bills-payment-api-openapi.yml
  format: yaml
  label: Interswitch Bills Payment API
  slug: interswitch-bills-payment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/interswitch/refs/heads/main/openapi/interswitch-bills-payment-api-openapi.yml
- filename: interswitch-airtime-recharge-api-openapi.yml
  format: yaml
  label: Interswitch Airtime Recharge API
  slug: interswitch-airtime-recharge-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/interswitch/refs/heads/main/openapi/interswitch-airtime-recharge-api-openapi.yml
- filename: interswitch-paycode-api-openapi.yml
  format: yaml
  label: Interswitch Paycode API
  slug: interswitch-paycode-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/interswitch/refs/heads/main/openapi/interswitch-paycode-api-openapi.yml
- filename: interswitch-refunds-api-openapi.yml
  format: yaml
  label: Interswitch Refunds API
  slug: interswitch-refunds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/interswitch/refs/heads/main/openapi/interswitch-refunds-api-openapi.yml
- filename: interswitch-recurring-payments-api-openapi.yml
  format: yaml
  label: Interswitch Recurring Payments API
  slug: interswitch-recurring-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/interswitch/refs/heads/main/openapi/interswitch-recurring-payments-api-openapi.yml
- filename: interswitch-card-360-api-openapi.yml
  format: yaml
  label: Interswitch Card 360 API
  slug: interswitch-card-360-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/interswitch/refs/heads/main/openapi/interswitch-card-360-api-openapi.yml
- filename: interswitch-lending-api-openapi.yml
  format: yaml
  label: Interswitch Lending API
  slug: interswitch-lending-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/interswitch/refs/heads/main/openapi/interswitch-lending-api-openapi.yml
- filename: interswitch-customer-insights-api-openapi.yml
  format: yaml
  label: Interswitch Customer Insights API
  slug: interswitch-customer-insights-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/interswitch/refs/heads/main/openapi/interswitch-customer-insights-api-openapi.yml
- filename: interswitch-transaction-search-api-openapi.yml
  format: yaml
  label: Interswitch Transaction Search API
  slug: interswitch-transaction-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/interswitch/refs/heads/main/openapi/interswitch-transaction-search-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Interswitch Authentication
name_suffix: Authentication
oauth_flows: []
overview: Interswitch secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Interswitch
provider_slug: interswitch
scheme_count: 2
schemes:
- in: header
  name: InterswitchAuth
  parameter: Authorization
  sources:
  - openapi/interswitch-airtime-recharge-api-openapi.yml
  - openapi/interswitch-bills-payment-api-openapi.yml
  - openapi/interswitch-web-checkout-api-openapi.yml
  type: apiKey
- name: BearerAuth
  scheme: bearer
  sources:
  - openapi/interswitch-card-360-api-openapi.yml
  - openapi/interswitch-customer-insights-api-openapi.yml
  - openapi/interswitch-lending-api-openapi.yml
  - openapi/interswitch-paycode-api-openapi.yml
  - openapi/interswitch-payment-gateway-api-openapi.yml
  - openapi/interswitch-recurring-payments-api-openapi.yml
  - openapi/interswitch-refunds-api-openapi.yml
  - openapi/interswitch-transaction-search-api-openapi.yml
  - openapi/interswitch-transfers-api-openapi.yml
  type: http
slug: interswitch-authentication
source_filename: interswitch-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/interswitch-airtime-recharge-api-openapi.yml, openapi/interswitch-bills-payment-api-openapi.yml,\n  openapi/interswitch-card-360-api-openapi.yml, openapi/interswitch-customer-insights-api-openapi.yml,\n  openapi/interswitch-lending-api-openapi.yml, openapi/interswitch-paycode-api-openapi.yml,\n  openapi/interswitch-payment-gateway-api-openapi.yml, openapi/interswitch-recurring-payments-api-openapi.yml,\n  openapi/interswitch-refunds-api-openapi.yml, openapi/interswitch-transaction-search-api-openapi.yml,\n  openapi/interswitch-transfers-api-openapi.yml, openapi/interswitch-web-checkout-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: InterswitchAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  sources:\n  - openapi/interswitch-airtime-recharge-api-openapi.yml\n  - openapi/interswitch-bills-payment-api-openapi.yml\n  - openapi/interswitch-web-checkout-api-openapi.yml\n\
  - name: BearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/interswitch-card-360-api-openapi.yml\n  - openapi/interswitch-customer-insights-api-openapi.yml\n  - openapi/interswitch-lending-api-openapi.yml\n  - openapi/interswitch-paycode-api-openapi.yml\n  - openapi/interswitch-payment-gateway-api-openapi.yml\n  - openapi/interswitch-recurring-payments-api-openapi.yml\n  - openapi/interswitch-refunds-api-openapi.yml\n  - openapi/interswitch-transaction-search-api-openapi.yml\n  - openapi/interswitch-transfers-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/interswitch/refs/heads/main/authentication/interswitch-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Payments
- Payment Infrastructure
- Card Network
- Verve
- Quickteller
- Webpay
- Bills Payment
- Transfers
- Lending
- Fintech
- Africa
- Nigeria
---
