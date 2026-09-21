---
anonymous_access: true
api_key_in:
- header
auth_types:
- none
- x402-payment
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: probed
name: Grokandmon Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: Grok & Mon secures its APIs with none, x402-payment, and apiKey across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Grok & Mon
provider_slug: grokandmon-com
scheme_count: 3
schemes:
- applies_to:
  - MCP initialize, tools/list, tools/call
  - GET /a2a/v1
  - GET /a2a/v1/acp/grow, /acp/signals, /acp/oracle
  - POST /a2a/v1 tasks/get and agent/info
  name: anonymous
  observed: HTTP 200 with no credential and no WWW-Authenticate on every call made in this pass (2026-09-19).
  type: none
- also_allowed_by_cors:
  - X-Payment
  - X-402-Payment
  - X-Payment-Address
  - X-Payment-Amount
  - X-Payment-Token
  - X-Payment-Network
  format: EIP-3009 transferWithAuthorization signature for a USDC transfer (CAIP-10 payTo eip155:10143:0x734B0e337bfa7d4764f4B806B4245Dd312DdF134; Base eip155:8453 also listed)
  in: header
  name: x402
  parameter: PAYMENT-SIGNATURE
  purpose: Pay per A2A request (default $0.001 USDC; per-skill prices in the pricing document) beyond the 100/day free tier; unlocks "priority access".
  scoped: false
  sources:
  - a2a/grokandmon-com-agent-card.json
  - well-known/grokandmon-com-x402-pricing.json
  - https://grokandmon.com/a2a.html
  type: x402-payment
  verified: declared-only - no HTTP 402 challenge was observed; message/send was not exercised
- in: header
  issued_at: not published
  name: apiKey
  parameter: Authorization
  purpose: 'Declared only on the legacy /.well-known/agent.json card (securitySchemes.apiKey, security [{apiKey: []}]); absent from the canonical card; no issuance page exists.'
  scoped: false
  sources:
  - a2a/grokandmon-com-agent-card-legacy.json
  type: apiKey
slug: grokandmon-com-authentication
source_filename: grokandmon-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: probed\nsource:\n- https://grokandmon.com/.well-known/agent-card.json\n- https://grokandmon.com/.well-known/agent.json\n- https://grokandmon.com/mcp/v1\n- https://grokandmon.com/a2a/v1\ndocs: https://grokandmon.com/a2a.html\nsummary:\n  types:\n  - none\n  - x402-payment\n  - apiKey\n  api_key_in:\n  - header\n  oauth2_flows: []\n  note: >-\n    There is no OpenAPI to derive from; this profile is read from the provider's own served documents and\n    observed responses. The canonical agent card declares NO securitySchemes: the gate on the A2A surface\n    is payment, not identity - an x402 micropayment (EIP-3009 USDC transferWithAuthorization) carried in a\n    PAYMENT-SIGNATURE header per a2a.html, with a 100-requests/day free tier per the pricing document. The\n    MCP surface needed no credential for initialize, tools/list or tools/call and issued no session id. The\n    legacy card at /.well-known/agent.json declares an apiKey scheme in\
  \ the Authorization header, but no\n    page says how such a key is issued and the canonical card dropped it. No OAuth or OIDC discovery\n    document is served.\nschemes:\n- name: anonymous\n  type: none\n  applies_to: ['MCP initialize, tools/list, tools/call', 'GET /a2a/v1', 'GET /a2a/v1/acp/grow, /acp/signals, /acp/oracle', 'POST /a2a/v1 tasks/get and agent/info']\n  observed: 'HTTP 200 with no credential and no WWW-Authenticate on every call made in this pass (2026-09-19).'\n- name: x402\n  type: x402-payment\n  in: header\n  parameter: PAYMENT-SIGNATURE\n  also_allowed_by_cors: [X-Payment, X-402-Payment, X-Payment-Address, X-Payment-Amount, X-Payment-Token, X-Payment-Network]\n  format: EIP-3009 transferWithAuthorization signature for a USDC transfer (CAIP-10 payTo eip155:10143:0x734B0e337bfa7d4764f4B806B4245Dd312DdF134; Base eip155:8453 also listed)\n  purpose: Pay per A2A request (default $0.001 USDC; per-skill prices in the pricing document) beyond the 100/day free tier; unlocks\
  \ \"priority access\".\n  scoped: false\n  verified: declared-only - no HTTP 402 challenge was observed; message/send was not exercised\n  sources: [a2a/grokandmon-com-agent-card.json, well-known/grokandmon-com-x402-pricing.json, 'https://grokandmon.com/a2a.html']\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: Authorization\n  purpose: 'Declared only on the legacy /.well-known/agent.json card (securitySchemes.apiKey, security [{apiKey: []}]); absent from the canonical card; no issuance page exists.'\n  issued_at: not published\n  scoped: false\n  sources: [a2a/grokandmon-com-agent-card-legacy.json]\ndiscovery:\n  oauth_authorization_server: {url: 'https://grokandmon.com/.well-known/oauth-authorization-server', status: 200, real_document: false, result: spa-shell}\n  oauth_protected_resource: {url: 'https://grokandmon.com/.well-known/oauth-protected-resource', status: 200, real_document: false, result: spa-shell}\n  openid_configuration: {url: 'https://grokandmon.com/.well-known/openid-configuration',\
  \ status: 200, real_document: false, result: spa-shell}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/grokandmon-com/refs/heads/main/authentication/grokandmon-com-authentication.yml
summary_line: none/x402-payment/apiKey · 3 schemes
tags:
- AI Agents
- A2A
- MCP
- x402
- Agentic Commerce
- Cannabis
- IoT
- Cryptocurrency
- Monad
- Trading Signals
- Generative Art
---
