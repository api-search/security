---
anonymous_access: true
api_key_in: []
api_specs:
- filename: dynamicfeed-ai-openapi.yml
  format: yaml
  label: Dynamic Feed REST API
  slug: dynamic-feed-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dynamicfeed-ai/refs/heads/main/openapi/dynamicfeed-ai-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Dynamicfeed Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Dynamic Feed declares 4 security scheme(s) across its OpenAPI definitions.
provider_name: Dynamic Feed
provider_slug: dynamicfeed-ai
scheme_count: 4
schemes:
- applies_to:
  - https://dynamicfeed.ai/mcp (all 94 tools)
  - https://dynamicfeed.ai/sse
  - POST /v1/batch
  - POST /v1/awareness, /v1/preflight, /v1/road, /v1/humanoid, /v1/marine
  - POST /v1/anchor, /v1/guard, /v1/drift; GET/POST /v1/explain; GET /v1/sources, /v1/snapshot, /v1/stream, /v1/discover, /v1/bundles, /v1/facts
  - GET /v1/notary/log*, /v1/checkpoints*, /v1/witness/sample and the other */sample routes
  - GET /.well-known/keys, /.well-known/signing-key-registry.json
  id: keyless
  policy: fair-use; "No per-key quota; subject to service availability" (MCP), max 20 calls per batch request
  type: none
  verified: probed — anonymous MCP tools/list and POST /v1/batch both returned 200 on 2026-09-19
- applies_to:
  - GET /v1/me
  - GET/POST/DELETE /v1/watchlist
  - GET/POST/DELETE /v1/webhooks, POST /v1/webhooks/test
  - POST /v1/witness, /v1/inference-receipt, /v1/robot-receipt, /v1/eval-receipt, /v1/proxy-witness, /v1/station/register, /v1/station/reading
  - GET /status, /whats-new and the direct per-feed GET routes (/earthquakes, /weather, /models …)
  - GET /v1/asof (paid key only; free key gets a 402 upgrade pointer)
  failure:
    body: '{"detail":"Missing API key. Get a free one at POST /signup, then send it as the ''X-API-Key'' header."}'
    observed: GET https://dynamicfeed.ai/status and GET /earthquakes on 2026-09-19
    status: 401
  id: api-key
  in: header
  introspection: GET /v1/me -> plan, calls used today, daily quota, remaining
  issuance:
    body: '{"email": "<optional, for receipts>"}'
    cost: free, no card
    endpoint: POST https://dynamicfeed.ai/signup
    human_ui: https://dynamicfeed.ai/dashboard (stores the key in browser localStorage)
    operation: signup_signup_post
    returns: api_key
  key_prefix_observed: amd_ (dashboard placeholder)
  name: X-API-Key
  optional_on_mcp: Sending the key on MCP calls only attributes usage; the default is keyless.
  rotation: No revoke/rotate operation published; the Terms reserve the provider's right to revoke.
  type: apiKey
  verified: probed (401 shape) + searched
- applies_to:
  - POST /v1/pro/batch
  - POST /v1/pro/tool/{tool}
  - POST /v1/pro/asof
  asset: USDC 0x833589fCD6eDb6E08f4c7C32D4f71b54bdA02913
  challenge:
    body: x402Version, error, accepts[] {scheme exact, network, maxAmountRequired, resource, payTo, asset, maxTimeoutSeconds 120, outputSchema}, extensions.bazaar
    observed: POST https://dynamicfeed.ai/v1/pro/tool/current_time on 2026-09-19
    status: 402
  docs: https://dynamicfeed.ai/x402
  facilitators:
  - https://api.cdp.coinbase.com/platform/v2/x402
  - https://facilitator.payai.network
  - https://facilitator.mogami.tech
  - https://dexter.cash/facilitator
  header: X-PAYMENT (request) / X-PAYMENT-RESPONSE (settlement proof on the response)
  id: x402
  network: base
  pay_to: '0xb525F2c54Ae0c3B3466206694726f85C7Cf7b985'
  price: 0.001 USDC per call
  protocol: x402 (x402Version 1)
  type: payment
  verified: probed (402 quote); no payment was made
- applies_to: the same 60 keyed operations, when called through the RapidAPI marketplace listing
  id: rapidapi-proxy
  in: header
  name: x-rapidapi-proxy-secret / x-rapidapi-user
  note: Declared as optional header parameters in the OpenAPI; the marketplace injects them. Not a credential a direct caller uses.
  type: apiKey
  verified: derived from the contract
