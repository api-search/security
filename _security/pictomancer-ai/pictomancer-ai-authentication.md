---
anonymous_access: true
api_key_in: []
api_specs:
- filename: pictomancer-ai-openapi.yml
  format: yaml
  label: Pictomancer.ai Image API
  slug: pictomancer-ai-image-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pictomancer-ai/refs/heads/main/openapi/pictomancer-ai-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Pictomancer Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Pictomancer.ai declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: Pictomancer.ai
provider_slug: pictomancer-ai
scheme_count: 3
schemes:
- applies_to: REST, MCP, A2A
  identity: X-Agent-Wallet header (Ethereum address) or source IP
  name: anonymous
  quota: 50 free requests per identity; analyze and estimate always free
  type: none
- applies_to: REST, MCP, A2A
  cost_guard: 'Optional X-Max-Cost-USD request header: the API returns 412 instead of charging above the cap; POST /v1/estimate prices a request for free first.'
  currency: USDC
  flow: request -> 402 with price -> pay -> retry with X-Payment -> 200 (~2s settlement per homepage)
  header: X-Payment
  name: x402
  network: base
  protocol: x402 (https://x402.org)
  type: payment
- applies_to: REST, MCP, A2A, WordPress plugin (PICTOMANCER_API_KEY in wp-config.php)
  format: 'Authorization: Bearer <PICTOMANCER_API_KEY>'
  header: Authorization
  issued_at: https://app.pictomancer.ai (dashboard; create/revoke, usage tracking — changelog v0.3.0)
  name: apiKey
  scheme: bearer
  type: http
slug: pictomancer-ai-authentication
source_filename: pictomancer-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: searched\nsource: https://pictomancer.ai/llms.txt (Identity, Pricing, How to connect), https://pictomancer.ai/ (Code and For-agents sections), CORS Access-Control-Allow-Headers on api.pictomancer.ai (Authorization, Content-Type, X-Agent-Wallet, X-Payment), https://pictomancer.ai/.well-known/mcp.json (authentication.required false), agent card x402 extension\ndocs: https://api.pictomancer.ai/docs\nspec_gap: openapi/pictomancer-ai-openapi.yml declares NO securitySchemes and no security requirement; the credential styles below are documented in prose only (captured for the spec in overlays/pictomancer-ai-openapi-overlay.yaml).\nsummary: >-\n  Three ways in, all on the same endpoints. (1) Anonymous — the first 50 requests per identity are free with\n  no account; identity is the X-Agent-Wallet header (an Ethereum address) or, absent that, the caller IP.\n  (2) x402 pay-per-request — after the free tier the API answers 402 with a USDC price on Base;\
  \ the agent pays\n  and retries with X-Payment. No account or key involved. (3) API key — created in the dashboard\n  (app.pictomancer.ai; login is Google or GitHub OAuth) and sent as Authorization: Bearer; subscription\n  plans (Dev/Pro/Enterprise) and Stripe top-ups bill against it. The MCP server and A2A endpoint accept the\n  same identities; /.well-known/mcp.json states authentication.required: false.\nschemes:\n- name: anonymous\n  type: none\n  identity: X-Agent-Wallet header (Ethereum address) or source IP\n  quota: 50 free requests per identity; analyze and estimate always free\n  applies_to: REST, MCP, A2A\n- name: x402\n  type: payment\n  header: X-Payment\n  protocol: x402 (https://x402.org)\n  currency: USDC\n  network: base\n  flow: request -> 402 with price -> pay -> retry with X-Payment -> 200 (~2s settlement per homepage)\n  cost_guard: 'Optional X-Max-Cost-USD request header: the API returns 412 instead of charging above the cap; POST /v1/estimate prices a request for\
  \ free first.'\n  applies_to: REST, MCP, A2A\n- name: apiKey\n  type: http\n  scheme: bearer\n  header: Authorization\n  format: 'Authorization: Bearer <PICTOMANCER_API_KEY>'\n  issued_at: https://app.pictomancer.ai (dashboard; create/revoke, usage tracking — changelog v0.3.0)\n  applies_to: REST, MCP, A2A, WordPress plugin (PICTOMANCER_API_KEY in wp-config.php)\noauth:\n  api: false\n  dashboard_login: Google and GitHub OAuth (changelog v0.3.0) — sign-in only, no API scopes, no authorization-server metadata published\nkey_prefix: not published\nrotation: create and revoke keys in the dashboard; no rotation policy published\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pictomancer-ai/refs/heads/main/authentication/pictomancer-ai-authentication.yml
summary_line: 3 schemes
tags:
- Company
- Image
- Image Optimization
- Image Processing
- Media
- Agents
- MCP
- A2A
- x402
- Micropayments
- Developer Tools
---
