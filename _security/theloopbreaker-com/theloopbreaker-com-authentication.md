---
anonymous_access: true
api_key_in: []
api_specs:
- filename: theloopbreaker-com-openapi.yml
  format: yaml
  label: Vaultfire Agent Hub API
  slug: vaultfire-agent-hub-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/theloopbreaker-com/refs/heads/main/openapi/theloopbreaker-com-openapi.yml
auth_types:
- none
- erc-8128-http-signature
- x402-payment
- wallet-signature
description: ''
kind: authentication
layout: security
mechanism_count: 4
method: searched
name: Theloopbreaker Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: Vaultfire Protocol secures its APIs with none, erc-8128-http-signature, x402-payment, and wallet-signature across 5 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Vaultfire Protocol
provider_slug: theloopbreaker-com
scheme_count: 5
schemes:
- applies_to: every GET operation in openapi/theloopbreaker-com-openapi.yml and the two free x402 endpoints (/api/x402/trust/health, /api/x402/oracle/chainlink-status)
  evidence: GET /api/agent/status?address=0xfA15...813C -> 200 with no credential (2026-09-19)
  name: publicRead
  type: none
- applies_to: routeTask (POST /agent/route) — observed; possibly other write operations, which the spec does not say
  documented_in_spec: false
  evidence: POST /api/agent/route {} -> 401 {"error":"unsigned","reason":"Request is missing ERC-8128 Signature and/or Signature-Input headers"}
  headers:
  - Signature
  - Signature-Input
  name: erc8128HttpSignature
  standard: ERC-8128 (profile of RFC 9421 HTTP Message Signatures, signed by the agent wallet key)
  type: http-message-signature
- applies_to: 75 priced endpoints under /api/x402/* (well-known/theloopbreaker-com-x402.json)
  evidence: 402 challenge observed on GET /api/x402/bonds/agent-bond-status and POST /api/x402/actions/accept-bid
  facilitator: https://api.cdp.coinbase.com/platform/v2/x402
  headers:
  - PAYMENT-SIGNATURE (request)
  - PAYMENT-REQUIRED (402 challenge)
  - PAYMENT-RESPONSE (settled response)
  name: x402Payment
  standard: x402 v2, scheme exact, USDC on Base (eip155:8453)
  type: payment
- applies_to: registerAgent, createBond, prepareTask, prepareVKPAction — the API returns an unsigned transaction / contract ABI; state changes happen only when the caller signs and broadcasts with their own wallet
  evidence: OpenAPI response descriptions ("Unsigned transaction to submit on-chain"); agent card authentication.note; Terms section 3 (self-custody)
  name: walletSignature
  type: self-custody
- applies_to: the two write tools of the stdio MCP server (vaultfire_register_agent, vaultfire_create_bond)
  evidence: '@vaultfire/mcp-server README, "Write Tools (require PRIVATE_KEY env var)"'
  name: mcpPrivateKey
  note: A wallet private key held by the local process, never sent to Vaultfire.
  type: environment-secret
  variable: PRIVATE_KEY
slug: theloopbreaker-com-authentication
source_filename: theloopbreaker-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: searched\ndocs: https://theloopbreaker.com/llms.txt\nsource: >-\n  derive-authentication.py found no securitySchemes (components.securitySchemes is {} and no global or\n  per-operation security[] in openapi/theloopbreaker-com-openapi.yml). The profile below is therefore from\n  the provider's own statements — the OpenAPI info.description (\"All endpoints are public and require no\n  authentication for reads\"), the agent card (authentication.schemes [\"none\"]; \"Write endpoints return\n  unsigned transactions for the caller to sign\"), ai-plugin.json (auth.type none), SKILL.md (\"ERC-8128 —\n  signed HTTP requests from agent wallets — request authentication without API keys\"), the @vaultfire/mcp-server\n  README (PRIVATE_KEY env for write tools) — and from live 2026-09-19 probes.\nsummary:\n  types: [none, erc-8128-http-signature, x402-payment, wallet-signature]\n  api_key_in: []\n  oauth2_flows: []\n  api_keys: false\n  oauth2: false\n  oidc:\
  \ false\n  mtls: false\nschemes:\n  - name: publicRead\n    type: none\n    applies_to: every GET operation in openapi/theloopbreaker-com-openapi.yml and the two free x402 endpoints (/api/x402/trust/health, /api/x402/oracle/chainlink-status)\n    evidence: 'GET /api/agent/status?address=0xfA15...813C -> 200 with no credential (2026-09-19)'\n  - name: erc8128HttpSignature\n    type: http-message-signature\n    standard: ERC-8128 (profile of RFC 9421 HTTP Message Signatures, signed by the agent wallet key)\n    headers: [Signature, Signature-Input]\n    applies_to: routeTask (POST /agent/route) — observed; possibly other write operations, which the spec does not say\n    evidence: 'POST /api/agent/route {} -> 401 {\"error\":\"unsigned\",\"reason\":\"Request is missing ERC-8128 Signature and/or Signature-Input headers\"}'\n    documented_in_spec: false\n  - name: x402Payment\n    type: payment\n    standard: x402 v2, scheme exact, USDC on Base (eip155:8453)\n    headers: [PAYMENT-SIGNATURE\
  \ (request), PAYMENT-REQUIRED (402 challenge), PAYMENT-RESPONSE (settled response)]\n    applies_to: 75 priced endpoints under /api/x402/* (well-known/theloopbreaker-com-x402.json)\n    facilitator: https://api.cdp.coinbase.com/platform/v2/x402\n    evidence: '402 challenge observed on GET /api/x402/bonds/agent-bond-status and POST /api/x402/actions/accept-bid'\n  - name: walletSignature\n    type: self-custody\n    applies_to: registerAgent, createBond, prepareTask, prepareVKPAction — the API returns an unsigned transaction / contract ABI; state changes happen only when the caller signs and broadcasts with their own wallet\n    evidence: OpenAPI response descriptions (\"Unsigned transaction to submit on-chain\"); agent card authentication.note; Terms section 3 (self-custody)\n  - name: mcpPrivateKey\n    type: environment-secret\n    applies_to: the two write tools of the stdio MCP server (vaultfire_register_agent, vaultfire_create_bond)\n    variable: PRIVATE_KEY\n    evidence: '@vaultfire/mcp-server\
  \ README, \"Write Tools (require PRIVATE_KEY env var)\"'\n    note: A wallet private key held by the local process, never sent to Vaultfire.\ncredential_issuance: none — there is no sign-up, API key or OAuth client; identity is the caller's wallet address\nspec_gap: >-\n  The contract declares no securitySchemes at all, so the ERC-8128 requirement on routeTask and the x402\n  requirement on the priced surface are invisible to a generated client. Captured in\n  overlays/theloopbreaker-com-openapi-overlay.yaml.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/theloopbreaker-com/refs/heads/main/authentication/theloopbreaker-com-authentication.yml
summary_line: none/erc-8128-http-signature/x402-payment/wallet-signature · 5 schemes
tags:
- AI Agents
- Agent Identity
- Trust
- Reputation
- Blockchain
- Web3
- Payments
- x402
- MCP
- A2A
- Company
---
