---
anonymous_access: false
api_key_in: []
api_specs:
- filename: muj428-com-trust-layer-openapi.json
  format: json
  label: MUJ428 Trust Layer API
  slug: muj428-trust-layer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/muj428-com/refs/heads/main/openapi/muj428-com-trust-layer-openapi.json
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 0
method: searched
name: Muj428 Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: MUJ428 LLC declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: MUJ428 LLC
provider_slug: muj428-com
scheme_count: 0
schemes: []
slug: muj428-com-authentication
source_filename: muj428-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: searched\nsource: openapi/muj428-com-trust-layer-openapi.json\ndocs:\n- https://agents.muj428.com/AGENTS.md\n- https://agents.muj428.com/developer.json\n- https://agents.muj428.com/index.md\nsummary:\n  types: []\n  api_key_in: []\n  oauth2_flows: []\n  bearer: false\n  credential_classes: 0\n  headline: >-\n    No credential of any kind on the read and free-preflight surface. Neither OpenAPI declares a securitySchemes\n    block or a security requirement (derive-authentication.py found nothing to extract), and the provider says\n    so in words: \"No card. No contract. No signup. No API key. No wallet commitment. No automatic charge.\"\n    (index.md); developer.json trust_reflex.auth_required_for_free_calls = false. The only gate on the surface\n    is ECONOMIC — x402 payment for the five paid services and for Trust Reflex after its free quota — plus one\n    narrowly scoped bearer token the monitoring endpoint mints. No OAuth, no OIDC, no\
  \ discovery documents on\n    any host.\nschemes: []\naccess_model:\n  free_tier:\n    what: POST /v1/trust (Trust Reflex), POST /v1/rescue, POST /v1/route, every GET, POST /v1/compatibility*, POST /v1/trust-requests, POST /v1/monitor\n    credential: none\n    identity: >-\n      A caller-chosen stable string, caller_ref (>=3 chars), used only for free-quota accounting (1,000 qualifying\n      decisions per caller_ref); action_ref is the per-action replay key. No registration binds caller_ref to anyone.\n    source: OpenAPI TrustAction schema; AGENTS.md \"Usage\"\n  paid_tier:\n    what: POST /v1/evidence-signal, /v1/reputation-check, /v1/milestone-attestation, /v1/trust-layer-report, /v1/transaction-assurance (also under /functions/v1/trust-layer-x402/), and /v1/trust after the free quota\n    credential: PAYMENT-SIGNATURE request header (x402 v2), caller-supplied\n    flow:\n    - POST the request without PAYMENT-SIGNATURE\n    - receive HTTP 402 and a PAYMENT-REQUIRED header naming\
  \ exact amount, network (eip155:8453), asset (USDC) and seller\n    - the caller independently authorizes payment under its own wallet/policy — MUJ428 never fabricates or sends a signature\n    - retry the same request with a valid PAYMENT-SIGNATURE\n    - MUJ428 verifies, reserves, settles, fulfils and returns 200 plus PAYMENT-RESPONSE\n    source: https://agents.muj428.com/developer.json x402_flow; OpenAPI /v1/trust description\n    note: This is payment, not authentication — it proves the caller paid, not who the caller is.\n  monitor_token:\n    what: POST /v1/monitor (201) \"response includes a one-time bearer monitor token\"\n    credential: bearer token returned by the create call, scoped to that monitor\n    source: OpenAPI /v1/monitor 201 description\n    note: The only bearer credential on the surface; its later use (state/observation updates) is not described in the public spec.\n  a2a:\n    what: JSON-RPC at https://agents.muj428.com/a2a\n    credential: none, but the A2A-Extensions\
  \ header MUST name https://agents.muj428.com/extensions/trust-reflex/v1 or the endpoint answers -32600\n    source: live probe 2026-09-19; extension descriptor activation block\n  mcp:\n    what: both MCP endpoints\n    credential: none for initialize / tools/list / free tools; paid tool calls carry payment_signature as a tool argument\n    source: live tools/list 2026-09-19; invoke_trust_service inputSchema\ngateway_headers_observed:\n  note: >-\n    The Supabase gateway's CORS allow-list names authorization, apikey and x-client-info — standard Supabase edge-function\n    headers — alongside payment-signature, x-request-id, idempotency-key and muj428-observer-ref. None of authorization /\n    apikey is required by any documented MUJ428 operation; do not read the allow-list as an auth scheme.\nsecrets_policy:\n  source: https://agents.muj428.com/.well-known/agent-permissions.json\n  rule: 'MUST NOT send private keys, seed phrases, payment credentials, or other secrets to MUJ428.'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/muj428-com/refs/heads/main/authentication/muj428-com-authentication.yml
summary_line: 0 schemes
tags:
- Agents
- Agent Trust
- Agentic Commerce
- A2A
- MCP
- x402
- Payments
- Risk
- Verification
- agent-native
---