slug: dynamicfeed-ai-authentication
source_filename: dynamicfeed-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: searched\nsource: https://dynamicfeed.ai/docs and /connect (access-policy table), https://dynamicfeed.ai/llms.txt, https://dynamicfeed.ai/v1\n  (keyless flags per route), https://dynamicfeed.ai/dashboard, live 401/402 responses observed 2026-09-19; openapi/_original/dynamicfeed-ai-openapi.json\n  declares NO securitySchemes (derive-authentication.py found nothing to derive), so this profile is searched, not\n  derived.\ndocs: https://dynamicfeed.ai/docs\nsummary: 'Three access modes on one host, none of them OAuth: (1) keyless — the MCP endpoint, POST /v1/batch and\n  the /v1 robot/ground-truth/notary/anchor routes need no credential at all; (2) a static X-API-Key header, issued\n  instantly by POST /signup with no card, required for per-user state (watchlist, webhooks, /v1/me), the direct\n  per-feed GET routes and /status; (3) x402 payment — /v1/pro/* return HTTP 402 with a USDC-on-Base quote and are\n  unlocked by an X-PAYMENT header from\
  \ an x402 client, no account. The OpenAPI models the key as an optional `x-api-key`\n  header parameter on 60 operations (alongside x-rapidapi-proxy-secret / x-rapidapi-user for the RapidAPI marketplace\n  channel) rather than as a securityScheme.'\nschemes:\n- id: keyless\n  type: none\n  applies_to:\n  - https://dynamicfeed.ai/mcp (all 94 tools)\n  - https://dynamicfeed.ai/sse\n  - POST /v1/batch\n  - POST /v1/awareness, /v1/preflight, /v1/road, /v1/humanoid, /v1/marine\n  - POST /v1/anchor, /v1/guard, /v1/drift; GET/POST /v1/explain; GET /v1/sources, /v1/snapshot, /v1/stream, /v1/discover,\n    /v1/bundles, /v1/facts\n  - GET /v1/notary/log*, /v1/checkpoints*, /v1/witness/sample and the other */sample routes\n  - GET /.well-known/keys, /.well-known/signing-key-registry.json\n  policy: fair-use; \"No per-key quota; subject to service availability\" (MCP), max 20 calls per batch request\n  verified: probed — anonymous MCP tools/list and POST /v1/batch both returned 200 on 2026-09-19\n\
  - id: api-key\n  type: apiKey\n  in: header\n  name: X-API-Key\n  issuance:\n    operation: signup_signup_post\n    endpoint: POST https://dynamicfeed.ai/signup\n    body: '{\"email\": \"<optional, for receipts>\"}'\n    returns: api_key\n    cost: free, no card\n    human_ui: https://dynamicfeed.ai/dashboard (stores the key in browser localStorage)\n  key_prefix_observed: amd_ (dashboard placeholder)\n  introspection: GET /v1/me -> plan, calls used today, daily quota, remaining\n  applies_to:\n  - GET /v1/me\n  - GET/POST/DELETE /v1/watchlist\n  - GET/POST/DELETE /v1/webhooks, POST /v1/webhooks/test\n  - POST /v1/witness, /v1/inference-receipt, /v1/robot-receipt, /v1/eval-receipt, /v1/proxy-witness, /v1/station/register,\n    /v1/station/reading\n  - GET /status, /whats-new and the direct per-feed GET routes (/earthquakes, /weather, /models …)\n  - GET /v1/asof (paid key only; free key gets a 402 upgrade pointer)\n  failure:\n    status: 401\n    body: '{\"detail\":\"Missing API key.\
  \ Get a free one at POST /signup, then send it as the ''X-API-Key'' header.\"}'\n    observed: GET https://dynamicfeed.ai/status and GET /earthquakes on 2026-09-19\n  optional_on_mcp: Sending the key on MCP calls only attributes usage; the default is keyless.\n  rotation: No revoke/rotate operation published; the Terms reserve the provider's right to revoke.\n  verified: probed (401 shape) + searched\n- id: x402\n  type: payment\n  protocol: x402 (x402Version 1)\n  header: X-PAYMENT (request) / X-PAYMENT-RESPONSE (settlement proof on the response)\n  network: base\n  asset: USDC 0x833589fCD6eDb6E08f4c7C32D4f71b54bdA02913\n  pay_to: '0xb525F2c54Ae0c3B3466206694726f85C7Cf7b985'\n  price: 0.001 USDC per call\n  applies_to:\n  - POST /v1/pro/batch\n  - POST /v1/pro/tool/{tool}\n  - POST /v1/pro/asof\n  challenge:\n    status: 402\n    body: x402Version, error, accepts[] {scheme exact, network, maxAmountRequired, resource, payTo, asset, maxTimeoutSeconds\n      120, outputSchema}, extensions.bazaar\n\
  \    observed: POST https://dynamicfeed.ai/v1/pro/tool/current_time on 2026-09-19\n  facilitators:\n  - https://api.cdp.coinbase.com/platform/v2/x402\n  - https://facilitator.payai.network\n  - https://facilitator.mogami.tech\n  - https://dexter.cash/facilitator\n  docs: https://dynamicfeed.ai/x402\n  verified: probed (402 quote); no payment was made\n- id: rapidapi-proxy\n  type: apiKey\n  in: header\n  name: x-rapidapi-proxy-secret / x-rapidapi-user\n  applies_to: the same 60 keyed operations, when called through the RapidAPI marketplace listing\n  note: Declared as optional header parameters in the OpenAPI; the marketplace injects them. Not a credential a\n    direct caller uses.\n  verified: derived from the contract\noauth2:\n  supported: false\n  evidence: /.well-known/oauth-authorization-server, /.well-known/oauth-protected-resource and /.well-known/openid-configuration\n    all return 404; no securitySchemes in the contract.\nresponse_signing:\n  note: 'Authentication of the SERVER\
  \ to the client is the stronger half of this profile: every response is Ed25519-signed\n    (DF-VERIFY/1) and the agent card carries a JWS. See conventions/dynamicfeed-ai-conventions.yml response_envelope\n    and json-schema/.'\ngaps:\n- No securitySchemes in the OpenAPI, so generated clients see every route as anonymous.\n- No key rotation or revocation endpoint.\n- No scoped or restricted keys; one key grants all per-user routes.\n- No OAuth/OIDC, so no delegated identity path for agents acting on behalf of a user.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dynamicfeed-ai/refs/heads/main/authentication/dynamicfeed-ai-authentication.yml
summary_line: 4 schemes
tags:
- Live Data
- AI Agents
- MCP
- A2A
- agent-native
- Provenance
- Weather
- Natural Hazards
- Vulnerabilities
- Sanctions
- Space
- Robotics
- x402
- Receipts
- Notary
- Australia
---
