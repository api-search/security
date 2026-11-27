---
anonymous_access: true
api_key_in: []
api_specs:
- filename: checkpoint402-com-blockchain-api-openapi.yml
  format: yaml
  label: Checkpoint402 Blockchain API
  slug: checkpoint402-com-blockchain-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/checkpoint402-com/openapi/checkpoint402-com-blockchain-api-openapi.yml
- filename: checkpoint402-com-defi-api-openapi.yml
  format: yaml
  label: Checkpoint402 Defi API
  slug: checkpoint402-com-defi-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/checkpoint402-com/openapi/checkpoint402-com-defi-api-openapi.yml
- filename: checkpoint402-com-sanctions-api-openapi.yml
  format: yaml
  label: Checkpoint402 Sanctions API
  slug: checkpoint402-com-sanctions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/checkpoint402-com/openapi/checkpoint402-com-sanctions-api-openapi.yml
- filename: checkpoint402-com-sec-api-openapi.yml
  format: yaml
  label: Checkpoint402 Sec API
  slug: checkpoint402-com-sec-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/checkpoint402-com/openapi/checkpoint402-com-sec-api-openapi.yml
- filename: checkpoint402-com-tokens-api-openapi.yml
  format: yaml
  label: Checkpoint402 Tokens API
  slug: checkpoint402-com-tokens-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/checkpoint402-com/openapi/checkpoint402-com-tokens-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Checkpoint402 Authentication
name_suffix: Authentication
oauth_flows: []
overview: Checkpoint402 declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Checkpoint402
provider_slug: checkpoint402-com
scheme_count: 2
schemes:
- challenge_header: PAYMENT-REQUIRED
  description: Call without payment, receive 402 with PAYMENT-REQUIRED (price, network, receiving wallet); sign a USDC transfer authorization on Base (signature only, no gas) and repeat the call with PAYMENT-SIGNATURE. Settled on-chain only if the request succeeds; the transaction is returned in PAYMENT-RESPONSE.
  in: header
  name: x402 payment
  receipt_header: PAYMENT-RESPONSE
  request_header: PAYMENT-SIGNATURE
  type: x402
- description: Free endpoints /, /health and /openapi.json need no payment or credentials.
  name: none
  type: none
slug: checkpoint402-com-authentication
source_filename: checkpoint402-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: searched\nsource: https://checkpoint402.com/docs\ndocs: https://checkpoint402.com/docs\nnote: 'The docs state \"There are no accounts or API keys\". The OpenAPI declares no securitySchemes. Access to paid endpoints is gated by per-request x402 payment rather than identity.'\nschemes:\n- name: x402 payment\n  type: x402\n  in: header\n  request_header: PAYMENT-SIGNATURE\n  challenge_header: PAYMENT-REQUIRED\n  receipt_header: PAYMENT-RESPONSE\n  description: Call without payment, receive 402 with PAYMENT-REQUIRED (price, network, receiving wallet); sign a USDC transfer authorization on Base (signature only, no gas) and repeat the call with PAYMENT-SIGNATURE. Settled on-chain only if the request succeeds; the transaction is returned in PAYMENT-RESPONSE.\n- name: none\n  type: none\n  description: Free endpoints /, /health and /openapi.json need no payment or credentials.\n"
source_yaml_url: https://artifacts.apis.io/checkpoint402-com/authentication/checkpoint402-com-authentication.yml
summary_line: 2 schemes
tags:
- Company
- AI Agents
- x402
- Payments
- Cryptocurrency
- DeFi
- Blockchain
- Sanctions Screening
- SEC Filings
- MCP
---
