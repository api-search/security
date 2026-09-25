---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: connskill-com-openapi.yml
  format: yaml
  label: CONNSKILL Growth Services API
  slug: connskill-growth-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/connskill-com/refs/heads/main/openapi/connskill-com-openapi.yml
auth_types:
- apiKey
description: 'CONNSKILL Growth Services has no accounts and no API keys. Access is gated three ways: free routes are open; paid routes are gated by x402 payment (an unpaid request answers 402 with the exact price, and the same request is repeated with a PAYMENT-SIGNATURE header carrying an EIP-3009 USDC authorization on Base); and the private support / redelivery / manual-purchase routes require a Sign-In-With-X wallet proof — a one-use, five-minute EIP-191 signature over a server-issued challenge bound to the method, path and canonical JSON body. The MCP and A2A surfaces inherit the same model: the hosted MCP server forwards payment headers supplied by the caller and the A2A card declares no securitySchemes.'
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Connskill Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: CONNSKILL secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: CONNSKILL
provider_slug: connskill-com
scheme_count: 2
schemes:
- also_used_by:
  - paymentWalletChallenge (issues the proof)
  - private redelivery on any paid route
  - manual X-Payment-Tx purchases
  applied_to:
  - supportTicketsList
  - supportTicketCreate
  - supportTicketGet
  - supportDiscountCheckout
  - supportDiscountClaim
  description: Base64 JSON containing the exact challenge fields, checksummed address, chainId eip155:8453, type eip191 and EIP-191 signature. Free authentication, not payment. One use, five minutes, bound to method, path and JSON body.
  docs: https://agent.connskill.com/v1/support/policy
  failure: 401 Wallet proof missing, invalid, expired or reused; 429 Challenge rate limit; 503 Wallet authentication unavailable; no access granted
  flow:
  - POST /v1/support/challenge (support) or POST /v1/payments/challenge with purpose purchase | redelivery (payments) — returns the exact message to sign and extensions.sign-in-with-x.info
  - sign the message with the EOA wallet that paid (EIP-191)
  - send the info fields plus address, chainId eip155:8453, type eip191 and signature as base64 JSON in the Sign-In-With-X header on the target request
  in: header
  name: signInWithX
  parameter: Sign-In-With-X
  properties:
    chain_id: eip155:8453
    lifetime_seconds: 300
    message_binding:
    - configured public origin
    - method
    - path
    - canonical JSON body
    one_use: true
    ownership: Only the settled payer can access a purchase or its support case
    signature_type: eip191
    supported_wallets: EOA
  sources:
  - openapi/connskill-com-openapi.yml
  - https://agent.connskill.com/v1/support/policy
  type: apiKey
- a2a: capabilities.extensions[0] = a2a-x402 v0.2 (required); paid skills return a payment-required task.
  description: Not an authentication scheme in the OpenAPI components (it is declared per operation via x-payment-info and 402 responses) but the mechanism that actually gates 41 operations. An unpaid request answers HTTP 402 with accepts[0].amount (micro-USDC), accepts[0].payTo, asset (USDC 0x833589fCD6eDb6E08f4c7C32D4f71b54bdA02913), network eip155:8453 and maxTimeoutSeconds; the client signs an EIP-3009 authorization for exactly that amount and repeats the same request with PAYMENT-SIGNATURE.
  docs: https://agent.connskill.com/llms.txt
  free_sample: 'x-free-sample: 1 — one free call per endpoint per UTC day on endpoints priced <= 0.15 USDC'
  in: header
  legacy_parameter: X-Payment
  manual_purchase: Where supported, transfer first, then POST /v1/payments/challenge with purpose purchase, the token payer address and the exact target request (x-payment-tx header, complete JSON body, only ref query parameters) and send the resulting Sign-In-With-X proof on the target request.
  mcp: The hosted MCP server forwards PAYMENT-SIGNATURE / X-Payment from the outer HTTP request and does not sign; the npm server signs with X402_WALLET_KEY under X402_MAX_USD.
  name: x402Payment
  parameter: PAYMENT-SIGNATURE
  pay_to: '0x43B85AE58f0A2505c710Bc715d6f3EB16b1f63dE'
  protocol: x402 v2
  sources:
  - openapi/connskill-com-openapi.yml
  - https://agent.connskill.com/.well-known/x402
  - https://agent.connskill.com/llms.txt
  type: payment
