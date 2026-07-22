---
api_key_in:
- header
api_specs:
- filename: merit-systems-merit-api-openapi.yml
  format: yaml
  label: Merit Systems API
  slug: merit-systems-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/merit-systems/refs/heads/main/openapi/merit-systems-merit-api-openapi.yml
- filename: merit-systems-agentcash-openapi.json
  format: json
  label: AgentCash API
  slug: agentcash-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/merit-systems/refs/heads/main/openapi/merit-systems-agentcash-openapi.json
auth_types:
- apiKey
- x402
- mpp
- siwx
description: ''
kind: authentication
layout: security
method: searched
name: Merit Systems Authentication
name_suffix: Authentication
oauth_flows: []
overview: Merit Systems secures its APIs with apiKey, x402, mpp, and siwx across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Merit Systems
provider_slug: merit-systems
scheme_count: 4
schemes:
- api: Merit Systems API
  in: header
  name: apiKey
  parameter: x-api-key
  source: openapi/merit-systems-merit-api-openapi.yml
  type: apiKey
- api: AgentCash
  description: Sign In With X — wallet-based identity header for free AgentCash endpoints (search, invite-codes, organizations).
  in: header
  name: siwx
  parameter: SIGN-IN-WITH-X
  source: openapi/merit-systems-agentcash-openapi.json
  type: apiKey
- api: AgentCash
  currency: USDC
  description: HTTP-native micropayment protocol. Paid endpoints (e.g. POST /api/send) return 402 Payment Required; the agent's wallet settles the payment in USDC (Base, Solana, or Tempo) inside the same request. No accounts or API keys.
  name: x402
  networks:
  - base
  - solana
  - tempo
  scheme: x402
  type: payment
- api: AgentCash
  description: Machine Payments Protocol — per-request server payment, alternative rail to x402.
  name: mpp
  scheme: mpp
  type: payment
slug: merit-systems-authentication
source_filename: merit-systems-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource:\n  - https://github.com/merit-systems/sdk/blob/master/api.md\n  - https://agentcash.dev/openapi.json\nsummary:\n  types: [apiKey, x402, mpp, siwx]\n  api_key_in: [header]\n  notes: >-\n    Two distinct auth models across Merit's surfaces. The Merit Systems REST API\n    uses a static API key header. AgentCash uses wallet-based auth: free\n    \"SIWX\" (Sign In With X-chain wallet) endpoints via a signed header, and paid\n    endpoints settled per-call over x402/MPP micropayments (HTTP 402) — no API\n    keys required for paid calls.\nschemes:\n  - name: apiKey\n    api: Merit Systems API\n    type: apiKey\n    in: header\n    parameter: x-api-key\n    source: openapi/merit-systems-merit-api-openapi.yml\n  - name: siwx\n    api: AgentCash\n    type: apiKey\n    in: header\n    parameter: SIGN-IN-WITH-X\n    description: Sign In With X — wallet-based identity header for free AgentCash endpoints (search, invite-codes, organizations).\n\
  \    source: openapi/merit-systems-agentcash-openapi.json\n  - name: x402\n    api: AgentCash\n    type: payment\n    scheme: x402\n    description: >-\n      HTTP-native micropayment protocol. Paid endpoints (e.g. POST /api/send)\n      return 402 Payment Required; the agent's wallet settles the payment in\n      USDC (Base, Solana, or Tempo) inside the same request. No accounts or API\n      keys.\n    networks: [base, solana, tempo]\n    currency: USDC\n  - name: mpp\n    api: AgentCash\n    type: payment\n    scheme: mpp\n    description: Machine Payments Protocol — per-request server payment, alternative rail to x402.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/merit-systems/refs/heads/main/authentication/merit-systems-authentication.yml
summary_line: apiKey/x402/mpp/siwx · 4 schemes
tags:
- Company
- Agentic Commerce
- Payments
- x402
- Micropayments
- Model Context Protocol
- Stablecoins
- API Discovery
- Open Source
- Developer Tools
---
