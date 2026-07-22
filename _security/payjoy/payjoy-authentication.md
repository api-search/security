---
api_key_in:
- header
api_specs:
- filename: payjoy-partner-api-openapi.yml
  format: yaml
  label: PayJoy Partner API V2 (Sales Integration)
  slug: payjoy-partner-api-v2-sales-integration
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payjoy/refs/heads/main/openapi/payjoy-partner-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: searched
name: Payjoy Authentication
name_suffix: Authentication
oauth_flows: []
overview: PayJoy secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: PayJoy
provider_slug: payjoy
scheme_count: 2
schemes:
- api: PayJoy Partner API V2 (Sales Integration)
  description: API key required to authenticate all requests. Include this key in the request header as `X-PayJoy-ApiKey`.
  in: header
  name: PayJoyApiKeyAuth
  parameter: X-PayJoy-ApiKey
  provisioning: Partner Console (https://app.payjoy.com/admin-console/login) -> API -> New
  sources:
  - openapi/payjoy-partner-api-openapi.yml
  type: apiKey
- api: PayJoy E-commerce API
  description: PayJoy-issued API key passed in an Authorization bearer header. A separate symmetric Base64 "E-commerce Key" is used to encrypt customer data sent to PayJoy (not an auth credential).
  name: EcommerceBearerAuth
  scheme: bearer
  source_docs: https://developers.payjoy.com/ecommerce/basics/authentication
  sources:
  - docs
  type: http
slug: payjoy-authentication
source_filename: payjoy-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: openapi/payjoy-partner-api-openapi.yml\ndocs: https://developers.payjoy.com/sales-integration/basics/authentication\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\n  model: >-\n    PayJoy uses API keys for machine-to-machine authentication. Each partner generates a unique\n    key in the Partner Console (Admin Console) under the API menu. The Partner API V2 sends the\n    key in the `X-PayJoy-ApiKey` header. The separate E-commerce API uses a bearer token plus a\n    symmetric Base64 \"E-commerce Key\" used to encrypt customer PII. There is no OAuth surface.\nschemes:\n- name: PayJoyApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-PayJoy-ApiKey\n  api: PayJoy Partner API V2 (Sales Integration)\n  description: API key required to authenticate all requests. Include this key in the request\n    header as `X-PayJoy-ApiKey`.\n  provisioning: Partner Console (https://app.payjoy.com/admin-console/login)\
  \ -> API -> New\n  sources:\n  - openapi/payjoy-partner-api-openapi.yml\n- name: EcommerceBearerAuth\n  type: http\n  scheme: bearer\n  api: PayJoy E-commerce API\n  description: >-\n    PayJoy-issued API key passed in an Authorization bearer header. A separate symmetric Base64\n    \"E-commerce Key\" is used to encrypt customer data sent to PayJoy (not an auth credential).\n  source_docs: https://developers.payjoy.com/ecommerce/basics/authentication\n  sources:\n  - docs\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/payjoy/refs/heads/main/authentication/payjoy-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Company
- Fintech
- Payments
- Lending
- Buy Now Pay Later
- Point of Sale
- Emerging Markets
- Financial Inclusion
- Partner API
---
