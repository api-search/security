---
anonymous_access: true
api_key_in: []
auth_types:
- payment
- none
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Verse Me Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: Verse (autonomous agent) secures its APIs with payment and none across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Verse (autonomous agent)
provider_slug: verse-me-com
scheme_count: 3
schemes:
- applies_to:
  - consultation (POST /expertise/consultation)
  - epistemic_audit (POST /expertise/epistemic-audit)
  - edgar_financial_intelligence (POST /expertise/edgar)
  - strategy_recommendation (routed through the consultation endpoint per the card)
  asset: USDC
  asset_contract: '0x833589fCD6eDb6E08f4c7C32D4f71b54bdA02913'
  description: 'Verbatim from the card: "x402 HTTP payment protocol. Client receives 402 response with payment requirements, pays onchain (Base USDC), retries with payment receipt header. No API keys or accounts needed." gettingStarted step 2: "Verse replies with the price first, usually $3–$25 USDC on Base ... sign the payment authorization with your wallet and retry the request with the receipt." The card''s CORS headers (Access-Control-Allow-Headers: Content-Type, PAYMENT-SIGNATURE, X-PAYMENT, X-Console-Token; Access-Control-Expose-Headers: PAYMENT-REQUIRED, PAYMENT-RESPONSE) name the request and response headers the payment flow uses. A planned second rail is named (x402 on Canton, asset USDCx) but not live.'
  facilitator: https://openfacilitator.io
  headers_named_by_edge:
  - PAYMENT-SIGNATURE
  - X-PAYMENT
  in: header (payment receipt on the retried request)
  name: x402Payment
  network: eip155:8453 (Base mainnet)
  observed: Not observed. POST /expertise/consultation without payment returned the Cloudflare challenge (403), so the 402 body and PaymentRequirements shape are unverified.
  pay_to: '0x1060D0B596685Ff429BD64f41611f5D1d15f1659'
  response_headers_named_by_edge:
  - PAYMENT-REQUIRED
  - PAYMENT-RESPONSE
  sources:
  - https://api.verse-me.com/.well-known/agent.json
  standard: x402 (HTTP 402)
  type: payment
- applies_to:
  - calibration_track_record (GET /expertise/calibration)
  - calibration_history (GET /expertise/calibration/history)
  - signed_calibration (GET /expertise/calibration/signed, GET /expertise/calibration/history/signed)
  - reputation / proof bundle (GET /reputation)
  - price estimate (POST /expertise/consultation/price-estimate)
  description: 'Verbatim: "No authentication required. Public read-only access." The AGP policy for these capabilities is requiresAuth false, cost 0, dataScope aggregate_only.'
  name: public
  observed: 'Not reachable by a non-browser client: GET /expertise/calibration returned the Cloudflare managed challenge (403, cf-mitigated: challenge) under three different User-Agents and Accept: application/json. The endpoint is public in policy and challenged at the edge in practice, which is the gap an agent will hit first.'
  sources:
  - https://api.verse-me.com/.well-known/agent.json
  type: none
- audience: internal (inferred from the name only)
  description: Not declared in the card. Appears only in the Access-Control-Allow-Headers of the card response alongside the payment headers. Recorded because it is observable; its purpose is undocumented and it should not be treated as a customer credential.
  in: header
  name: X-Console-Token
  parameter: X-Console-Token
  sources:
  - HTTP response headers of https://api.verse-me.com/.well-known/agent.json
  type: apiKey
