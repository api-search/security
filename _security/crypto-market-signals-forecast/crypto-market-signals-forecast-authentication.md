---
anonymous_access: false
api_key_in: []
api_specs:
- filename: crypto-market-signals-forecast-openapi-original.json
  format: json
  label: Crypto Market Signals & Forecast
  slug: crypto-market-signals-forecast
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crypto-market-signals-forecast/refs/heads/main/openapi/crypto-market-signals-forecast-openapi-original.json
auth_types:
- x402
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Crypto Market Signals Forecast Authentication
name_suffix: Authentication
oauth_flows: []
overview: Crypto Market Signals & Forecast secures its APIs with x402 across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Crypto Market Signals & Forecast
provider_slug: crypto-market-signals-forecast
scheme_count: 1
schemes:
- asset: USDC (0x833589fCD6eDb6E08f4c7C32D4f71b54bdA02913)
  description: HTTP 402 payment challenge; pay in USDC on Base (eip155:8453) and retry with the PAYMENT-SIGNATURE header. No accounts or API keys.
  facilitator: https://x402.xyz/facilitate
  name: x402
  network: eip155:8453
  pay_to: '0x1304EC1A8945365e43A5c18a734065f107B417cA'
  request_header: PAYMENT-SIGNATURE
  scheme: http-402-payment
  sources:
  - openapi/crypto-market-signals-forecast-openapi-original.json
  type: x402
slug: crypto-market-signals-forecast-authentication
source_filename: crypto-market-signals-forecast-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-17'\nmethod: searched\nsource:\n  - https://x402.coinopai.com/openapi.json\n  - https://x402.coinopai.com/.well-known/agent-card.json\n  - https://x402.coinopai.com/llms.txt\nnote: >-\n  The OpenAPI declares NO securitySchemes — access is not gated by an API key, OAuth\n  token, or session. Instead every paid route answers HTTP 402 with an x402 payment\n  challenge; the client settles a USDC micropayment on Base and retries with the\n  PAYMENT-SIGNATURE header. The provider's agent card formalizes this as a security\n  scheme of type \"x402\". This is a payment-as-access model, not a traditional\n  authentication model.\nsummary:\n  types: [x402]\n  api_key_in: []\n  oauth2_flows: []\n  accounts_required: false\nschemes:\n  - name: x402\n    type: x402\n    scheme: http-402-payment\n    description: >-\n      HTTP 402 payment challenge; pay in USDC on Base (eip155:8453) and retry with the\n      PAYMENT-SIGNATURE header. No accounts or API keys.\n    network:\
  \ eip155:8453\n    asset: USDC (0x833589fCD6eDb6E08f4c7C32D4f71b54bdA02913)\n    pay_to: '0x1304EC1A8945365e43A5c18a734065f107B417cA'\n    facilitator: https://x402.xyz/facilitate\n    request_header: PAYMENT-SIGNATURE\n    sources: [openapi/crypto-market-signals-forecast-openapi-original.json]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/crypto-market-signals-forecast/refs/heads/main/authentication/crypto-market-signals-forecast-authentication.yml
summary_line: x402 · 1 scheme
tags:
- Cryptocurrency
- Financial markets
- Market data
- Trading signals
- Market intelligence
- AI agents
- Agentic tooling
- x402
- On-chain micropayments
- Fintech
- Workflow automation
---
