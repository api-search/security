---
anonymous_access: false
api_key_in: []
api_specs:
- filename: lvlltd-com-openapi.yml
  format: yaml
  label: LVL LTD Agent Skill Market API
  slug: lvl-ltd-agent-skill-market-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lvlltd-com/refs/heads/main/openapi/lvlltd-com-openapi.yml
auth_types:
- none
- x402-payment-proof
description: ''
kind: authentication
layout: security
mechanism_count: 4
method: searched
name: Lvlltd Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: LVL LTD CO secures its APIs with none and x402-payment-proof across 5 declared security schemes, as derived from its OpenAPI definitions.
provider_name: LVL LTD CO
provider_slug: lvlltd-com
scheme_count: 5
schemes:
- applies_to:
  - POST /api/pay (unlock)
  - POST /api/recover
  - MCP purchase_skill / install_skill_payload / subscribe_plan tx_hash argument
  format: JSON {"txHash":"0x…","skill":"<id>"} (also accepted as the request body)
  idempotent: true — same (txHash, skill) re-downloads the pack without re-charging
  in: header
  name: x402_payment_proof
  obtained_by: GET /api/pay?skill=<id> -> HTTP 402 challenge -> ERC-20 USDC transfer on Base (eip155:8453) of maxAmountRequired to payTo -> the transaction hash
  parameter: X-PAYMENT
  purpose: payment proof, not identity
  sources:
  - openapi/lvlltd-com-openapi.yml#POST /api/pay parameters.X-PAYMENT
  - a2a/lvlltd-com-agent-card.json securitySchemes.x402_http
  - https://lvlltd.com/docs/REFERENCE.md
  type: apiKey
