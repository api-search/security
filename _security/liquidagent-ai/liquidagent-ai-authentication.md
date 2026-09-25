---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: liquidagent-ai-openapi.yml
  format: yaml
  label: Liquid Agent Tokenized Stock Index and Gas Sponsor API
  slug: liquid-agent-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/liquidagent-ai/refs/heads/main/openapi/liquidagent-ai-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Liquidagent Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Liquid Agent secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Liquid Agent
provider_slug: liquidagent-ai
scheme_count: 2
schemes:
- applies_to:
  - get_v1_guide
  - get_v1_basket
  - get_v1_vault_address
  - get_v1_balance_agent
  - get_v1_quote
  - post_v1_create-vault
  - post_v1_set-weights
  - post_v1_buy
  - post_v1_redeem
  - post_v1_rebalance
  - post_v1_send
  description: Sign-In with X wallet identity (EIP-4361). Optional; no payment.
  in: header
  name: siwx
  observed: All eleven operations answer 200 without the header (probed 2026-09-19), so the scheme is identity, not access control.
  parameter: SIGN-IN-WITH-X
  required: false
  sources:
  - openapi/liquidagent-ai-openapi.yml
  type: apiKey
- applies_to:
  - getV1Signals
  - postV1Publish
  - postV1Gas
  - postV1GasSolana
  description: Pay-per-call via x402 (exact scheme, EIP-3009 USDC on Base eip155:8453 or Polygon eip155:137). Sign a USDC authorization; no account, no key held by the server.
  name: x402
  protocol:
    challenge: HTTP 402; body is the PaymentRequired JSON {x402Version, error, resource, accepts[], extensions}; the same JSON base64-encoded in PAYMENT-REQUIRED and X-PAYMENT-REQUIRED response headers
    erc7677_in_band: On POST /v1/gas JSON-RPC calls HTTP is always 200; an unpaid pm_getPaymasterData returns a JSON-RPC error {code:402, data:<PaymentRequired>} and the payment object goes in params[3].context.x402
    evm_authorization: EIP-3009 transferWithAuthorization on USDC - Base 0x833589fCD6eDb6E08f4c7C32D4f71b54bdA02913, Polygon 0x3c499c542cEF5E3811e1192ce70d8cC03d5c3359; accepts[].extra carries {name USD Coin, version 2, chainId, verifyingContract}
    facilitator: PayAI (named in the gas-sponsor SKILL.md)
    payTo:
      evm: '0x487b28A4FbbA8Cf46eb6E1d72e6959202Bb75e90'
      solana: BBcAL97dyJPGmsjQ7pPxCdUsFk1wgZ6jqYQ4DFvCVHkn
    payment_header: X-PAYMENT (PAYMENT-SIGNATURE also accepted on the Solana lane)
    scheme: exact
    solana_authorization: one USDC TransferChecked of exactly accepts[].amount to the sponsor's USDC account, sponsor as fee payer, wrapped as {x402Version:2, scheme:exact, network, accepted, payload:{transaction}} and base64d
    timeout: maxTimeoutSeconds 60 per accepts[] entry
    version: 2
  required: true
  scheme: x402
  sources:
  - openapi/liquidagent-ai-openapi.yml
  - https://api.liquidagent.ai/v1/signals (live 402)
  - https://api.liquidagent.ai/v1/gas (live 402)
  type: http
