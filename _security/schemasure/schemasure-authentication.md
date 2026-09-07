---
anonymous_access: false
api_key_in: []
api_specs:
- filename: schemasure-openapi.json
  format: json
  label: SchemaSure Structured Extraction API
  slug: schemasure-structured-extraction-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/schemasure/refs/heads/main/openapi/schemasure-openapi.json
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Schemasure Authentication
name_suffix: Authentication
oauth_flows: []
overview: SchemaSure declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: SchemaSure
provider_slug: schemasure
scheme_count: 2
schemes:
- applies_to:
  - /v2/extract
  - /v2/extract-image
  asset: USDC (0x833589fCD6eDb6E08f4c7C32D4f71b54bdA02913)
  challenge_header: PAYMENT-REQUIRED
  in: header
  name: x402-payment
  network: eip155:8453 (Base mainnet)
  note: Charge-only-on-success; failed calls are not settled. Do not hardcode payment terms — validate the live challenge.
  receipt_header: PAYMENT-RESPONSE
  request_header: PAYMENT-SIGNATURE
  type: x402
  version: 2
- applies_to:
  - /extract
  in: header
  name: x402-payment-v1
  note: Legacy flow after the 3 free evaluation calls per client.
  receipt_header: X-PAYMENT-RESPONSE
  request_header: X-PAYMENT
  type: x402
  version: 1
slug: schemasure-authentication
source_filename: schemasure-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-03'\nmethod: searched\nsource: https://schemasure.com/llms.txt + well-known/schemasure-x402.json\nnote: >-\n  derive-authentication.py produced no profile because the OpenAPI declares no securitySchemes —\n  correctly: SchemaSure has no authentication in the credential sense. There are no accounts, API\n  keys, or OAuth. Access control is x402 pay-per-call payment: an unsigned request returns 402\n  with a PAYMENT-REQUIRED challenge; the caller signs the terms with an x402 V2-compatible wallet\n  (USDC on Base mainnet, eip155:8453) and retries with PAYMENT-SIGNATURE. Identity is the payer\n  wallet address. OAuth discovery documents 404 (recorded in well-known/schemasure-well-known.yml).\nschemes:\n- name: x402-payment\n  type: x402\n  version: 2\n  in: header\n  request_header: PAYMENT-SIGNATURE\n  challenge_header: PAYMENT-REQUIRED\n  receipt_header: PAYMENT-RESPONSE\n  network: eip155:8453 (Base mainnet)\n  asset: USDC (0x833589fCD6eDb6E08f4c7C32D4f71b54bdA02913)\n\
  \  applies_to: [/v2/extract, /v2/extract-image]\n  note: Charge-only-on-success; failed calls are not settled. Do not hardcode payment terms — validate the live challenge.\n- name: x402-payment-v1\n  type: x402\n  version: 1\n  in: header\n  request_header: X-PAYMENT\n  receipt_header: X-PAYMENT-RESPONSE\n  applies_to: [/extract]\n  note: Legacy flow after the 3 free evaluation calls per client.\napi_keys: none\noauth: none\naccounts: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/schemasure/refs/heads/main/authentication/schemasure-authentication.yml
summary_line: 2 schemes
tags:
- Structured Data Extraction
- text-to-JSON
- JSON-Schema
- Document Parsing
- Data Cleaning
- LLM Tooling
- AI Agents
- x402-micropayments
- agent-native
- A2A
- MCP
---
