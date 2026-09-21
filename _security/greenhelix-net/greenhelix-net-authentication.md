---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: greenhelix-net-a2a-commerce-gateway-openapi.yml
  format: yaml
  label: A2A Commerce Gateway API
  slug: a2a-commerce-gateway-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/greenhelix-net/refs/heads/main/openapi/greenhelix-net-a2a-commerce-gateway-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Greenhelix Net Authentication
name_suffix: Authentication
oauth_flows: []
overview: Green Helix secures its APIs with apiKey and http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Green Helix
provider_slug: greenhelix-net
scheme_count: 3
schemes:
- description: API key passed as Bearer token in the Authorization header.
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/greenhelix-net-a2a-commerce-gateway-openapi.yml
  type: http
- description: API key passed directly in the X-API-Key header (alternative to Bearer).
  in: header
  name: ApiKeyAuth
  parameter: X-API-Key
  sources:
  - openapi/greenhelix-net-a2a-commerce-gateway-openapi.yml
  type: apiKey
- description: x402 payment proof for stateless authentication.
  in: header
  name: X402Payment
  parameter: X-PAYMENT
  sources:
  - openapi/greenhelix-net-a2a-commerce-gateway-openapi.yml
  type: apiKey
slug: greenhelix-net-authentication
source_filename: greenhelix-net-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: searched\nsource: openapi/greenhelix-net-a2a-commerce-gateway-openapi.yml (three securitySchemes) upgraded from https://www.greenhelix.net/docs.html#authentication,\n  https://github.com/mirni/a2a/blob/main/docs/api-reference.md#1-authentication and https://github.com/mirni/a2a/blob/main/docs/adr/009-auth-rate-limiting.md;\n  401 shapes observed live 2026-09-19\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\n  style: Opaque per-agent API key with the tier embedded in the prefix; no OAuth, no OIDC, no JWT (ADR-009). x402\n    payment proof accepted as a stateless alternative when enabled.\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: API key passed as Bearer token in the Authorization header.\n  sources:\n  - openapi/greenhelix-net-a2a-commerce-gateway-openapi.yml\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: API key passed directly in the X-API-Key\
  \ header (alternative to Bearer).\n  sources:\n  - openapi/greenhelix-net-a2a-commerce-gateway-openapi.yml\n- name: X402Payment\n  type: apiKey\n  in: header\n  parameter: X-PAYMENT\n  description: x402 payment proof for stateless authentication.\n  sources:\n  - openapi/greenhelix-net-a2a-commerce-gateway-openapi.yml\ndocs:\n- https://www.greenhelix.net/docs.html\n- https://github.com/mirni/a2a/blob/main/docs/api-reference.md#1-authentication\n- https://github.com/mirni/a2a/blob/main/docs/adr/009-auth-rate-limiting.md\napi_key:\n  format: 'a2a_{tier}_{24_hex_chars}  (tiers: free, starter, pro, enterprise; e.g. a2a_free_… )'\n  issuance: 'Self-service: POST /v1/register {\"agent_id\"} (no auth) creates a wallet, a free-tier key and an identity\n    in one step; POST /v1/billing/keys (create_billing_api_key) issues further keys; POST /v1/infra/keys is the\n    deprecated older route.'\n  storage: Plaintext returned exactly once at creation; stored server-side as a SHA-3-256 hash (api-reference)\
  \ /\n    SHA-256 (ADR-009).\n  rotation: POST /v1/infra/keys/rotate {current_key} with optional X-Rotate-Confirmation header (revoke old, issue\n    new at the same tier); POST /v1/infra/keys/revoke.\n  header_precedence:\n  - 'Authorization: Bearer <key> (preferred)'\n  - 'X-API-Key: <key>'\n  scoping: Tier-scoped (free 100/h … enterprise 100000/h); a key can act only for its own agent_id — 403 forbidden\n    when creating keys for another agent.\nx402:\n  header: X-PAYMENT\n  encoding: base64-encoded JSON payment proof\n  when: when no API key is provided and x402 payment verification is enabled on the gateway\n  settlement: on-chain USDC micropayments\n  errors:\n    402 payment_required: no key and x402 enabled\n    402 payment_verification_failed: proof invalid\n    402 payment_replay_detected: nonce already used\n  note: Declared as securitySchemes.X402Payment and applied globally; not exercised live in this pass (unauthenticated\n    calls answered 401 missing-key, no 402 challenge\
  \ observed).\nobserved:\n- request: GET https://api.greenhelix.net/v1/billing/wallets/example-agent/balance (no credentials)\n  status: 401\n  content_type: application/problem+json\n  body:\n    type: https://api.greenhelix.net/errors/missing-key\n    title: Unauthorized\n    detail: Missing API key\n  www_authenticate: null\n- request: 'same, Authorization: Bearer a2a_free_<unknown>'\n  status: 401\n  body:\n    type: https://api.greenhelix.net/errors/authentication-error\n    title: Unauthorized\n    detail: API key not found\n- request: GET https://api.greenhelix.net/v1/metrics\n  status: 403\n  body:\n    type: https://api.greenhelix.net/errors/forbidden\n    detail: Metrics requires enterprise tier or allowed IP\npublic_endpoints:\n- GET /v1/health, /livez, /readyz\n- GET /v1/pricing, /v1/pricing/{tool}, /v1/pricing/summary, /v1/pricing/tiers\n- GET /v1/openapi.json, /v1/onboarding, /docs, /redoc\n- GET /.well-known/agent-card.json, /.well-known/ai-plugin.json\n- POST /v1/register\n\
  oauth:\n  supported: false\n  note: No oauth2/openIdConnect scheme; /.well-known/oauth-authorization-server, oauth-protected-resource and openid-configuration\n    all 404 on api, sandbox and www hosts. No scopes artifact is written.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/greenhelix-net/refs/heads/main/authentication/greenhelix-net-authentication.yml
summary_line: apiKey/http · 3 schemes
tags:
- Agents
- Agentic Commerce
- Payments
- Escrow
- Billing
- Marketplace
- Identity
- Trust
- Messaging
- Webhook
- MCP
- A2A
- x402
---
