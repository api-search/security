---
api_key_in:
- header
api_specs:
- filename: tsys-payment-gateway-openapi.yml
  format: yaml
  label: TSYS Payment Gateway
  slug: tsys-payment-gateway
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/total-system-services/refs/heads/main/openapi/tsys-payment-gateway-openapi.yml
- filename: tsys-issuing-openapi.yml
  format: yaml
  label: TSYS Issuing Platform
  slug: tsys-issuing
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/total-system-services/refs/heads/main/openapi/tsys-issuing-openapi.yml
- filename: tsys-merchant-openapi.yml
  format: yaml
  label: TSYS Merchant Services
  slug: tsys-merchant
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/total-system-services/refs/heads/main/openapi/tsys-merchant-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Total System Services Authentication
name_suffix: Authentication
oauth_flows: []
overview: Total System Services secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Total System Services
provider_slug: total-system-services
scheme_count: 2
schemes:
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/tsys-issuing-openapi.yml
  type: http
- in: header
  name: apiKeyAuth
  parameter: X-TSYS-API-Key
  sources:
  - openapi/tsys-payment-gateway-openapi.yml
  type: apiKey
slug: total-system-services-authentication
source_filename: total-system-services-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/tsys-issuing-openapi.yml, openapi/tsys-payment-gateway-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/tsys-issuing-openapi.yml\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-TSYS-API-Key\n  sources:\n  - openapi/tsys-payment-gateway-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/total-system-services/refs/heads/main/authentication/total-system-services-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Payments
- Payment Processing
- Card Issuing
- Merchant Services
- Fintech
- Financial Services
- Fortune 1000
---
