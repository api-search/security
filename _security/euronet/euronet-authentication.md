---
api_key_in:
- header
api_specs:
- filename: xe-currency-data-api-openapi.json
  format: json
  label: Xe Currency Data API
  slug: xe-currency-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/euronet/refs/heads/main/openapi/xe-currency-data-api-openapi.json
- filename: xe-payments-api-openapi.json
  format: json
  label: Xe Payments API
  slug: xe-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/euronet/refs/heads/main/openapi/xe-payments-api-openapi.json
- filename: xe-mass-payments-api-openapi.json
  format: json
  label: Xe Mass Payments API
  slug: xe-mass-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/euronet/refs/heads/main/openapi/xe-mass-payments-api-openapi.json
- filename: xe-currency-data-tradable-rates-api-openapi.json
  format: json
  label: Xe Currency Data Tradable Rates API
  slug: xe-currency-data-tradable-rates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/euronet/refs/heads/main/openapi/xe-currency-data-tradable-rates-api-openapi.json
- filename: xeta-api-openapi.json
  format: json
  label: XETA API
  slug: xeta-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/euronet/refs/heads/main/openapi/xeta-api-openapi.json
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Euronet Authentication
name_suffix: Authentication
oauth_flows: []
overview: Euronet Worldwide secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Euronet Worldwide
provider_slug: euronet
scheme_count: 2
schemes:
- name: basicAuth
  scheme: basic
  sources:
  - openapi/xe-currency-data-api-openapi.json
  type: http
- in: header
  name: xeta-drupal-authorizer
  parameter: Cookie
  sources:
  - openapi/xeta-api-openapi.json
  type: apiKey
slug: euronet-authentication
source_filename: euronet-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-24'\nmethod: derived\nsource: openapi/xe-currency-data-api-openapi.json, openapi/xeta-api-openapi.json\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  sources:\n  - openapi/xe-currency-data-api-openapi.json\n- name: xeta-drupal-authorizer\n  type: apiKey\n  in: header\n  parameter: Cookie\n  sources:\n  - openapi/xeta-api-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/euronet/refs/heads/main/authentication/euronet-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Payments
- United States
- Payment Processing
- Cross-Border
- Money Transfer
- Currency Exchange
- FX
- Payouts
- Real-Time Payments
- ISO 20022
- Acquiring
---
