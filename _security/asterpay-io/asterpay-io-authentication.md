---
anonymous_access: false
api_key_in: []
api_specs:
- filename: asterpay-io-ai-api-openapi.yml
  format: yaml
  label: AsterPay AI API
  slug: asterpay-io-ai-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/asterpay-io/openapi/asterpay-io-ai-api-openapi.yml
- filename: asterpay-io-crypto-api-openapi.yml
  format: yaml
  label: AsterPay Crypto API
  slug: asterpay-io-crypto-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/asterpay-io/openapi/asterpay-io-crypto-api-openapi.yml
- filename: asterpay-io-data-api-openapi.yml
  format: yaml
  label: AsterPay Data API
  slug: asterpay-io-data-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/asterpay-io/openapi/asterpay-io-data-api-openapi.yml
- filename: asterpay-io-discovery-api-openapi.yml
  format: yaml
  label: AsterPay Discovery API
  slug: asterpay-io-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/asterpay-io/openapi/asterpay-io-discovery-api-openapi.yml
- filename: asterpay-io-market-api-openapi.yml
  format: yaml
  label: AsterPay Market API
  slug: asterpay-io-market-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/asterpay-io/openapi/asterpay-io-market-api-openapi.yml
- filename: asterpay-io-sessions-api-openapi.yml
  format: yaml
  label: AsterPay Sessions API
  slug: asterpay-io-sessions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/asterpay-io/openapi/asterpay-io-sessions-api-openapi.yml
- filename: asterpay-io-settlement-api-openapi.yml
  format: yaml
  label: AsterPay Settlement API
  slug: asterpay-io-settlement-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/asterpay-io/openapi/asterpay-io-settlement-api-openapi.yml
- filename: asterpay-io-trust-api-openapi.yml
  format: yaml
  label: AsterPay Trust API
  slug: asterpay-io-trust-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/asterpay-io/openapi/asterpay-io-trust-api-openapi.yml
- filename: asterpay-io-utility-api-openapi.yml
  format: yaml
  label: AsterPay Utility API
  slug: asterpay-io-utility-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/asterpay-io/openapi/asterpay-io-utility-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Asterpay Io Authentication
name_suffix: Authentication
oauth_flows: []
overview: AsterPay declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: AsterPay
provider_slug: asterpay-io
scheme_count: 2
schemes:
- description: x402 payment signature header; per-request wallet signature.
  in: header
  name: PAYMENT-SIGNATURE
  official: true
  type: apiKey
- description: MPP (Machine Payments Protocol) Authorization header.
  official: true
  scheme: Payment
  type: http
slug: asterpay-io-authentication
source_filename: asterpay-io-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: searched\nsource: https://asterpay.io/docs.md\nschemes:\n  - type: apiKey\n    name: PAYMENT-SIGNATURE\n    in: header\n    description: x402 payment signature header; per-request wallet signature.\n    official: true\n  - type: http\n    scheme: Payment\n    description: MPP (Machine Payments Protocol) Authorization header.\n    official: true\n"
source_yaml_url: https://artifacts.apis.io/asterpay-io/authentication/asterpay-io-authentication.yml
summary_line: 2 schemes
tags:
- Payments
- Fintech
- Artificial Intelligence
- EUR
- Settlement
---
