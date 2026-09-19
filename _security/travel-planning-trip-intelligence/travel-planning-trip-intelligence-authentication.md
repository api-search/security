---
anonymous_access: false
api_key_in: []
api_specs:
- filename: travel-planning-trip-intelligence-openapi-original.json
  format: json
  label: ForgeMesh Travel Agent API
  slug: forgemesh-travel-agent-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/travel-planning-trip-intelligence/refs/heads/main/openapi/travel-planning-trip-intelligence-openapi-original.json
auth_types:
- x402-payment
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Travel Planning Trip Intelligence Authentication
name_suffix: Authentication
oauth_flows: []
overview: ForgeMesh Travel Agent secures its APIs with x402-payment across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: ForgeMesh Travel Agent
provider_slug: travel-planning-trip-intelligence
scheme_count: 1
schemes:
- asset: '0x833589fCD6eDb6E08f4c7C32D4f71b54bdA02913'
  description: HTTP 402 payment challenge. The paid route answers 402 with x402 payment terms; the client pays in USDC on Base (eip155:8453) and retries the same request carrying the PAYMENT-SIGNATURE header (x402 v2) or X-PAYMENT (v1). No accounts or API keys.
  headers:
  - PAYMENT-SIGNATURE
  - X-PAYMENT
  name: x402
  network: eip155:8453
  pay_to: '0x7F7C9bfF1DDF2817641740962A9872e6421eBBFc'
  protocols:
  - x402
  - mpp
  scheme: http-402-payment
  source: agent-card.json securitySchemes + /.well-known/x402.json + llms.txt
  type: x402
slug: travel-planning-trip-intelligence-authentication
source_filename: travel-planning-trip-intelligence-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-17'\nmethod: searched\nsource: https://travel-agent.forgemesh.io/.well-known/agent-card.json\ndocs: https://travel-agent.forgemesh.io/llms.txt\nsummary:\n  types: [x402-payment]\n  api_key_in: []\n  oauth2_flows: []\n  accounts_required: false\n  api_keys_required: false\nnote: >-\n  There is no token/credential auth. The OpenAPI declares no securitySchemes;\n  free routes carry security: [] and paid routes gate on the x402 HTTP-402\n  payment challenge. Access is authorized by an on-chain USDC payment on Base,\n  not by an identity credential.\nschemes:\n- name: x402\n  type: x402\n  scheme: http-402-payment\n  description: >-\n    HTTP 402 payment challenge. The paid route answers 402 with x402 payment\n    terms; the client pays in USDC on Base (eip155:8453) and retries the same\n    request carrying the PAYMENT-SIGNATURE header (x402 v2) or X-PAYMENT (v1).\n    No accounts or API keys.\n  network: eip155:8453\n  asset: '0x833589fCD6eDb6E08f4c7C32D4f71b54bdA02913'\
  \   # USDC on Base\n  pay_to: '0x7F7C9bfF1DDF2817641740962A9872e6421eBBFc'\n  headers: [PAYMENT-SIGNATURE, X-PAYMENT]\n  protocols: [x402, mpp]\n  source: agent-card.json securitySchemes + /.well-known/x402.json + llms.txt\nfree_routes:\n- GET /api/categories\n- GET /api/currency-exchange\n- GET /api/request-coverage\n- GET /health\n- GET /\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/travel-planning-trip-intelligence/refs/heads/main/authentication/travel-planning-trip-intelligence-authentication.yml
summary_line: x402-payment · 1 scheme
tags:
- travel
- trip-planning
- itinerary
- weather
- mobility/transit
- disruption-intelligence
- x402
- pay-per-call / micropayments
- USDC
- Base / onchain payments
- MCP
- agent-native
- OpenAPI
- llms.txt
---
