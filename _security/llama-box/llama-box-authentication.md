---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: llama-box-crvusd-yield-optimizer-openapi.yml
  format: yaml
  label: crvUSD Yield Optimizer API
  slug: crvusd-yield-optimizer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/llama-box/refs/heads/main/openapi/llama-box-crvusd-yield-optimizer-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Llama Box Authentication
name_suffix: Authentication
oauth_flows: []
overview: Chado Studio secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Chado Studio
provider_slug: llama-box
scheme_count: 2
schemes:
- declared_as: 'An optional header PARAMETER (anyOf string|null, required: false) on each operation — not a securityScheme. A generator reading securitySchemes sees an unauthenticated API.'
  in: header
  issuance: Not published. The simulate_rebalance description says "Requires pro or enterprise tier"; /yo/api/pricing lists per-request x402 prices and the contact api@chado.studio but no tier, signup or key-issuance page.
  name: X-API-Key (undeclared)
  observed:
  - body: '{"detail":"Invalid API key"}'
    fetched: '2026-09-19'
    request: 'GET https://llama.box/yo/api/best-yield?top=1 with X-API-Key: invalid-probe'
    status: 401
  - fetched: '2026-09-19'
    note: free operation
    request: GET https://llama.box/yo/api/best-yield?top=1 with no key
    status: 200
  - body: '{}'
    fetched: '2026-09-19'
    note: paid operation — x402 challenge in the PAYMENT-REQUIRED header
    request: POST https://llama.box/yo/api/rebalance with no key
    status: 402
  parameter: X-API-Key
  sources:
  - openapi/llama-box-crvusd-yield-optimizer-openapi.yml
  type: apiKey
  used_by:
  - list_pools_api_pools_get
  - best_yield_api_best_yield_get
  - risk_score_api_risk_score__pool_id__get
  - simulate_rebalance_api_rebalance_post
  - a2a_endpoint_a2a_post
  - a2a_stream_endpoint_a2a_stream_post
- applies_to:
  - operation: risk_score_api_risk_score__pool_id__get
    price: $0.005
  - operation: simulate_rebalance_api_rebalance_post
    price: $0.01
  - operation: a2a_endpoint_a2a_post
    price: $0.01
  - operation: a2a_stream_endpoint_a2a_stream_post
    price: $0.01
  description: 'Per /yo/api/pricing: "1. Request any paid endpoint without payment -> get 402 with payment details. 2. Sign a USDC payment on Base using the returned parameters. 3. Resend request with X-PAYMENT header -> get 200 with data." The observed challenge is x402Version 2, scheme "exact", network eip155:84532 (Base Sepolia testnet), asset 0x036CbD53842c5426634e7929541eC2318f3dCF7e (extra.name USDC, extra.version 2), payTo 0x6a1175D0EA0e6817786Ce51F1C4F3294F907f410, maxTimeoutSeconds 300, amount 10000 base units ($0.01) for POST /a2a.'
  free_operations:
  - health_health_get
  - list_pools_api_pools_get
  - best_yield_api_best_yield_get
  - pricing_api_pricing_get
  - agent_card__well_known_agent_json_get
  - access_log_api_access_log_get
  in: header
  name: x402 payment
  note: Not a securityScheme in the OpenAPI and not declared in the agent card. The paid operations declare only 200 and 422 responses; the 402 is undocumented in the contract and discoverable only by calling.
  parameter: X-PAYMENT (request) / PAYMENT-REQUIRED (challenge response)
  sources:
  - https://llama.box/yo/api/pricing
  - a2a/llama-box-a2a.yml (x-evidence: decoded PAYMENT-REQUIRED header)
  standard: x402 v2 (HTTP 402 Payment Required)
  type: payment
