---
anonymous_access: true
api_key_in: []
api_specs:
- filename: gitdealflow-com-signals-openapi.yml
  format: yaml
  label: VC Deal Flow Signal API
  slug: vc-deal-flow-signal-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitdealflow-com/refs/heads/main/openapi/gitdealflow-com-signals-openapi.yml
auth_types:
- none
- http-bearer
- x402-payment
- oauth2-client-credentials
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Gitdealflow Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: GitDealFlow secures its APIs with none, http-bearer, x402-payment, and oauth2-client-credentials across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: GitDealFlow
provider_slug: gitdealflow-com
scheme_count: 4
schemes:
- applies_to: every GET route (signals, answers, search, badges, citations, pricing, changelog, dataset, methodology, glossary, receipts, markets, scout predict) and the MCP/A2A/NLWeb endpoints
  name: none
  observed: 200 anonymous on /api/signals.json, /api/openapi.json, MCP initialize/tools/list, A2A tasks/get, NLWeb GET
  type: none
- bearerFormat: gdf_v2.<customerId>.<hmac>
  description: Per-request credit-pack API key delivered by email after Stripe checkout (EUR 19 = 100 credits). HMAC-keyed, validated without a database lookup per the credits page. Format gdf_v2.<stripe_customer_id>.<hmac16>.
  failure: 401 {"error":"missing_api_key", ...purchaseUrl, x402Url} (observed); 402 when credits are exhausted
  header: 'Authorization: Bearer gdf_v2.…'
  mcp_env: GITDEALFLOW_API_KEY (stdio package, paid tools)
  name: creditPackKey
  obtain: https://signals.gitdealflow.com/agents/credits
  operations:
  - getDeepSignal
  - redeemDeepSignalSolana
  - getCredits
  rotation: 'support page: never email the full key; send the first eight characters and support verifies or rotates it'
  scheme: bearer
  sources:
  - openapi/gitdealflow-com-signals-openapi.yml
  type: http
- description: No account or key; the agent's wallet signs each request. 402 challenge observed with accepts[] {scheme exact, network base, asset 0x8335…2913 USDC, maxAmountRequired 190000, maxTimeoutSeconds 30}; settled by the Coinbase x402 facilitator. Misses (404) are not charged.
  header: X-PAYMENT (request) / X-PAYMENT-RESPONSE and PAYMENT-REQUIRED (response)
  name: x402
  operations:
  - getDeepSignalX402
  scheme: x402 (HTTP 402 + EIP-3009 transferWithAuthorization, USDC on Base mainnet)
  type: payment
- applies_to: https://signals.gitdealflow.com/api/mcp/rpc
  client_authentication: none (anonymous clients receive a token)
  detail: scopes/gitdealflow-com-scopes.yml
  flow: clientCredentials
  metadata: https://signals.gitdealflow.com/.well-known/oauth-authorization-server
  name: oauth2-client-credentials
  observed: POST grant_type=client_credentials&scope=mcp:read -> 200, Bearer JWT, expires_in 3600
  required: false
  scopes:
    mcp:read: Read access to the MCP server
  token_url: https://signals.gitdealflow.com/api/oauth/token
  type: oauth2
slug: gitdealflow-com-authentication
source_filename: gitdealflow-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: searched\nsource: openapi/gitdealflow-com-signals-openapi.yml (securitySchemes.creditPackKey, per-operation security, getDeepSignalX402 description), https://signals.gitdealflow.com/agents/credits, https://signals.gitdealflow.com/developers, https://signals.gitdealflow.com/.well-known/oauth-authorization-server, https://signals.gitdealflow.com/.well-known/mcp.json, live probes 2026-09-19 (401 body on POST /api/agent/deep-signal, 402 on /x402, 200 token from /api/oauth/token)\ndocs: https://signals.gitdealflow.com/agents/credits\nsummary:\n  types: [none, http-bearer, x402-payment, oauth2-client-credentials]\n  default: none — 34 of 37 operations and all 11 free MCP tools require no credentials\n  global_security: null (spec declares security per operation only)\nschemes:\n- name: none\n  type: none\n  applies_to: every GET route (signals, answers, search, badges, citations, pricing, changelog, dataset, methodology, glossary, receipts, markets,\
  \ scout predict) and the MCP/A2A/NLWeb endpoints\n  observed: 200 anonymous on /api/signals.json, /api/openapi.json, MCP initialize/tools/list, A2A tasks/get, NLWeb GET\n- name: creditPackKey\n  type: http\n  scheme: bearer\n  bearerFormat: gdf_v2.<customerId>.<hmac>\n  description: Per-request credit-pack API key delivered by email after Stripe checkout (EUR 19 = 100 credits). HMAC-keyed, validated without a database lookup per the credits page. Format gdf_v2.<stripe_customer_id>.<hmac16>.\n  header: 'Authorization: Bearer gdf_v2.…'\n  operations: [getDeepSignal, redeemDeepSignalSolana, getCredits]\n  mcp_env: GITDEALFLOW_API_KEY (stdio package, paid tools)\n  failure: 401 {\"error\":\"missing_api_key\", ...purchaseUrl, x402Url} (observed); 402 when credits are exhausted\n  obtain: https://signals.gitdealflow.com/agents/credits\n  rotation: 'support page: never email the full key; send the first eight characters and support verifies or rotates it'\n  sources: [openapi/gitdealflow-com-signals-openapi.yml]\n\
  - name: x402\n  type: payment\n  scheme: x402 (HTTP 402 + EIP-3009 transferWithAuthorization, USDC on Base mainnet)\n  header: X-PAYMENT (request) / X-PAYMENT-RESPONSE and PAYMENT-REQUIRED (response)\n  operations: [getDeepSignalX402]\n  description: No account or key; the agent's wallet signs each request. 402 challenge observed with accepts[] {scheme exact, network base, asset 0x8335…2913 USDC, maxAmountRequired 190000, maxTimeoutSeconds 30}; settled by the Coinbase x402 facilitator. Misses (404) are not charged.\n- name: oauth2-client-credentials\n  type: oauth2\n  flow: clientCredentials\n  token_url: https://signals.gitdealflow.com/api/oauth/token\n  scopes: {mcp:read: Read access to the MCP server}\n  client_authentication: none (anonymous clients receive a token)\n  required: false\n  applies_to: https://signals.gitdealflow.com/api/mcp/rpc\n  metadata: https://signals.gitdealflow.com/.well-known/oauth-authorization-server\n  observed: POST grant_type=client_credentials&scope=mcp:read\
  \ -> 200, Bearer JWT, expires_in 3600\n  detail: scopes/gitdealflow-com-scopes.yml\nkey_prefixes:\n  gdf_v2: credit-pack API key (paid REST routes / paid MCP tool)\ntest_mode: none — no sandbox or test keys are published (sandbox/ intentionally absent)\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gitdealflow-com/refs/heads/main/authentication/gitdealflow-com-authentication.yml
summary_line: none/http-bearer/x402-payment/oauth2-client-credentials · 4 schemes
tags:
- Venture Capital
- Deal Flow
- Startups
- GitHub
- Alternative Data
- Investing
- MCP
- Agents
- Developer Tools
- A2A
---
