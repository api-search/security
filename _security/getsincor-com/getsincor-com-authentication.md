---
anonymous_access: true
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 4
method: searched
name: Getsincor Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: SINCOR declares 5 security scheme(s) across its OpenAPI definitions.
provider_name: SINCOR
provider_slug: getsincor-com
scheme_count: 5
schemes:
- applies_to:
  - POST /api/a2a message/send (free skills
  - first 5 calls)
  - tasks/get
  - tasks/list
  - tasks/cancel
  - GET /api/a2a/quote
  - GET /api/a2a/agents
  - GET /docs/a2a
  - /.well-known/*
  evidence:
  - quote: POST /api/a2a JSON-RPC message/send | 200. Task created. metadata.caller_id=anonymous, free_call=true, simulation_mode. Did not require the registered agent_id.
    source: https://github.com/OrderofChaos33/SINCOR2/blob/main/docs/A2A_EXTERNAL_WIRE.md
  - detail: 'POST /api/a2a with X-API-Key: invalid returned the same -32602 skill-validation error as the anonymous request; tasks/list returned {"tasks": []} with no credential.'
    source: live probe 2026-09-20
  id: anonymous-free-quota
  note: The quote says "FREE — include caller_id in your tasks/send request (no txHash needed)". caller_id is a self-asserted string, not a credential.
  type: none
- applies_to:
  - POST /api/a2a (per docs/api/README.md)
  evidence:
  - quote: A2A discovery and task execution — Agent Cards advertise an apiKey security scheme using the X-API-Key header.
    source: https://github.com/OrderofChaos33/SINCOR2/blob/main/docs/api/README.md
  - quote: '"authentication": {"description": "Pass your API key in the X-API-Key header. Obtain a key at https://getsincor.com/api-keys.", "schemes": []}'
    source: well-known/getsincor-com-agent.json
  - detail: The canonical card declares NO securitySchemes and NO security, contradicting the docs.
    source: a2a/getsincor-com-agent-card.json
  id: apiKey
  in: header
  key_issuance: https://getsincor.com/api-keys
  key_issuance_status: 404
  name: X-API-Key
  note: Recorded because the provider documents it; not credited as an enforced scheme because the canonical card omits it, the issuance page is dead, and the live endpoint neither required nor validated it.
  status: documented-but-not-observed
  type: apiKey
- applies_to:
  - paid skills — healthcare-credential-check
  - dental-billing-scrub
  - compliance-sbom
  - deal-scoring
  - cashflow-recovery
  - local-business-site-builder
  - toa-decision
  - contract-negotiation
  - quality-audit
  - agent-lifecycle
  - axiom-payment
  - and any free skill after its 5-call quota
  evidence:
  - quote: AXM-only. Pay 6.0000 AXM to pay_to on Base (chain 8453), then include txHash in your tasks/send request. Platform fee 500 bps routes to treasury 0x09E2891432827D8835d2E9b83B25e2a5ba9612Ac.
    source: https://getsincor.com/api/a2a/quote?skill_id=toa-decision
  - detail: 'paymentMethods[0] = {scheme: x402, network: base, chainId: 8453, acceptedTokens: [AXM, USDC, SINC], payTo: 0x09E2…12Ac}; baseCommerce.x402.enabled true.'
    source: a2a/getsincor-com-agent-card.json
  id: payment-as-authorization
  note: Declared as "x402" on the card but executed as pay-first-then-reference; no HTTP 402 challenge was observed. The x402_pricing.yaml in the runtime prices some resources in SINC and healthcare-credential-check in USDC (5.0), while the live quote prices everything in AXM — the live quote is authoritative.
  platform_fee: 500 bps to the treasury (quote field platform_fee_bps)
  settlement: AXM (AXIOM) ERC-20 transfer on Base mainnet (eip155:8453) to treasury 0x09E2891432827D8835d2E9b83B25e2a5ba9612Ac, referenced by txHash in the task request
  type: x-payment
- applies_to:
  - POST /api/auth/login
  - POST /api/auth/verify-token
  - GET /api/auth/profile
  - GET /api/auth/admin/users
  audience: dashboard / operator, not the developer API
  bearerFormat: JWT
  evidence:
  - quote: Dashboard/admin API flows — JWT-backed endpoints under /api/auth rely on standard JWT bearer authorization headers.
    source: https://github.com/OrderofChaos33/SINCOR2/blob/main/docs/api/README.md
  id: jwt-bearer
  scheme: bearer
  type: http
- algorithm: HMAC-SHA256 over the canonical JSON payload (sorted keys, no spaces), hex digest in `signature`
  applies_to:
  - POST /v1/a2a/register
  evidence:
  - detail: register() signs {agent_id, name, capability_tags, rpc_callback, wallet, chain_id} with HMAC-SHA256; the TypeScript client instead POSTs the payload to /api/v1/sign (which returned 404 on 2026-09-20).
    source: https://github.com/OrderofChaos33/SINCOR2/blob/main/sdk/python/sincor_a2a/__init__.py
  - detail: POST /v1/a2a/register {} → HTTP 400 {"error":"capability_tags required"}; GET /v1/kya/directory and GET /v1/quest → 200 JSON; GET /v1/a2a/stream → 200 text/event-stream.
    source: live probe 2026-09-20
  - quote: 'Min stake: 10 AXM. Verify fee: 2 AXM. States: listed -> bound -> staked -> verified | revoked | expired'
    source: https://github.com/OrderofChaos33/SINCOR2/blob/main/docs/KYA_SPEC.md
  id: worker-registration-signature
  identity: wallet address on Base (chain_id 8453) + agent_id; KYA record states listed → bound → staked → verified
  note: This is the surface for agents that want to SELL work into the swarm, not for callers buying it.
  then:
  - POST /v1/a2a/heartbeat every ≤60 s
  - POST /v1/a2a/bids
  - POST /v1/a2a/proofs
  - GET /v1/a2a/stream (SSE)
  type: x-hmac
slug: getsincor-com-authentication
source_filename: getsincor-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: searched\nsource: >-\n  a2a/getsincor-com-agent-card.json (no securitySchemes), well-known/getsincor-com-agent.json (deprecated\n  `authentication` block), https://github.com/OrderofChaos33/SINCOR2/blob/main/docs/api/README.md\n  (Authentication section), https://github.com/OrderofChaos33/SINCOR2/blob/main/docs/A2A_EXTERNAL_WIRE.md\n  (the provider's own external probe log, 2026-09-10), the sdk/python and sdk/typescript clients in the same\n  repository, and live anonymous probes of https://getsincor.com/api/a2a on 2026-09-20.\ndocs: https://github.com/OrderofChaos33/SINCOR2/blob/main/docs/api/README.md#authentication\nchecked: '2026-09-19'\nderived_from: null   # no OpenAPI exists; derive-authentication.py found nothing to read\nsummary: >-\n  SINCOR has no OpenAPI, so the auth profile is read from the agent card, the provider's API reference\n  and observed behaviour. Three patterns coexist and they do not fully agree. (1) The A2A task surface\n\
  \  (POST /api/a2a) accepts ANONYMOUS calls: the canonical card declares no securitySchemes, and the provider's\n  own friction log records that message/send \"accepts anonymous free calls\" with caller_id=anonymous,\n  free_call=true and simulation_mode, up to a free quota of 5 per skill; an invalid X-API-Key was ignored on\n  our probe. (2) The API reference and the LEGACY card advertise an apiKey scheme in the X-API-Key header,\n  \"obtain a key at https://getsincor.com/api-keys\" — that URL returns 404, so there is no public key\n  issuance path today. (3) Paid skills are authorised by PAYMENT, not credentials: the quote says \"pay N AXM\n  to pay_to on Base (chain 8453), then include txHash in your tasks/send request\"; the on-chain transfer\n  to the treasury is the credential. Dashboard/admin routes under /api/auth use JWT bearer tokens\n  (login → verify-token → profile), which is an operator surface rather than a developer one. Worker\n  agents joining the inbound fabric register\
  \ with a wallet + HMAC-SHA256 signature over the payload\n  (/v1/a2a/register) and must heartbeat every 60 s or their KYA listing expires.\nschemes:\n  - id: anonymous-free-quota\n    type: none\n    applies_to: [POST /api/a2a message/send (free skills, first 5 calls), tasks/get, tasks/list, tasks/cancel, GET /api/a2a/quote, GET /api/a2a/agents, GET /docs/a2a, /.well-known/*]\n    evidence:\n      - source: https://github.com/OrderofChaos33/SINCOR2/blob/main/docs/A2A_EXTERNAL_WIRE.md\n        quote: 'POST /api/a2a JSON-RPC message/send | 200. Task created. metadata.caller_id=anonymous, free_call=true, simulation_mode. Did not require the registered agent_id.'\n      - source: live probe 2026-09-20\n        detail: 'POST /api/a2a with X-API-Key: invalid returned the same -32602 skill-validation error as the anonymous request; tasks/list returned {\"tasks\": []} with no credential.'\n    note: 'The quote says \"FREE — include caller_id in your tasks/send request (no txHash needed)\". caller_id\
  \ is a self-asserted string, not a credential.'\n  - id: apiKey\n    type: apiKey\n    in: header\n    name: X-API-Key\n    status: documented-but-not-observed\n    applies_to: [POST /api/a2a (per docs/api/README.md)]\n    key_issuance: https://getsincor.com/api-keys\n    key_issuance_status: 404\n    evidence:\n      - source: https://github.com/OrderofChaos33/SINCOR2/blob/main/docs/api/README.md\n        quote: 'A2A discovery and task execution — Agent Cards advertise an apiKey security scheme using the X-API-Key header.'\n      - source: well-known/getsincor-com-agent.json\n        quote: '\"authentication\": {\"description\": \"Pass your API key in the X-API-Key header. Obtain a key at https://getsincor.com/api-keys.\", \"schemes\": []}'\n      - source: a2a/getsincor-com-agent-card.json\n        detail: 'The canonical card declares NO securitySchemes and NO security, contradicting the docs.'\n    note: >-\n      Recorded because the provider documents it; not credited as an enforced\
  \ scheme because the canonical\n      card omits it, the issuance page is dead, and the live endpoint neither required nor validated it.\n  - id: payment-as-authorization\n    type: x-payment\n    settlement: AXM (AXIOM) ERC-20 transfer on Base mainnet (eip155:8453) to treasury 0x09E2891432827D8835d2E9b83B25e2a5ba9612Ac, referenced by txHash in the task request\n    applies_to: [paid skills — healthcare-credential-check, dental-billing-scrub, compliance-sbom, deal-scoring, cashflow-recovery, local-business-site-builder, toa-decision, contract-negotiation, quality-audit, agent-lifecycle, axiom-payment, and any free skill after its 5-call quota]\n    platform_fee: 500 bps to the treasury (quote field platform_fee_bps)\n    evidence:\n      - source: https://getsincor.com/api/a2a/quote?skill_id=toa-decision\n        quote: 'AXM-only. Pay 6.0000 AXM to pay_to on Base (chain 8453), then include txHash in your tasks/send request. Platform fee 500 bps routes to treasury 0x09E2891432827D8835d2E9b83B25e2a5ba9612Ac.'\n\
  \      - source: a2a/getsincor-com-agent-card.json\n        detail: 'paymentMethods[0] = {scheme: x402, network: base, chainId: 8453, acceptedTokens: [AXM, USDC, SINC], payTo: 0x09E2…12Ac}; baseCommerce.x402.enabled true.'\n    note: >-\n      Declared as \"x402\" on the card but executed as pay-first-then-reference; no HTTP 402 challenge was\n      observed. The x402_pricing.yaml in the runtime prices some resources in SINC and healthcare-credential-check\n      in USDC (5.0), while the live quote prices everything in AXM — the live quote is authoritative.\n  - id: jwt-bearer\n    type: http\n    scheme: bearer\n    bearerFormat: JWT\n    applies_to: [POST /api/auth/login, POST /api/auth/verify-token, GET /api/auth/profile, GET /api/auth/admin/users]\n    audience: dashboard / operator, not the developer API\n    evidence:\n      - source: https://github.com/OrderofChaos33/SINCOR2/blob/main/docs/api/README.md\n        quote: 'Dashboard/admin API flows — JWT-backed endpoints under /api/auth\
  \ rely on standard JWT bearer authorization headers.'\n  - id: worker-registration-signature\n    type: x-hmac\n    algorithm: HMAC-SHA256 over the canonical JSON payload (sorted keys, no spaces), hex digest in `signature`\n    applies_to: [POST /v1/a2a/register]\n    then: [POST /v1/a2a/heartbeat every ≤60 s, POST /v1/a2a/bids, POST /v1/a2a/proofs, GET /v1/a2a/stream (SSE)]\n    identity: wallet address on Base (chain_id 8453) + agent_id; KYA record states listed → bound → staked → verified\n    evidence:\n      - source: https://github.com/OrderofChaos33/SINCOR2/blob/main/sdk/python/sincor_a2a/__init__.py\n        detail: 'register() signs {agent_id, name, capability_tags, rpc_callback, wallet, chain_id} with HMAC-SHA256; the TypeScript client instead POSTs the payload to /api/v1/sign (which returned 404 on 2026-09-20).'\n      - source: live probe 2026-09-20\n        detail: 'POST /v1/a2a/register {} → HTTP 400 {\"error\":\"capability_tags required\"}; GET /v1/kya/directory and GET\
  \ /v1/quest → 200 JSON; GET /v1/a2a/stream → 200 text/event-stream.'\n      - source: https://github.com/OrderofChaos33/SINCOR2/blob/main/docs/KYA_SPEC.md\n        quote: 'Min stake: 10 AXM. Verify fee: 2 AXM. States: listed -> bound -> staked -> verified | revoked | expired'\n    note: 'This is the surface for agents that want to SELL work into the swarm, not for callers buying it.'\noauth2: false\nopenid_connect: false\nmutual_tls: false\ngaps:\n  - 'No securitySchemes on the canonical agent card, so an A2A client cannot discover the (documented) API-key scheme.'\n  - 'The key-issuance page https://getsincor.com/api-keys returns 404.'\n  - 'No /.well-known/oauth-authorization-server or oauth-protected-resource metadata; no dynamic client registration; no delegated identity path.'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/getsincor-com/refs/heads/main/authentication/getsincor-com-authentication.yml
summary_line: 5 schemes
tags:
- Company
- AI Agents
- A2A
- Agentic Commerce
- Agentic Payments
- x402
- Base
- Crypto
- Lead Generation
- Healthcare
- Compliance
- Market Intelligence
- agent-native
---
