---
anonymous_access: false
api_key_in: []
api_specs:
- filename: openapi.json
  format: json
  label: DELTA Witness API
  slug: delta-witness-api
  spec_type: OpenAPI
  url: https://delta-witness-api.ruphussten.workers.dev/openapi.json
- filename: delta-witness-partner-gateway-openapi.json
  format: json
  label: DELTA Witness Partner Gateway
  slug: delta-witness-partner-gateway
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/delta-witness/refs/heads/main/openapi/delta-witness-partner-gateway-openapi.json
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Delta Witness Authentication
name_suffix: Authentication
oauth_flows: []
overview: DELTA Witness — Trust Layer for Autonomous Actions declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: DELTA Witness — Trust Layer for Autonomous Actions
provider_slug: delta-witness
scheme_count: 2
schemes:
- applies_to:
  - POST /v1/capture
  - POST /v1/preflight
  - POST /v1/guarded-action-pilot
  asset: USDC (0x833589fCD6eDb6E08f4c7C32d4f71b54bdA02913)
  facilitator: https://facilitator.payai.network
  id: x402-payment
  location: HTTP 402 challenge + payment-required header
  network: eip155:8453
  note: 'Not a classic securityScheme. The paid operations declare security: [] in OpenAPI and enforce payment at runtime via the x402 402 flow.'
  protocol: x402-v2
  recipient: '0x1990e21bc219696ff7fbc26527dbaed335ac6367'
  type: payment
- applies_to:
  - partner gateway /capture, /preflight, /watch
  host: delta-witness-partner-gateway.ruphussten.workers.dev
  id: PartnerProxySecret
  in: header
  name: x-delta-partner-secret
  note: Provider-managed reseller secret; must not be exposed to marketplace end users. Used only on the authenticated partner rail (not the public API).
  type: apiKey
slug: delta-witness-authentication
source_filename: delta-witness-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-11'\nmethod: searched\nsource: >-\n  openapi/delta-witness-openapi.json (security: [] on all operations),\n  the /.well-known/x402 discovery document, observed 402 challenges, and\n  openapi/delta-witness-partner-gateway-openapi.json.\nsummary: >-\n  The public DELTA Witness API declares no traditional authentication. Access to\n  billable operations is gated by machine payment (x402 v2) rather than by an API\n  key or OAuth token. Free operations (/health, /v1/quote, /v1/demo,\n  /v1/proofs/{id}) are open. The separate partner gateway uses an apiKey secret.\nschemes:\n  - id: x402-payment\n    type: payment\n    protocol: x402-v2\n    location: HTTP 402 challenge + payment-required header\n    network: eip155:8453\n    asset: USDC (0x833589fCD6eDb6E08f4c7C32d4f71b54bdA02913)\n    recipient: '0x1990e21bc219696ff7fbc26527dbaed335ac6367'\n    facilitator: https://facilitator.payai.network\n    applies_to:\n      - POST /v1/capture\n      - POST /v1/preflight\n\
  \      - POST /v1/guarded-action-pilot\n    note: >-\n      Not a classic securityScheme. The paid operations declare security: [] in\n      OpenAPI and enforce payment at runtime via the x402 402 flow.\n  - id: PartnerProxySecret\n    type: apiKey\n    in: header\n    name: x-delta-partner-secret\n    applies_to:\n      - partner gateway /capture, /preflight, /watch\n    host: delta-witness-partner-gateway.ruphussten.workers.dev\n    note: >-\n      Provider-managed reseller secret; must not be exposed to marketplace end\n      users. Used only on the authenticated partner rail (not the public API).\nopen_operations:\n  - GET /health\n  - GET /v1/quote\n  - GET /v1/demo\n  - GET /v1/proofs/{proof_id}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/delta-witness/refs/heads/main/authentication/delta-witness-authentication.yml
summary_line: 2 schemes
tags:
- web-verification
- proof-of-observation
- page-state-monitoring
- content-hashing
- agent-guardrails
- preflight-checks
- x402-payments
- pay-per-use
- base-usdc
- autonomous-agents
- mcp
- a2a
- agent-skill
- trust-and-safety
---
