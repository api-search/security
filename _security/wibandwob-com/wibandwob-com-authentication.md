---
anonymous_access: true
api_key_in: []
api_specs:
- filename: wibandwob-com-scramble-openapi.yml
  format: yaml
  label: Scramble API
  slug: scramble-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wibandwob-com/refs/heads/main/openapi/wibandwob-com-scramble-openapi.yml
auth_types:
- none
- x402-payment
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: probed
name: Wibandwob Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: Wib&Wob (symbients) secures its APIs with none and x402-payment across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Wib&Wob (symbients)
provider_slug: wibandwob-com
scheme_count: 2
schemes:
- applies_to:
  - GET /api, /api/pet, /api/guestbook, /api/kibble, /api/kibble/testnet, /api/terms, /api/bankr
  - POST /api/sign
  - POST /api/bankr/tip/claim (proof is the confirmed on-chain transaction hash in the body, not a credential)
  - A2A JSON-RPC message/send at / and /a2a
  name: anonymous
  observed: All GETs and the JSON-RPC endpoint returned HTTP 200 with no header of any kind. POST /api/sign and the tip claim were not exercised (permanent write / requires a real transfer) but the provider documents both as "no auth".
  type: none
- applies_to:
  - POST /api/feed
  - POST /api/feed/testnet
  challenge: HTTP 402 with JSON terms in the body and base64 JSON in the PAYMENT-REQUIRED header (observed)
  credential: a signed EIP-3009 transferWithAuthorization for exactly maxAmountRequired (100000 base units USDC) to payTo 0x55c1186ceC287387f9e2c7C8aBD2323a21E88e74, valid until its own validBefore
  header: X-PAYMENT
  in: header
  name: x402Payment
  networks:
    base: '0x833589fCD6eDb6E08f4c7C32D4f71b54bdA02913'
    base-sepolia: '0x036CbD53842c5426634e7929541eC2318f3dCF7e'
  note: One authorization pays for one call; the server cannot initiate a charge. This is per-request payment, not authentication of an identity.
  protocol: x402 v1, scheme exact
  revocation: '"stop sending X-PAYMENT headers. There is no subscription to cancel and no allowance to revoke." (/api/terms)'
  settlement: facilitator.openx402.ai executes the authorization; receipt in the body and the X-PAYMENT-RESPONSE header
  type: payment
slug: wibandwob-com-authentication
source_filename: wibandwob-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: probed\nsource:\n- https://scramble.wibandwob.com/api/pet (GET, no credential -> 200)\n- https://scramble.wibandwob.com/api/kibble (GET, no credential -> 200)\n- https://scramble.wibandwob.com/api/guestbook (GET, no credential -> 200)\n- https://scramble.wibandwob.com/api/feed (POST, no X-PAYMENT -> 402 with x402 terms)\n- https://scramble.wibandwob.com/a2a (POST JSON-RPC, no credential -> 200)\n- https://scramble.wibandwob.com/api/terms\ndocs: https://scramble.wibandwob.com/skill.md\nnote: >-\n  Derived from live probes and the provider's own machine-readable terms, not from an OpenAPI document -\n  the provider publishes no spec and derive-authentication.py was not run. The model is simple and the\n  provider states it plainly: \"No account, no key, no signup\" (agents.md). The only gate anywhere is\n  economic - an x402 payment on the two feed operations - and the provider is explicit that a payment\n  authorization is not a credential (\"\
  This server holds NO private keys ... nothing to revoke\").\nsummary:\n  types: [none, x402-payment]\n  api_key_in: []\n  oauth2_flows: []\n  anonymous_surfaces: 9\n  paid_surfaces: 2\nschemes:\n- name: anonymous\n  type: none\n  applies_to:\n  - GET /api, /api/pet, /api/guestbook, /api/kibble, /api/kibble/testnet, /api/terms, /api/bankr\n  - POST /api/sign\n  - POST /api/bankr/tip/claim (proof is the confirmed on-chain transaction hash in the body, not a credential)\n  - A2A JSON-RPC message/send at / and /a2a\n  observed: All GETs and the JSON-RPC endpoint returned HTTP 200 with no header of any kind. POST /api/sign and the tip claim were not exercised (permanent write / requires a real transfer) but the provider documents both as \"no auth\".\n- name: x402Payment\n  type: payment\n  protocol: x402 v1, scheme exact\n  in: header\n  header: X-PAYMENT\n  applies_to: [POST /api/feed, POST /api/feed/testnet]\n  challenge: HTTP 402 with JSON terms in the body and base64 JSON in the PAYMENT-REQUIRED\
  \ header (observed)\n  credential: a signed EIP-3009 transferWithAuthorization for exactly maxAmountRequired (100000 base units USDC) to payTo 0x55c1186ceC287387f9e2c7C8aBD2323a21E88e74, valid until its own validBefore\n  networks: {base: '0x833589fCD6eDb6E08f4c7C32D4f71b54bdA02913', base-sepolia: '0x036CbD53842c5426634e7929541eC2318f3dCF7e'}\n  settlement: facilitator.openx402.ai executes the authorization; receipt in the body and the X-PAYMENT-RESPONSE header\n  revocation: '\"stop sending X-PAYMENT headers. There is no subscription to cancel and no allowance to revoke.\" (/api/terms)'\n  note: One authorization pays for one call; the server cannot initiate a charge. This is per-request payment, not authentication of an identity.\nidentity:\n  agent_identity_required: false\n  note: The guest book asks for a self-declared name; nothing verifies it. The provider identifies ITSELF with a DID (did:web:wibandwob.com:wibwob in /.well-known/digit.json) but asks no identity of callers.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wibandwob-com/refs/heads/main/authentication/wibandwob-com-authentication.yml
summary_line: none/x402-payment · 2 schemes
tags:
- Company
- Agents
- A2A
- x402
- Micropayments
- USDC
- Base
- Art
- ASCII Art
- Generative Art
- Symbients
- AI Agents
- llms-txt
---