slug: verse-me-com-authentication
source_filename: verse-me-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: searched\nsource: https://api.verse-me.com/.well-known/agent.json\ndocs:\n- https://api.verse-me.com/.well-known/agent.json\nspec: null\nsummary:\n  types:\n  - payment\n  - none\n  api_key_in: []\n  oauth2_flows: []\n  bearer: false\n  credential_classes: 2\n  headline: >-\n    No account, no API key, no signup. Verse's only credential is money: paid endpoints answer HTTP 402 with x402\n    payment requirements, the caller pays USDC on Base and retries with the payment receipt header; the calibration\n    and reputation endpoints are declared public. There is no OpenAPI, so derive-authentication.py had nothing to\n    read — the profile is the agent card's securitySchemes / securityRequirements plus the x402 block in its\n    extensions. None of it could be exercised live: every application path answers a Cloudflare managed challenge\n    to a non-browser client.\nschemes:\n- name: x402Payment\n  type: payment\n  standard: x402 (HTTP 402)\n\
  \  in: header (payment receipt on the retried request)\n  headers_named_by_edge: [PAYMENT-SIGNATURE, X-PAYMENT]\n  response_headers_named_by_edge: [PAYMENT-REQUIRED, PAYMENT-RESPONSE]\n  network: eip155:8453 (Base mainnet)\n  asset: USDC\n  asset_contract: '0x833589fCD6eDb6E08f4c7C32D4f71b54bdA02913'\n  facilitator: https://openfacilitator.io\n  pay_to: '0x1060D0B596685Ff429BD64f41611f5D1d15f1659'\n  applies_to:\n  - consultation (POST /expertise/consultation)\n  - epistemic_audit (POST /expertise/epistemic-audit)\n  - edgar_financial_intelligence (POST /expertise/edgar)\n  - strategy_recommendation (routed through the consultation endpoint per the card)\n  description: >-\n    Verbatim from the card: \"x402 HTTP payment protocol. Client receives 402 response with payment requirements,\n    pays onchain (Base USDC), retries with payment receipt header. No API keys or accounts needed.\" gettingStarted\n    step 2: \"Verse replies with the price first, usually $3–$25 USDC on Base ... sign\
  \ the payment authorization\n    with your wallet and retry the request with the receipt.\" The card's CORS headers (Access-Control-Allow-Headers:\n    Content-Type, PAYMENT-SIGNATURE, X-PAYMENT, X-Console-Token; Access-Control-Expose-Headers: PAYMENT-REQUIRED,\n    PAYMENT-RESPONSE) name the request and response headers the payment flow uses. A planned second rail is\n    named (x402 on Canton, asset USDCx) but not live.\n  observed: >-\n    Not observed. POST /expertise/consultation without payment returned the Cloudflare challenge (403), so the\n    402 body and PaymentRequirements shape are unverified.\n  sources:\n  - https://api.verse-me.com/.well-known/agent.json\n- name: public\n  type: none\n  applies_to:\n  - calibration_track_record (GET /expertise/calibration)\n  - calibration_history (GET /expertise/calibration/history)\n  - signed_calibration (GET /expertise/calibration/signed, GET /expertise/calibration/history/signed)\n  - reputation / proof bundle (GET /reputation)\n \
  \ - price estimate (POST /expertise/consultation/price-estimate)\n  description: 'Verbatim: \"No authentication required. Public read-only access.\" The AGP policy for these capabilities is requiresAuth false, cost 0, dataScope aggregate_only.'\n  observed: >-\n    Not reachable by a non-browser client: GET /expertise/calibration returned the Cloudflare managed challenge\n    (403, cf-mitigated: challenge) under three different User-Agents and Accept: application/json. The endpoint\n    is public in policy and challenged at the edge in practice, which is the gap an agent will hit first.\n  sources:\n  - https://api.verse-me.com/.well-known/agent.json\n- name: X-Console-Token\n  type: apiKey\n  in: header\n  parameter: X-Console-Token\n  audience: internal (inferred from the name only)\n  description: >-\n    Not declared in the card. Appears only in the Access-Control-Allow-Headers of the card response alongside the\n    payment headers. Recorded because it is observable; its purpose is\
  \ undocumented and it should not be treated\n    as a customer credential.\n  sources:\n  - HTTP response headers of https://api.verse-me.com/.well-known/agent.json\ndiscovery:\n  oauth_authorization_server: 404\n  oauth_protected_resource: 404\n  openid_configuration: 404\nidentity_and_provenance:\n  agent_identity: Ed25519 key published in the card (fingerprint 153b303b701f1a67) signs outputs; ERC-8004 agentId 29481 on Base, owner wallet = payTo wallet (verified on-chain).\n  note: These authenticate Verse to its callers; they are not caller credentials.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/verse-me-com/refs/heads/main/authentication/verse-me-com-authentication.yml
summary_line: payment/none · 3 schemes
tags:
- Company
- AI Agents
- Autonomous Agents
- A2A
- x402
- Agentic Commerce
- Forecasting
- Predictions
- Calibration
- Financial Analysis
- SEC EDGAR
- Blockchain
- Base
- Agent-Native
---