- applies_to:
  - POST /api/pay
  format: EIP-3009 transferWithAuthorization typed data signed with eth_signTypedData_v4 from the 402's wallet_next_action
  in: header
  name: x402_payment_signature
  parameter: PAYMENT-SIGNATURE
  purpose: signed payment authorization (no on-chain broadcast by the buyer)
  sources:
  - https://lvlltd.com/api/x402
  - https://lvlltd.com/SKILL.md (step 5)
  - CORS Access-Control-Allow-Headers on /api/pay
  type: apiKey
  verified_by: Coinbase CDP x402 facilitator (https://api.cdp.coinbase.com/platform/v2/x402/verify + /settle) — "primary" path per /api/x402; on-chain receipt scan is the fallback
- applies_to:
  - POST /api/pay -> verified_authorized_purchase
  failure: 403 AP2_MANDATE_REJECTED
  format: mandate_id (md_…) or a full AP2 IntentMandate signed with EIP-191; registered via POST /api/mandates
  in: header
  name: ap2_mandate
  parameter: X-AP2-MANDATE
  purpose: optional authorization layer (a human-signed spend mandate), never required to buy
  sources:
  - openapi/lvlltd-com-openapi.yml#POST /api/pay parameters.X-AP2-MANDATE
  - https://lvlltd.com/api/mandates
  type: apiKey
- in: header
  name: capability_token
  parameter: X-CAPABILITY
  purpose: short-lived capability token (P1 rail) — "not an API key for purchase"
  sources:
  - mcp/lvlltd-com-mcp-tools-list.json#get_capability_info
  status: described only by the MCP tool get_capability_info and the CORS allow-list; no issuance endpoint is documented (/api/capabilities 404)
  type: apiKey
- in: body
  name: license_token
  parameter: license.token
  purpose: optional portable re-redeem token returned by a successful unlock ("when KV bound"); 403 INVALID_LICENSE if bad
  sources:
  - https://lvlltd.com/docs/REFERENCE.md#unlock-response-post--200
  type: apiKey
slug: lvlltd-com-authentication
source_filename: lvlltd-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: searched\nsource: openapi/lvlltd-com-openapi.yml (declares NO securitySchemes; the X-PAYMENT and X-AP2-MANDATE header parameters on POST /api/pay are the only auth-shaped elements)\ndocs:\n- https://lvlltd.com/docs/REFERENCE.md\n- https://lvlltd.com/how-to/agent-setup/\n- https://lvlltd.com/api/x402\n- https://lvlltd.com/.well-known/agent-card.json (securitySchemes x402_http, ap2_mandate)\n- https://lvlltd.com/.well-known/oauth-protected-resource\n- https://lvlltd.com/docs/AGENT-RAILS-2026.md (\"Wallet-native buy — No API key required for first-party unlocks\")\nsummary:\n  types: [none, x402-payment-proof]\n  api_key_in: []\n  oauth2_flows: []\n  model: >-\n    Anonymous reads; payment proof instead of credentials for writes that deliver value. There are no\n    accounts, no API keys and no OAuth: an agent discovers, searches and evaluates with no header at all,\n    then proves a Base USDC payment on POST /api/pay. The provider's own documents\
  \ call this\n    \"wallet-native buy\" and the MCP manifest's deployment.auth is none. derive-authentication.py found 0\n    schemes because the OpenAPI declares none; the overlay adds three header schemes so downstream\n    tooling can see them.\nschemes:\n- name: x402_payment_proof\n  type: apiKey\n  in: header\n  parameter: X-PAYMENT\n  purpose: payment proof, not identity\n  format: 'JSON {\"txHash\":\"0x…\",\"skill\":\"<id>\"} (also accepted as the request body)'\n  obtained_by: GET /api/pay?skill=<id> -> HTTP 402 challenge -> ERC-20 USDC transfer on Base (eip155:8453) of maxAmountRequired to payTo -> the transaction hash\n  applies_to: [POST /api/pay (unlock), POST /api/recover, MCP purchase_skill / install_skill_payload / subscribe_plan tx_hash argument]\n  idempotent: true — same (txHash, skill) re-downloads the pack without re-charging\n  sources: [openapi/lvlltd-com-openapi.yml#POST /api/pay parameters.X-PAYMENT, a2a/lvlltd-com-agent-card.json securitySchemes.x402_http, https://lvlltd.com/docs/REFERENCE.md]\n\
  - name: x402_payment_signature\n  type: apiKey\n  in: header\n  parameter: PAYMENT-SIGNATURE\n  purpose: signed payment authorization (no on-chain broadcast by the buyer)\n  format: EIP-3009 transferWithAuthorization typed data signed with eth_signTypedData_v4 from the 402's wallet_next_action\n  verified_by: Coinbase CDP x402 facilitator (https://api.cdp.coinbase.com/platform/v2/x402/verify + /settle) — \"primary\" path per /api/x402; on-chain receipt scan is the fallback\n  applies_to: [POST /api/pay]\n  sources: [https://lvlltd.com/api/x402, https://lvlltd.com/SKILL.md (step 5), CORS Access-Control-Allow-Headers on /api/pay]\n- name: ap2_mandate\n  type: apiKey\n  in: header\n  parameter: X-AP2-MANDATE\n  purpose: optional authorization layer (a human-signed spend mandate), never required to buy\n  format: mandate_id (md_…) or a full AP2 IntentMandate signed with EIP-191; registered via POST /api/mandates\n  applies_to: [POST /api/pay -> verified_authorized_purchase]\n  failure: 403\
  \ AP2_MANDATE_REJECTED\n  sources: [openapi/lvlltd-com-openapi.yml#POST /api/pay parameters.X-AP2-MANDATE, https://lvlltd.com/api/mandates]\n- name: capability_token\n  type: apiKey\n  in: header\n  parameter: X-CAPABILITY\n  purpose: short-lived capability token (P1 rail) — \"not an API key for purchase\"\n  status: described only by the MCP tool get_capability_info and the CORS allow-list; no issuance endpoint is documented (/api/capabilities 404)\n  sources: [mcp/lvlltd-com-mcp-tools-list.json#get_capability_info]\n- name: license_token\n  type: apiKey\n  in: body\n  parameter: license.token\n  purpose: optional portable re-redeem token returned by a successful unlock (\"when KV bound\"); 403 INVALID_LICENSE if bad\n  sources: [https://lvlltd.com/docs/REFERENCE.md#unlock-response-post--200]\ndeclared_but_absent:\n- name: OAuth 2.0 bearer\n  evidence: >-\n    /.well-known/oauth-protected-resource lists scopes_supported [agent:read, agent:execute, x402:pay,\n    openid] and bearer_methods_supported\
  \ [header], and the /api/a2a CORS allow-list includes Authorization\n    — but the named authorization server (https://lvlltd.com) publishes no RFC 8414 or OIDC metadata,\n    no token endpoint exists, and no operation documents a bearer token. See scopes/lvlltd-com-scopes.yml.\nidentity_note: >-\n  Identity, where it exists, is a wallet address: purchases, access resolution, meter budgets, mandates\n  and ERC-8004 lookups are all keyed on 0x addresses. Privacy policy section 8 recommends \"a fresh wallet\n  if you prefer not to link purchases to a known address\".\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lvlltd-com/refs/heads/main/authentication/lvlltd-com-authentication.yml
summary_line: none/x402-payment-proof · 5 schemes
tags:
- Agents
- Agentic Commerce
- Agent Skills
- A2A
- MCP
- x402
- Micropayments
- Stablecoins
- Marketplace
- Agent-Native
- United States
---
