---
anonymous_access: false
api_key_in: []
api_specs:
- filename: agentum-lat-apis-brasil-openapi.json
  format: json
  label: AGENTUM APIs Brasil
  slug: apis-brasil
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agentum-lat/refs/heads/main/openapi/agentum-lat-apis-brasil-openapi.json
- filename: agentum-lat-business-openapi.json
  format: json
  label: AGENTUM Business API
  slug: business
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agentum-lat/refs/heads/main/openapi/agentum-lat-business-openapi.json
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 0
method: searched
name: Agentum Lat Authentication
name_suffix: Authentication
oauth_flows: []
overview: AGENTUM declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: AGENTUM
provider_slug: agentum-lat
scheme_count: 0
schemes: []
slug: agentum-lat-authentication
source_filename: agentum-lat-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: searched\nsource: https://agentum.lat/llms.txt\nadditional_docs:\n- https://agentum.lat/ (\"Sem conta, sem chave, sem assinatura: seu agente paga e recebe o resultado na mesma requisição\")\n- https://agentum.lat/openapi.json and https://business.agentum.lat/openapi.json (no securitySchemes, no security requirements; x-payment-info per operation)\n- https://github.com/orionlabsai/agentum-mcp-server (README + index.js — how the provider's own client authorises a call)\n- live 402 challenges on both hosts, 2026-09-19\nsummary:\n  types: []\n  http_schemes: []\n  api_key_in: []\n  oauth2_flows: []\n  credential_types: []\n  access_model: payment-gated, credential-less — x402 v2 per-request payment in USDC on Base mainnet stands in for authentication\n  public_operations: [GET https://business.agentum.lat/health, GET https://business.agentum.lat/ (service index), GET /openapi.json on both hosts, GET https://agentum.lat/llms.txt, GET /.well-known/agent-card.json\
  \ and /.well-known/security.txt]\n  discovery: none — no RFC 8414 authorization-server metadata, no RFC 9728 protected-resource metadata, no OpenID configuration on any host (well-known/agentum-lat-well-known.yml). The machine-readable access contract is the 402 challenge itself.\n  dynamic_client_registration: false\n  delegated_identity: false\n  consent_identity: false\nschemes: []\npayment_gate:\n  protocol: x402 v2\n  scheme: exact\n  network: eip155:8453\n  asset: USDC 0x833589fCD6eDb6E08f4c7C32D4f71b54bdA02913\n  challenge: HTTP 402 with PAYMENT-REQUIRED (base64 JSON PaymentRequirements) on every paid route; maxTimeoutSeconds 300\n  identity: the payer's on-chain address is the only identity the server sees; there is no account, session, key or token to issue, rotate or revoke\n  pay_to:\n    agentum_lat: '0xB4f9061e3a6A5533431336506b34e1035029599f'\n    business_agentum_lat: '0x7D1EDdfBd167787251fed83b250ABBeA1cf59a6F'\n  gate_order: the payment gate answers before input validation\
  \ — malformed identifiers (cnpj=123, q=) received a 402, not the contract's 400\n  reference_client: '@agentum/mcp-server holds the CALLER''s wallet private key in env AGENTUM_MCP_WALLET_KEY and signs with @x402/fetch; the provider never issues or holds a credential'\nagent_auth:\n  model: wallet-as-principal. An agent needs a funded Base wallet and an x402-capable client; nothing else. No scopes, no consent screen, no delegation — the wallet key IS full authority to spend, which the provider's README treats as the main risk (dedicated wallet, minimal balance, never commit the key).\n  human_in_the_loop: none at the protocol level; the provider's separate @agentum/x402-spend-guard library offers caller-side caps, allowlists and a kill switch\na2a_surface:\n  securitySchemes: >-\n    {} (empty) and securityRequirements [] in the agent card; the JSON-RPC root accepted an unauthenticated GetTask (answered -32001 TASK_NOT_FOUND). Whether paid skills are x402-gated over A2A was not observed.\n\
  notes:\n- 'No OAuthScopes artifact is emitted: there is no OAuth surface. scopes/ is intentionally absent.'\n- 'The derive-authentication.py pass produced no profile (0 securitySchemes across both specs), which is correct; this file was written by hand from the provider''s statements and the observed gate.'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/agentum-lat/refs/heads/main/authentication/agentum-lat-authentication.yml
summary_line: 0 schemes
tags:
- Company
- Business Intelligence
- KYB
- Company Data
- Compliance
- Brazil
- x402
- Agentic Commerce
- Exchange Rates
- Address Verification
- Economic Data
- MCP
- A2A
- Agents
---
