---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: mearef-dev-alerts-api-openapi.yml
  format: yaml
  label: Mearef Alerts API
  slug: mearef-dev-alerts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mearef-dev/openapi/mearef-dev-alerts-api-openapi.yml
- filename: mearef-dev-answers-api-openapi.yml
  format: yaml
  label: Mearef Answers API
  slug: mearef-dev-answers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mearef-dev/openapi/mearef-dev-answers-api-openapi.yml
- filename: mearef-dev-certified-api-openapi.yml
  format: yaml
  label: Mearef Certified API
  slug: mearef-dev-certified-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mearef-dev/openapi/mearef-dev-certified-api-openapi.yml
- filename: mearef-dev-discovery-api-openapi.yml
  format: yaml
  label: Mearef Discovery API
  slug: mearef-dev-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mearef-dev/openapi/mearef-dev-discovery-api-openapi.yml
- filename: mearef-dev-free-api-openapi.yml
  format: yaml
  label: Mearef Free API
  slug: mearef-dev-free-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mearef-dev/openapi/mearef-dev-free-api-openapi.yml
- filename: mearef-dev-jobs-api-openapi.yml
  format: yaml
  label: Mearef Jobs API
  slug: mearef-dev-jobs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mearef-dev/openapi/mearef-dev-jobs-api-openapi.yml
- filename: mearef-dev-keys-api-openapi.yml
  format: yaml
  label: Mearef Keys API
  slug: mearef-dev-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mearef-dev/openapi/mearef-dev-keys-api-openapi.yml
- filename: mearef-dev-reference-data-api-openapi.yml
  format: yaml
  label: Mearef Reference data API
  slug: mearef-dev-reference-data-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mearef-dev/openapi/mearef-dev-reference-data-api-openapi.yml
- filename: mearef-dev-x402-sellers-api-openapi.yml
  format: yaml
  label: Mearef x402 sellers API
  slug: mearef-dev-x402-sellers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mearef-dev/openapi/mearef-dev-x402-sellers-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: derived
name: Mearef Authentication
name_suffix: Authentication
oauth_flows: []
overview: Mearef secures its APIs with apiKey across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Mearef
provider_slug: mearef-dev
scheme_count: 3
schemes:
- description: x402 (USDC on Base). Call without this header, receive HTTP 402 carrying the price and payment details, then retry with the signed payment payload in X-PAYMENT. No signup, no account, no key. Per-operation prices are in the x-payment-info extension and at https://mearef.dev/pricing.
  in: header
  name: x402Payment
  parameter: X-PAYMENT
  sources:
  - openapi/mearef-dev-openapi.json
  type: apiKey
- description: 'Prepaid credit bought by card (from $10) at https://mearef.dev/pricing, or a free key by email at https://mearef.dev/free-key (50 calls a day on answer endpoints, commercial use allowed). Send the key on every call. How the two payment rails charge: both rails charge the same US-dollar price per call. By card, prepaid credit is worth $0.001 per credit on the $10, $25 and $100 packs and each succes'
  in: header
  name: apiKey
  parameter: X-API-Key
  sources:
  - openapi/mearef-dev-openapi.json
  type: apiKey
- description: 'x402 v2 (USDC on Base, network eip155:8453): call without payment, receive HTTP 402 with the v2 PAYMENT-REQUIRED challenge, retry with the signed payload in PAYMENT-SIGNATURE. The challenge is v2 only, so a client must read v2; X-PAYMENT is also accepted as the payment header. No signup, no key.'
  in: header
  name: x402
  parameter: PAYMENT-SIGNATURE
  sources:
  - openapi/mearef-dev-openapi.json
  type: apiKey
slug: mearef-dev-authentication
source_filename: mearef-dev-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: derived\nsource: openapi/mearef-dev-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: x402Payment\n  type: apiKey\n  in: header\n  parameter: X-PAYMENT\n  description: x402 (USDC on Base). Call without this header, receive HTTP 402 carrying the\n    price and payment details, then retry with the signed payment payload in X-PAYMENT. No signup,\n    no account, no key. Per-operation prices are in the x-payment-info extension and at https://mearef.dev/pricing.\n  sources:\n  - openapi/mearef-dev-openapi.json\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: 'Prepaid credit bought by card (from $10) at https://mearef.dev/pricing, or a\n    free key by email at https://mearef.dev/free-key (50 calls a day on answer endpoints, commercial\n    use allowed). Send the key on every call. How the two payment rails charge: both rails charge\n    the same US-dollar price per call.\
  \ By card, prepaid credit is worth $0.001 per credit on\n    the $10, $25 and $100 packs and each succes'\n  sources:\n  - openapi/mearef-dev-openapi.json\n- name: x402\n  type: apiKey\n  in: header\n  parameter: PAYMENT-SIGNATURE\n  description: 'x402 v2 (USDC on Base, network eip155:8453): call without payment, receive HTTP\n    402 with the v2 PAYMENT-REQUIRED challenge, retry with the signed payload in PAYMENT-SIGNATURE.\n    The challenge is v2 only, so a client must read v2; X-PAYMENT is also accepted as the payment\n    header. No signup, no key.'\n  sources:\n  - openapi/mearef-dev-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/mearef-dev/authentication/mearef-dev-authentication.yml
summary_line: apiKey · 3 schemes
tags:
- Company
- Data
- Government
- Middle East
---
