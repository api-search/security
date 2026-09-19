---
anonymous_access: false
api_key_in: []
api_specs:
- filename: x402-proxy-openapi-original.json
  format: json
  label: x402-proxy API
  slug: x402-proxy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/x402-proxy/refs/heads/main/openapi/x402-proxy-openapi-original.json
auth_types:
- x402-payment-challenge
- wallet-signature
- email-magic-link
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: X402 Proxy Authentication
name_suffix: Authentication
oauth_flows: []
overview: x402-proxy secures its APIs with x402-payment-challenge, wallet-signature, and email-magic-link across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: x402-proxy
provider_slug: x402-proxy
scheme_count: 3
schemes:
- applies_to: caller
  asset: 749071750893463290574776461331093852760741783827
  description: Paid routes answer HTTP 402 with x402 payment terms; the caller pays USDC on Base (eip155:8453) and retries with the PAYMENT-SIGNATURE header (x402 v2) or X-PAYMENT header (v1). No accounts, no API keys.
  headers:
  - PAYMENT-SIGNATURE
  - X-PAYMENT
  name: x402
  network: eip155:8453
  scheme: x402
  sources:
  - well-known/x402-proxy-x402.json
  - a2a/x402-proxy-agent-card.json
  type: payment-challenge
- applies_to: creator-dashboard
  description: Route creators authenticate by signing with a Base/Ethereum wallet (Coinbase Wallet or MetaMask); signature-only, no on-chain transaction.
  name: wallet-signature
  scheme: siwe-style
  sources:
  - https://proxy.forgemesh.io/faq
  type: wallet-signin
- applies_to: creator-dashboard
  description: Route creators can instead request an emailed sign-in link; a wallet can be linked later for payouts.
  name: email-magic-link
  scheme: email
  sources:
  - https://proxy.forgemesh.io/faq
  type: magic-link
slug: x402-proxy-authentication
source_filename: x402-proxy-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-17'\nmethod: searched\nsource: https://proxy.forgemesh.io/.well-known/agent-card.json + https://proxy.forgemesh.io/faq\nnote: >-\n  The OpenAPI declares no formal securitySchemes, so this profile is authored from the published agent\n  card (securitySchemes.x402) and the FAQ. Two distinct surfaces: (1) the CALLER side — paid /p/:slug\n  routes are gated only by an x402 HTTP 402 payment challenge, no accounts or API keys; (2) the CREATOR\n  side — route owners sign in with an Ethereum wallet signature or an emailed magic link.\nsummary:\n  types:\n  - x402-payment-challenge\n  - wallet-signature\n  - email-magic-link\n  api_key_in: []\n  oauth2_flows: []\nschemes:\n- name: x402\n  type: payment-challenge\n  scheme: x402\n  description: >-\n    Paid routes answer HTTP 402 with x402 payment terms; the caller pays USDC on Base (eip155:8453) and\n    retries with the PAYMENT-SIGNATURE header (x402 v2) or X-PAYMENT header (v1). No accounts, no API keys.\n  network:\
  \ eip155:8453\n  asset: 0x833589fCD6eDb6E08f4c7C32D4f71b54bdA02913\n  headers:\n  - PAYMENT-SIGNATURE\n  - X-PAYMENT\n  applies_to: caller\n  sources:\n  - well-known/x402-proxy-x402.json\n  - a2a/x402-proxy-agent-card.json\n- name: wallet-signature\n  type: wallet-signin\n  scheme: siwe-style\n  description: Route creators authenticate by signing with a Base/Ethereum wallet (Coinbase Wallet or\n    MetaMask); signature-only, no on-chain transaction.\n  applies_to: creator-dashboard\n  sources:\n  - https://proxy.forgemesh.io/faq\n- name: email-magic-link\n  type: magic-link\n  scheme: email\n  description: Route creators can instead request an emailed sign-in link; a wallet can be linked later\n    for payouts.\n  applies_to: creator-dashboard\n  sources:\n  - https://proxy.forgemesh.io/faq\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/x402-proxy/refs/heads/main/authentication/x402-proxy-authentication.yml
summary_line: x402-payment-challenge/wallet-signature/email-magic-link · 3 schemes
tags:
- api-monetization
- payments
- x402
- micropayments
- usdc
- stablecoin
- base-l2
- blockchain
- web3
- agentic-commerce
- ai-agents
- api-proxy
- api-gateway
- pay-per-use
---