slug: liquidagent-ai-authentication
source_filename: liquidagent-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: searched\nsource: openapi/liquidagent-ai-openapi.yml\ndocs: https://api.liquidagent.ai/v1/guide\ndocs_also:\n- https://api.liquidagent.ai/llms.txt\n- https://api.liquidagent.ai/v1/gas?docs=1\n- https://api.liquidagent.ai/.well-known/x402-resources\n- https://raw.githubusercontent.com/LiquidAgent/liquidagentx402/main/skills/liquid-gas-sponsor/SKILL.md\nsummary:\n  types: [apiKey, http]\n  api_key_in: [header]\n  accounts: false\n  api_keys_issued: false\n  oauth2_flows: []\n  model: >-\n    No account, no API key, no allowlist. Eleven free operations accept an OPTIONAL wallet identity (SIWX,\n    EIP-4361, in a SIGN-IN-WITH-X header) and work anonymously without it - observed live: every free read\n    answered 200 with no headers at all. Four paid operations are gated by x402 v2 payment rather than identity:\n    the server answers 402 with a PaymentRequired document, the caller signs a USDC authorization for exactly the\n    quoted amount and\
  \ retries with it in an X-PAYMENT (or PAYMENT-SIGNATURE) header. The server holds no key and\n    never signs; the caller's own wallet is the only credential anywhere in the system.\nschemes:\n- name: siwx\n  type: apiKey\n  in: header\n  parameter: SIGN-IN-WITH-X\n  description: Sign-In with X wallet identity (EIP-4361). Optional; no payment.\n  required: false\n  applies_to: [get_v1_guide, get_v1_basket, get_v1_vault_address, get_v1_balance_agent, get_v1_quote, post_v1_create-vault, post_v1_set-weights, post_v1_buy, post_v1_redeem, post_v1_rebalance, post_v1_send]\n  observed: All eleven operations answer 200 without the header (probed 2026-09-19), so the scheme is identity, not access control.\n  sources: [openapi/liquidagent-ai-openapi.yml]\n- name: x402\n  type: http\n  scheme: x402\n  description: Pay-per-call via x402 (exact scheme, EIP-3009 USDC on Base eip155:8453 or Polygon eip155:137). Sign a USDC authorization; no account, no key held by the server.\n  required: true\n  applies_to:\
  \ [getV1Signals, postV1Publish, postV1Gas, postV1GasSolana]\n  protocol:\n    version: 2\n    scheme: exact\n    challenge: 'HTTP 402; body is the PaymentRequired JSON {x402Version, error, resource, accepts[], extensions}; the same JSON base64-encoded in PAYMENT-REQUIRED and X-PAYMENT-REQUIRED response headers'\n    payment_header: X-PAYMENT (PAYMENT-SIGNATURE also accepted on the Solana lane)\n    evm_authorization: EIP-3009 transferWithAuthorization on USDC - Base 0x833589fCD6eDb6E08f4c7C32D4f71b54bdA02913, Polygon 0x3c499c542cEF5E3811e1192ce70d8cC03d5c3359; accepts[].extra carries {name USD Coin, version 2, chainId, verifyingContract}\n    solana_authorization: one USDC TransferChecked of exactly accepts[].amount to the sponsor's USDC account, sponsor as fee payer, wrapped as {x402Version:2, scheme:exact, network, accepted, payload:{transaction}} and base64d\n    payTo: {evm: '0x487b28A4FbbA8Cf46eb6E1d72e6959202Bb75e90', solana: BBcAL97dyJPGmsjQ7pPxCdUsFk1wgZ6jqYQ4DFvCVHkn}\n    timeout:\
  \ maxTimeoutSeconds 60 per accepts[] entry\n    erc7677_in_band: On POST /v1/gas JSON-RPC calls HTTP is always 200; an unpaid pm_getPaymasterData returns a JSON-RPC error {code:402, data:<PaymentRequired>} and the payment object goes in params[3].context.x402\n    facilitator: PayAI (named in the gas-sponsor SKILL.md)\n  sources: [openapi/liquidagent-ai-openapi.yml, https://api.liquidagent.ai/v1/signals (live 402), https://api.liquidagent.ai/v1/gas (live 402)]\nsigning_is_not_authentication:\n  note: >-\n    The six transaction builders return unsigned calldata or EIP-712 typed data; the caller signs with the wallet\n    that owns the funds and broadcasts to Base itself. That signature authorizes the on-chain action, not the API\n    call - the API call needs nothing. Consequently there is nothing to rotate, revoke or leak on the API side.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/liquidagent-ai/refs/heads/main/authentication/liquidagent-ai-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Tokenized Stocks
- DeFi
- Investing
- Agentic Commerce
- x402
- Stablecoins
- Account Abstraction
- Gas Sponsorship
- Base
- Solana
- AI Agents
- Agent-Native
- A2A
- Portfolio Management
- Market Data
---
