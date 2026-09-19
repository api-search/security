---
anonymous_access: false
api_key_in: []
api_specs:
- filename: layoff-workforce-disruption-tracker-openapi.json
  format: json
  label: Disruption Intelligence API
  slug: disruption-intelligence-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/layoff-workforce-disruption-tracker/refs/heads/main/openapi/layoff-workforce-disruption-tracker-openapi.json
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Layoff Workforce Disruption Tracker Authentication
name_suffix: Authentication
oauth_flows: []
overview: Layoff & Workforce Disruption Tracker declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Layoff & Workforce Disruption Tracker
provider_slug: layoff-workforce-disruption-tracker
scheme_count: 1
schemes:
- asset: '0x833589fCD6eDb6E08f4c7C32D4f71b54bdA02913'
  challenge_status: 402
  description: HTTP 402 payment challenge; pay USDC on Base and retry with the payment header. Discovery and coarse-inventory endpoints are unauthenticated and free.
  facilitator: https://x402.org/facilitator/
  headers:
  - PAYMENT-SIGNATURE
  - X-PAYMENT
  in: header
  name: x402 payment challenge
  network: eip155:8453
  payTo: '0xA8774fACfD3Da2EA11f240C977b9973D78aDFCFe'
  receipt_header: PAYMENT-RESPONSE
  type: x402
slug: layoff-workforce-disruption-tracker-authentication
source_filename: layoff-workforce-disruption-tracker-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-17'\nmethod: searched\nsource: https://disruption.forgemesh.io/llms.txt\nalso:\n- https://disruption.forgemesh.io/agents.txt\n- https://disruption.forgemesh.io/.well-known/agent-card.json (securitySchemes.x402)\nsummary: >-\n  No API keys, no OAuth, no accounts. Authorization IS payment: every paid route answers HTTP 402\n  with x402 payment terms, and the caller settles in USDC on Base mainnet (eip155:8453) and retries\n  with a payment header. The OpenAPI declares no components.securitySchemes because the scheme is\n  carried in the x-x402 root extension and per-operation x-payment-info instead.\nschemes:\n- type: x402\n  name: x402 payment challenge\n  in: header\n  headers:\n  - PAYMENT-SIGNATURE   # x402 v2 (on the paid retry)\n  - X-PAYMENT           # x402 v1 (legacy)\n  challenge_status: 402\n  receipt_header: PAYMENT-RESPONSE   # settlement receipt returned after a paid call\n  network: eip155:8453\n  asset: '0x833589fCD6eDb6E08f4c7C32D4f71b54bdA02913'\
  \   # USDC on Base\n  payTo: '0xA8774fACfD3Da2EA11f240C977b9973D78aDFCFe'\n  facilitator: https://x402.org/facilitator/\n  description: >-\n    HTTP 402 payment challenge; pay USDC on Base and retry with the payment header. Discovery and\n    coarse-inventory endpoints are unauthenticated and free.\nnotes: >-\n  The x-x402 extension advertises live optional extensions: Bazaar marketplace discovery, an optional\n  retry-safe payment-identifier (idempotency), and signed offer/receipt (300s offer validity). No\n  sign-in-with-x is used (\"not needed for one-shot disruption outputs\").\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/layoff-workforce-disruption-tracker/refs/heads/main/authentication/layoff-workforce-disruption-tracker-authentication.yml
summary_line: 1 scheme
tags:
- Workforce intelligence
- Layoffs
- WARN filings
- Labor-market data
- Economic intelligence
- Geospatial intelligence
- Risk scoring
- Company intelligence
- Supply-chain analysis
- Ripple-effect analysis
- Agent-native
- MCP
- x402
- Pay-per-call
---
