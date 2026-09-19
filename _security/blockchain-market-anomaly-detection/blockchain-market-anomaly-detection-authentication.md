---
anonymous_access: false
api_key_in: []
api_specs:
- filename: blockchain-market-anomaly-detection-openapi.json
  format: json
  label: Blockchain & Market Anomaly Detection API
  slug: blockchain-market-anomaly-detection-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blockchain-market-anomaly-detection/refs/heads/main/openapi/blockchain-market-anomaly-detection-openapi.json
auth_types:
- x402
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Blockchain Market Anomaly Detection Authentication
name_suffix: Authentication
oauth_flows: []
overview: Blockchain & Market Anomaly Detection secures its APIs with x402 across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Blockchain & Market Anomaly Detection
provider_slug: blockchain-market-anomaly-detection
scheme_count: 1
schemes:
- description: HTTP 402 payment challenge. Pay per call in USDC on Base (eip155:8453) and retry with the payment signature header. No accounts or API keys.
  name: x402
  scheme: http-402-payment-challenge
  sources:
  - a2a/blockchain-market-anomaly-detection-agent-card.json
  - openapi/blockchain-market-anomaly-detection-openapi.json
  type: x402
slug: blockchain-market-anomaly-detection-authentication
source_filename: blockchain-market-anomaly-detection-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-17'\nmethod: searched\nsource: https://anomaly.forgemesh.io/llms.txt\ndocs: https://anomaly.forgemesh.io/llms.txt\nsummary:\n  types: [x402]\n  api_key_in: []\n  oauth2_flows: []\n  note: >-\n    No API keys, no accounts, no OAuth. Access is gated by the x402 payment protocol: an unpaid\n    request to any /api/* route returns HTTP 402 with x402 payment terms; the agent signs a USDC\n    authorization on Base mainnet (eip155:8453) and retries with the payment header. The OpenAPI\n    declares no securitySchemes; the agent card declares a single x402 scheme.\nschemes:\n- name: x402\n  type: x402\n  scheme: http-402-payment-challenge\n  description: >-\n    HTTP 402 payment challenge. Pay per call in USDC on Base (eip155:8453) and retry with the\n    payment signature header. No accounts or API keys.\n  sources:\n  - a2a/blockchain-market-anomaly-detection-agent-card.json\n  - openapi/blockchain-market-anomaly-detection-openapi.json\npayment:\n  protocol:\
  \ x402\n  also_supported: mpp\n  network: eip155:8453\n  network_name: Base mainnet\n  currency: USDC\n  currency_contract: '0x833589fCD6eDb6E08f4c7C32D4f71b54bdA02913'\n  pay_to: '0xE295B6641b32998537Ae0f8E61Babf729EAEd6E5'\n  facilitator: https://x402.xyz/facilitate\n  x402_extensions:\n    bazaar: live\n    payment_identifier: live (retry-safe idempotency keys)\n    builder_code: bc_4ypyymtf\n    offer_receipt: live\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/blockchain-market-anomaly-detection/refs/heads/main/authentication/blockchain-market-anomaly-detection-authentication.yml
summary_line: x402 · 1 scheme
tags:
- blockchain
- crypto
- web3
- anomaly-detection
- mempool
- stablecoin-monitoring
- defi
- nft-analytics
- market-surveillance
- aviation-tracking
- github-signals
- x402
- agent-commerce
- mcp
---
