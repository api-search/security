---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: latamref-dev-alerts-api-openapi.yml
  format: yaml
  label: Latamref Alerts API
  slug: latamref-dev-alerts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/latamref-dev/openapi/latamref-dev-alerts-api-openapi.yml
- filename: latamref-dev-answers-api-openapi.yml
  format: yaml
  label: Latamref Answers API
  slug: latamref-dev-answers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/latamref-dev/openapi/latamref-dev-answers-api-openapi.yml
- filename: latamref-dev-certified-api-openapi.yml
  format: yaml
  label: Latamref Certified API
  slug: latamref-dev-certified-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/latamref-dev/openapi/latamref-dev-certified-api-openapi.yml
- filename: latamref-dev-discovery-api-openapi.yml
  format: yaml
  label: Latamref Discovery API
  slug: latamref-dev-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/latamref-dev/openapi/latamref-dev-discovery-api-openapi.yml
- filename: latamref-dev-free-api-openapi.yml
  format: yaml
  label: Latamref Free API
  slug: latamref-dev-free-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/latamref-dev/openapi/latamref-dev-free-api-openapi.yml
- filename: latamref-dev-jobs-api-openapi.yml
  format: yaml
  label: Latamref Jobs API
  slug: latamref-dev-jobs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/latamref-dev/openapi/latamref-dev-jobs-api-openapi.yml
- filename: latamref-dev-keys-api-openapi.yml
  format: yaml
  label: Latamref Keys API
  slug: latamref-dev-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/latamref-dev/openapi/latamref-dev-keys-api-openapi.yml
- filename: latamref-dev-reference-data-api-openapi.yml
  format: yaml
  label: Latamref Reference data API
  slug: latamref-dev-reference-data-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/latamref-dev/openapi/latamref-dev-reference-data-api-openapi.yml
- filename: latamref-dev-x402-sellers-api-openapi.yml
  format: yaml
  label: Latamref x402 sellers API
  slug: latamref-dev-x402-sellers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/latamref-dev/openapi/latamref-dev-x402-sellers-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: derived
name: Latamref Authentication
name_suffix: Authentication
oauth_flows: []
overview: Latamref secures its APIs with apiKey across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Latamref
provider_slug: latamref-dev
scheme_count: 3
schemes:
- description: x402 (USDC on Base). Call without this header, receive HTTP 402 carrying the price and payment details, then retry with the signed payment payload in X-PAYMENT. No signup, no account, no key. Per-operation prices are in the x-payment-info extension and at https://latamref.dev/pricing.
  in: header
  name: x402Payment
  parameter: X-PAYMENT
  sources:
  - openapi/latamref-dev-openapi.json
  type: apiKey
- description: 'Prepaid credit bought by card (from $10) at https://latamref.dev/pricing, or a free key by email at https://latamref.dev/free-key (50 calls a day on answer endpoints, commercial use allowed). Send the key on every call. How the two payment rails charge: both rails charge the same US-dollar price per call. By card, prepaid credit is worth $0.001 per credit on the $10, $25 and $100 packs and each su'
  in: header
  name: apiKey
  parameter: X-API-Key
  sources:
  - openapi/latamref-dev-openapi.json
  type: apiKey
- description: 'x402 v2 (USDC on Base, network eip155:8453): call without payment, receive HTTP 402 with the v2 PAYMENT-REQUIRED challenge, retry with the signed payload in PAYMENT-SIGNATURE. The challenge is v2 only, so a client must read v2; X-PAYMENT is also accepted as the payment header. No signup, no key.'
  in: header
  name: x402
  parameter: PAYMENT-SIGNATURE
  sources:
  - openapi/latamref-dev-openapi.json
  type: apiKey
slug: latamref-dev-authentication
source_filename: latamref-dev-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-15'\nmethod: derived\nsource: openapi/latamref-dev-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: x402Payment\n  type: apiKey\n  in: header\n  parameter: X-PAYMENT\n  description: x402 (USDC on Base). Call without this header, receive HTTP 402 carrying the\n    price and payment details, then retry with the signed payment payload in X-PAYMENT. No signup,\n    no account, no key. Per-operation prices are in the x-payment-info extension and at https://latamref.dev/pricing.\n  sources:\n  - openapi/latamref-dev-openapi.json\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: 'Prepaid credit bought by card (from $10) at https://latamref.dev/pricing, or\n    a free key by email at https://latamref.dev/free-key (50 calls a day on answer endpoints,\n    commercial use allowed). Send the key on every call. How the two payment rails charge: both\n    rails charge the same US-dollar price\
  \ per call. By card, prepaid credit is worth $0.001\n    per credit on the $10, $25 and $100 packs and each su'\n  sources:\n  - openapi/latamref-dev-openapi.json\n- name: x402\n  type: apiKey\n  in: header\n  parameter: PAYMENT-SIGNATURE\n  description: 'x402 v2 (USDC on Base, network eip155:8453): call without payment, receive HTTP\n    402 with the v2 PAYMENT-REQUIRED challenge, retry with the signed payload in PAYMENT-SIGNATURE.\n    The challenge is v2 only, so a client must read v2; X-PAYMENT is also accepted as the payment\n    header. No signup, no key.'\n  sources:\n  - openapi/latamref-dev-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/latamref-dev/authentication/latamref-dev-authentication.yml
summary_line: apiKey · 3 schemes
tags:
- Data
- Government
- Latin America
- Reference
---
