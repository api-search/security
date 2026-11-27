---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: AI Rook Authentication
name_suffix: Authentication
oauth_flows: []
overview: AI Rook declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: AI Rook
provider_slug: ai-rook-com
scheme_count: 2
schemes:
- description: Per-call USDC payment required via 402 challenge and X-Payment header. No API keys.
  headers:
  - X-Payment
  - X-Payment-Response
  name: x402-payment
  type: custom
- description: Prepaid credit wallet identifier for bulk usage.
  in: header
  name: X-Credit-Wallet
  notes: Use after purchasing credits via POST /api/credits/purchase (not callable here).
  type: apiKey
slug: ai-rook-com-authentication
source_filename: ai-rook-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: searched\nsource: https://agents.ai-rook.com/llms.txt\nschemes:\n  - type: custom\n    name: x402-payment\n    description: Per-call USDC payment required via 402 challenge and X-Payment header. No API keys.\n    headers:\n      - X-Payment\n      - X-Payment-Response\n  - type: apiKey\n    name: X-Credit-Wallet\n    in: header\n    description: Prepaid credit wallet identifier for bulk usage.\n    notes: Use after purchasing credits via POST /api/credits/purchase (not callable here).\n"
source_yaml_url: https://artifacts.apis.io/ai-rook-com/authentication/ai-rook-com-authentication.yml
summary_line: 2 schemes
tags:
- Artificial Intelligence
- Autonomous
- Cryptocurrency
- LLM
- Payments
- Trading
---