slug: llama-box-authentication
source_filename: llama-box-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: searched\nsource: openapi/llama-box-crvusd-yield-optimizer-openapi.yml\ndocs:\n- https://llama.box/yo/docs\n- https://llama.box/yo/api/pricing\nprobed: true\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  oauth2_flows: []\n  bearer: false\n  security_schemes_declared: 0\n  headline: >-\n    The contract declares NO components.securitySchemes and no security[] requirement — derive-authentication.py\n    found nothing to profile — yet six of its ten operations accept an optional X-API-Key header as an ordinary\n    parameter, and the live service enforces it: an invalid key returns 401 {\"detail\":\"Invalid API key\"}. The\n    real gate on the four paid operations is x402 payment (HTTP 402 with a PAYMENT-REQUIRED header, USDC on\n    Base Sepolia); the key is the alternative that bypasses it, tied to a \"pro or enterprise tier\" the\n    rebalance operation mentions and nothing publishes. Free operations need neither. No OAuth,\
  \ no OIDC, no\n    bearer tokens, no discovery documents on the host.\nschemes:\n- name: X-API-Key (undeclared)\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  declared_as: >-\n    An optional header PARAMETER (anyOf string|null, required: false) on each operation — not a securityScheme.\n    A generator reading securitySchemes sees an unauthenticated API.\n  used_by: [list_pools_api_pools_get, best_yield_api_best_yield_get, risk_score_api_risk_score__pool_id__get, simulate_rebalance_api_rebalance_post, a2a_endpoint_a2a_post, a2a_stream_endpoint_a2a_stream_post]\n  issuance: >-\n    Not published. The simulate_rebalance description says \"Requires pro or enterprise tier\"; /yo/api/pricing\n    lists per-request x402 prices and the contact api@chado.studio but no tier, signup or key-issuance page.\n  observed:\n  - {request: 'GET https://llama.box/yo/api/best-yield?top=1 with X-API-Key: invalid-probe', status: 401, body: '{\"detail\":\"Invalid API key\"}', fetched: '2026-09-19'}\n\
  \  - {request: 'GET https://llama.box/yo/api/best-yield?top=1 with no key', status: 200, fetched: '2026-09-19', note: free operation}\n  - {request: 'POST https://llama.box/yo/api/rebalance with no key', status: 402, body: '{}', fetched: '2026-09-19', note: paid operation — x402 challenge in the PAYMENT-REQUIRED header}\n  sources:\n  - openapi/llama-box-crvusd-yield-optimizer-openapi.yml\n- name: x402 payment\n  type: payment\n  standard: x402 v2 (HTTP 402 Payment Required)\n  in: header\n  parameter: X-PAYMENT (request) / PAYMENT-REQUIRED (challenge response)\n  description: >-\n    Per /yo/api/pricing: \"1. Request any paid endpoint without payment -> get 402 with payment details.\n    2. Sign a USDC payment on Base using the returned parameters. 3. Resend request with X-PAYMENT header ->\n    get 200 with data.\" The observed challenge is x402Version 2, scheme \"exact\", network eip155:84532 (Base\n    Sepolia testnet), asset 0x036CbD53842c5426634e7929541eC2318f3dCF7e (extra.name USDC,\
  \ extra.version 2),\n    payTo 0x6a1175D0EA0e6817786Ce51F1C4F3294F907f410, maxTimeoutSeconds 300, amount 10000 base units\n    ($0.01) for POST /a2a.\n  applies_to:\n  - {operation: risk_score_api_risk_score__pool_id__get, price: '$0.005'}\n  - {operation: simulate_rebalance_api_rebalance_post, price: '$0.01'}\n  - {operation: a2a_endpoint_a2a_post, price: '$0.01'}\n  - {operation: a2a_stream_endpoint_a2a_stream_post, price: '$0.01'}\n  free_operations: [health_health_get, list_pools_api_pools_get, best_yield_api_best_yield_get, pricing_api_pricing_get, agent_card__well_known_agent_json_get, access_log_api_access_log_get]\n  note: >-\n    Not a securityScheme in the OpenAPI and not declared in the agent card. The paid operations declare only\n    200 and 422 responses; the 402 is undocumented in the contract and discoverable only by calling.\n  sources:\n  - https://llama.box/yo/api/pricing\n  - a2a/llama-box-a2a.yml (x-evidence: decoded PAYMENT-REQUIRED header)\ndiscovery_documents:\n\
  \  openid_configuration: 404\n  oauth_authorization_server: 404\n  oauth_protected_resource: 404\n  note: See well-known/llama-box-well-known.yml.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/llama-box/refs/heads/main/authentication/llama-box-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Agents
- A2A
- x402
- DeFi
- Yield
- Curve Finance
- crvUSD
- Stablecoins
- Risk Scoring
- Analytics
- Agent-Native
---