slug: connskill-com-authentication
source_filename: connskill-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: searched\nsource: >-\n  openapi/connskill-com-openapi.yml (components.securitySchemes.signInWithX; info.x-trust.auth; security on 5 support\n  operations; 41 operations with x-payment-info and 402 responses); https://agent.connskill.com/v1/support/policy\n  (authentication block: chainId eip155:8453, type eip191, supportedWallets EOA, lifetimeSeconds 300, oneUse true,\n  challengeUrl /v1/support/challenge, messageBinding); https://agent.connskill.com/llms.txt (\"How one call works\");\n  https://agent.connskill.com/.well-known/agent-card.json (securitySchemes {} / security []);\n  https://agent.connskill.com/.well-known/ai-plugin.json (auth.type none); npm README (X402_WALLET_KEY).\ndocs: https://agent.connskill.com/llms.txt\ndescription: >-\n  CONNSKILL Growth Services has no accounts and no API keys. Access is gated three ways: free routes are open;\n  paid routes are gated by x402 payment (an unpaid request answers 402 with the exact price,\
  \ and the same request\n  is repeated with a PAYMENT-SIGNATURE header carrying an EIP-3009 USDC authorization on Base); and the private\n  support / redelivery / manual-purchase routes require a Sign-In-With-X wallet proof — a one-use, five-minute\n  EIP-191 signature over a server-issued challenge bound to the method, path and canonical JSON body. The MCP and\n  A2A surfaces inherit the same model: the hosted MCP server forwards payment headers supplied by the caller and\n  the A2A card declares no securitySchemes.\nverbatim: >-\n  No account or API key. Manual first purchases and private redelivery require a free Sign-In-With-X wallet proof\n  from POST /v1/payments/challenge.\nsummary:\n  types: [apiKey]\n  api_key_in: [header]\n  accounts: false\n  api_keys: false\n  oauth2: false\n  oidc: false\n  payment_gated: true\n  free_operations: 47\n  paid_operations: 41\n  wallet_proof_operations: 5\nschemes:\n  - name: signInWithX\n    type: apiKey\n    in: header\n    parameter: Sign-In-With-X\n\
  \    description: >-\n      Base64 JSON containing the exact challenge fields, checksummed address, chainId eip155:8453, type eip191 and\n      EIP-191 signature. Free authentication, not payment. One use, five minutes, bound to method, path and JSON body.\n    flow:\n      - POST /v1/support/challenge (support) or POST /v1/payments/challenge with purpose purchase | redelivery\n        (payments) — returns the exact message to sign and extensions.sign-in-with-x.info\n      - sign the message with the EOA wallet that paid (EIP-191)\n      - send the info fields plus address, chainId eip155:8453, type eip191 and signature as base64 JSON in the\n        Sign-In-With-X header on the target request\n    properties:\n      chain_id: eip155:8453\n      signature_type: eip191\n      supported_wallets: EOA\n      lifetime_seconds: 300\n      one_use: true\n      message_binding: [configured public origin, method, path, canonical JSON body]\n      ownership: Only the settled payer can access a purchase\
  \ or its support case\n    applied_to: [supportTicketsList, supportTicketCreate, supportTicketGet, supportDiscountCheckout, supportDiscountClaim]\n    also_used_by: [paymentWalletChallenge (issues the proof), private redelivery on any paid route, manual X-Payment-Tx purchases]\n    failure: '401 Wallet proof missing, invalid, expired or reused; 429 Challenge rate limit; 503 Wallet authentication unavailable; no access granted'\n    docs: https://agent.connskill.com/v1/support/policy\n    sources: [openapi/connskill-com-openapi.yml, https://agent.connskill.com/v1/support/policy]\n  - name: x402Payment\n    type: payment\n    in: header\n    parameter: PAYMENT-SIGNATURE\n    legacy_parameter: X-Payment\n    protocol: x402 v2\n    description: >-\n      Not an authentication scheme in the OpenAPI components (it is declared per operation via x-payment-info and\n      402 responses) but the mechanism that actually gates 41 operations. An unpaid request answers HTTP 402 with\n      accepts[0].amount\
  \ (micro-USDC), accepts[0].payTo, asset (USDC 0x833589fCD6eDb6E08f4c7C32D4f71b54bdA02913),\n      network eip155:8453 and maxTimeoutSeconds; the client signs an EIP-3009 authorization for exactly that amount\n      and repeats the same request with PAYMENT-SIGNATURE.\n    pay_to: '0x43B85AE58f0A2505c710Bc715d6f3EB16b1f63dE'\n    free_sample: 'x-free-sample: 1 — one free call per endpoint per UTC day on endpoints priced <= 0.15 USDC'\n    manual_purchase: >-\n      Where supported, transfer first, then POST /v1/payments/challenge with purpose purchase, the token payer address\n      and the exact target request (x-payment-tx header, complete JSON body, only ref query parameters) and send the\n      resulting Sign-In-With-X proof on the target request.\n    mcp: The hosted MCP server forwards PAYMENT-SIGNATURE / X-Payment from the outer HTTP request and does not sign; the npm server signs with X402_WALLET_KEY under X402_MAX_USD.\n    a2a: capabilities.extensions[0] = a2a-x402 v0.2 (required);\
  \ paid skills return a payment-required task.\n    docs: https://agent.connskill.com/llms.txt\n    sources: [openapi/connskill-com-openapi.yml, https://agent.connskill.com/.well-known/x402, https://agent.connskill.com/llms.txt]\nwell_known:\n  oauth_authorization_server: 404 on agent.connskill.com and connskill.com\n  oauth_protected_resource: 404 on agent.connskill.com and connskill.com\n  openid_configuration: 404 on every host\n  note: There is no OAuth to discover; payment gates access.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/connskill-com/refs/heads/main/authentication/connskill-com-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Company
- API Provider
- SEO
- SERP
- Keyword Research
- x402
- Agentic Payments
- AI Agents
- MCP
- A2A
- SMS Verification
- LLM Inference
- Social Media Marketing
- Web Analytics
- Blockchain Data
- Marketing Agency
- Germany
---
