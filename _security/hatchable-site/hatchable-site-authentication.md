---
anonymous_access: false
api_key_in: []
api_specs:
- filename: hatchable-site-openapi.yml
  format: yaml
  label: IntentGuard Router API
  slug: intentguard-router-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hatchable-site/refs/heads/main/openapi/hatchable-site-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Hatchable Site Authentication
name_suffix: Authentication
oauth_flows: []
overview: IntentGuard declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: IntentGuard
provider_slug: hatchable-site
scheme_count: 1
schemes:
- amount_per_call: 0.0009 USDC (900 base units)
  applies_to:
  - routeTask
  - checkImageIntent
  - MCP tools/call
  asset: 0x833589fCD6eDb6E08f4c7C32D4f71b54bdA02913 (USDC on Base)
  description: Modeled as an apiKey-in-header scheme because that is the closest OpenAPI primitive; it is not a static credential - the header value is a signed, single-use, amount-bound payment authorization. The OpenAPI declares no securitySchemes at all; overlays/hatchable-site-openapi-overlay.yaml adds this one.
  evidence:
    error_string: PAYMENT-SIGNATURE header is required
    status: 402
    url: https://intentguard.hatchable.site/api/route
  facilitator: https://facilitator.payai.network
  id: x402
  in: header
  max_timeout_seconds: 60
  name: PAYMENT-SIGNATURE
  network: eip155:8453
  pay_to: '0xcd461ac1783b22c4610d1d34f8fb01063532cb9e'
  protocol: x402 v2
  type: apiKey
slug: hatchable-site-authentication
source_filename: hatchable-site-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: searched\nsource: >-\n  https://intentguard.hatchable.site/llms.txt, https://intentguard.hatchable.site/skill.md,\n  well-known/hatchable-site-ai-plugin.json (auth type none), well-known/hatchable-site-x402-service.json,\n  openapi/hatchable-site-openapi.yml (x-payment-info, no securitySchemes), and live 402 challenges observed at\n  POST /api/route and POST /api/intent-check on 2026-09-19\ndocs: https://intentguard.hatchable.site/llms.txt\nmodel: payment-as-authorization\naccounts: false\napi_keys: false\noauth: false\nsummary: >-\n  There is no account, no registration, no API key and no bearer token anywhere on this surface - the homepage\n  says \"no account\" and ai-plugin.json declares auth type none. Authorization IS payment on the two paid\n  operations: a request without a signed payment gets HTTP 402 with an x402 v2 challenge carrying one accepts[]\n  entry (USDC on Base, 0.0009 per call, 60-second authorization timeout); the caller\
  \ signs an EIP-3009\n  transferWithAuthorization for it and retries the identical request with the signed payload in a\n  PAYMENT-SIGNATURE header, settled through the facilitator at https://facilitator.payai.network. The free\n  preview, the MCP initialize/tools/list methods, the A2A discovery door and every discovery document need\n  nothing at all.\nschemes:\n- id: x402\n  type: apiKey\n  in: header\n  name: PAYMENT-SIGNATURE\n  protocol: x402 v2\n  applies_to: [routeTask, checkImageIntent, MCP tools/call]\n  network: eip155:8453\n  asset: 0x833589fCD6eDb6E08f4c7C32D4f71b54bdA02913 (USDC on Base)\n  pay_to: '0xcd461ac1783b22c4610d1d34f8fb01063532cb9e'\n  amount_per_call: 0.0009 USDC (900 base units)\n  max_timeout_seconds: 60\n  facilitator: https://facilitator.payai.network\n  description: >-\n    Modeled as an apiKey-in-header scheme because that is the closest OpenAPI primitive; it is not a static\n    credential - the header value is a signed, single-use, amount-bound payment authorization.\
  \ The OpenAPI\n    declares no securitySchemes at all; overlays/hatchable-site-openapi-overlay.yaml adds this one.\n  evidence:\n    url: https://intentguard.hatchable.site/api/route\n    status: 402\n    error_string: PAYMENT-SIGNATURE header is required\nopen_surfaces:\n- POST /api/router-preview (previewModelRoute)\n- POST /api/mcp - initialize, tools/list\n- POST /api/a2a - message/send answers with a discovery message\n- GET /openapi.json, /mcp.json, /llms.txt, /skill.md, /router-catalog.json, /.well-known/*\nplatform_note: >-\n  The hosting platform's OAuth 2.1 metadata at https://hatchable.com/.well-known/oauth-authorization-server\n  (issuer hatchable.com, scopes_supported [mcp], resource https://hatchable.com/mcp) governs Hatchable's OWN\n  platform MCP server for building apps and has no bearing on this operator's API; it is recorded here only so\n  a later pass does not mistake it for IntentGuard's auth.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hatchable-site/refs/heads/main/authentication/hatchable-site-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Artificial Intelligence
- Agents
- Model Routing
- Cost Optimization
- x402
- MCP
- A2A
- pay-per-call
- Prompt Optimization
- Agentic Payments
---
