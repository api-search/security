---
api_key_in: []
api_specs:
- filename: exponential-protocol-openapi.yml
  format: yaml
  label: YO Protocol API
  slug: yo-protocol-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/exponential/refs/heads/main/openapi/exponential-protocol-openapi.yml
- filename: exponential-risk-graph-openapi.yml
  format: yaml
  label: YO Risk Graph API
  slug: yo-risk-graph-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/exponential/refs/heads/main/openapi/exponential-risk-graph-openapi.yml
auth_types:
- none
- payment-gated
description: ''
kind: authentication
layout: security
method: searched
name: Exponential Authentication
name_suffix: Authentication
oauth_flows: []
overview: Exponential secures its APIs with none and payment-gated across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Exponential
provider_slug: exponential
scheme_count: 3
schemes:
- applies_to:
  - openapi/exponential-protocol-openapi.yml
  - risk.yo.xyz /api/v1/public/vault/**
  description: No API key required.
  name: publicRead
  type: none
- applies_to:
  - risk.yo.xyz /api/v1/agent/**
  asset: USDC 0x833589fCD6eDb6E08f4c7C32D4f71b54bdA02913
  challenge_status: 402
  description: Per-call payment gate; no onboarding or credential.
  header: X-PAYMENT
  name: x402Payment
  network: eip155:8453 (Base mainnet)
  scheme: x402
  settlement: EIP-3009 transferWithAuthorization via Coinbase CDP
  type: payment
- applies_to:
  - yoGateway 0xF1EeE0957267b1A474323Ff9CfF7719E964969FA
  description: Deposits and redeems are authorized by the user's EVM wallet signature via the yoGateway.
  name: walletSignature
  type: onchain
slug: exponential-authentication
source_filename: exponential-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://docs.yo.xyz/yo-risk-graph/agent-api\nnotes: >-\n  YO's HTTP surfaces do not use API keys, OAuth, or OIDC. The Protocol read\n  API (api.yo.xyz) and the public Vault Exposure endpoint (risk.yo.xyz) are\n  fully unauthenticated. The Risk Graph Agent API (risk.yo.xyz/api/v1/agent/*)\n  is not authenticated with a credential either — access is gated by per-call\n  payment via the x402 v2 micropayment protocol: an unpaid request returns 402\n  with an invoice, the caller signs the amount and retries with an X-PAYMENT\n  header, settled on-chain via EIP-3009 transferWithAuthorization in USDC on\n  Base. On-chain writes (deposit/redeem) are authorized by the user's own\n  wallet signature through the yoGateway, not by an API credential.\nsummary:\n  types: [none, payment-gated]\n  api_key_in: []\n  oauth2_flows: []\nschemes:\n  - name: publicRead\n    type: none\n    applies_to:\n      - openapi/exponential-protocol-openapi.yml\n\
  \      - \"risk.yo.xyz /api/v1/public/vault/**\"\n    description: No API key required.\n  - name: x402Payment\n    type: payment\n    scheme: x402\n    header: X-PAYMENT\n    challenge_status: 402\n    network: eip155:8453 (Base mainnet)\n    asset: \"USDC 0x833589fCD6eDb6E08f4c7C32D4f71b54bdA02913\"\n    settlement: EIP-3009 transferWithAuthorization via Coinbase CDP\n    applies_to:\n      - \"risk.yo.xyz /api/v1/agent/**\"\n    description: Per-call payment gate; no onboarding or credential.\n  - name: walletSignature\n    type: onchain\n    applies_to:\n      - yoGateway 0xF1EeE0957267b1A474323Ff9CfF7719E964969FA\n    description: Deposits and redeems are authorized by the user's EVM wallet signature via the yoGateway.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/exponential/refs/heads/main/authentication/exponential-authentication.yml
summary_line: none/payment-gated · 3 schemes
tags:
- Company
- DeFi
- Decentralized Finance
- Yield
- Yield Optimizer
- Vaults
- ERC-4626
- Cross-chain
- Blockchain
- Crypto
- Risk
- Risk Ratings
- Agents
- x402
- Web3
---
