---
api_key_in: []
api_specs:
- filename: farmdash-account-api-openapi.yml
  format: yaml
  label: FarmDash Agent Hub Account API
  slug: farmdash-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/farmdash/refs/heads/main/openapi/farmdash-account-api-openapi.yml
- filename: farmdash-autopilot-api-openapi.yml
  format: yaml
  label: FarmDash Agent Hub Autopilot API
  slug: farmdash-autopilot-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/farmdash/refs/heads/main/openapi/farmdash-autopilot-api-openapi.yml
- filename: farmdash-delegation-api-openapi.yml
  format: yaml
  label: FarmDash Agent Hub Delegation API
  slug: farmdash-delegation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/farmdash/refs/heads/main/openapi/farmdash-delegation-api-openapi.yml
- filename: farmdash-execution-api-openapi.yml
  format: yaml
  label: FarmDash Agent Hub Execution API
  slug: farmdash-execution-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/farmdash/refs/heads/main/openapi/farmdash-execution-api-openapi.yml
- filename: farmdash-history-api-openapi.yml
  format: yaml
  label: FarmDash Agent Hub History API
  slug: farmdash-history-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/farmdash/refs/heads/main/openapi/farmdash-history-api-openapi.yml
- filename: farmdash-intelligence-api-openapi.yml
  format: yaml
  label: FarmDash Agent Hub Intelligence API
  slug: farmdash-intelligence-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/farmdash/refs/heads/main/openapi/farmdash-intelligence-api-openapi.yml
- filename: farmdash-research-api-openapi.yml
  format: yaml
  label: FarmDash Agent Hub Research API
  slug: farmdash-research-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/farmdash/refs/heads/main/openapi/farmdash-research-api-openapi.yml
- filename: farmdash-risk-api-openapi.yml
  format: yaml
  label: FarmDash Agent Hub Risk API
  slug: farmdash-risk-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/farmdash/refs/heads/main/openapi/farmdash-risk-api-openapi.yml
- filename: farmdash-session-api-openapi.yml
  format: yaml
  label: FarmDash Agent Hub Session API
  slug: farmdash-session-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/farmdash/refs/heads/main/openapi/farmdash-session-api-openapi.yml
- filename: farmdash-strategy-api-openapi.yml
  format: yaml
  label: FarmDash Agent Hub Strategy API
  slug: farmdash-strategy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/farmdash/refs/heads/main/openapi/farmdash-strategy-api-openapi.yml
- filename: farmdash-swap-api-openapi.yml
  format: yaml
  label: FarmDash Agent Hub Swap API
  slug: farmdash-swap-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/farmdash/refs/heads/main/openapi/farmdash-swap-api-openapi.yml
auth_types:
- http
- apiKey-literal
- wallet-signature
- http-payment
description: ''
kind: authentication
layout: security
method: searched
name: Farmdash Authentication
name_suffix: Authentication
oauth_flows: []
overview: FarmDash Agent Hub secures its APIs with http, apiKey-literal, wallet-signature, and http-payment across 7 declared security schemes, as derived from its OpenAPI definitions.
provider_name: FarmDash Agent Hub
provider_slug: farmdash
scheme_count: 7
schemes:
- description: Pioneer or Syndicate API key.
  header: 'Authorization: Bearer <key>'
  issuance: https://www.farmdash.one/api/v1/agent/api-key
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/farmdash-agent-api-openapi.yaml
  spec_declared: true
  type: http
- description: '12 of 27 operations declare `security: [{bearerAuth: []}, {}]` — the empty scheme makes keyless access an explicit part of the contract. Omit the header entirely, or send the published literal `fd_scout_free`.'
  limit: 5 requests / 24h per IP
  name: anonymous (Scout)
  public_literal: fd_scout_free
  spec_declared: true
  type: none
- description: 'Deterministic unmetered mock. Authorization: Bearer fd_sandbox_mock, or ?mock=true, or X-FarmDash-Mock: true.'
  live_data: false
  name: sandbox literal
  scope: /v1/agent/protocols and /v1/trail-heat only
  spec_declared: true
  type: apiKey-literal
- description: 'EIP-191 personal_sign required for zero-custody swap execution (executeSwap). Message template: v1:FARMDASH_SWAP:{fromChainId}:{toChainId}:{fromToken}:{toToken}:{fromAmount}:{agentAddress}:{toAddress}'
  failure_status: 401 (invalid signature or expired nonce)
  name: eip191
  source: https://www.farmdash.one/.well-known/agent.json
  spec_declared: false
  type: wallet-signature
- description: EIP-712 typed-data signature required for Hyperliquid perp order execution (executeOrder) and for the MCP IntentApproval flow (request_approval_payload -> submit_signed_approval).
  name: eip712
  source: https://www.farmdash.one/agents/openapi.yaml (info.description)
  spec_declared: false
  type: wallet-signature
- description: 'One-off USDC payment over HTTP 402. Retry a challenged request with PAYMENT-SIGNATURE, or with the legacy X-Payment-Proof: 0x<txHash>. Declared in the contract via the PaymentRequiredError schema on 24 of 27 operations and verified live (402 observed 2026-08-26).'
  name: x402
  spec_declared: true
  type: http-payment
- description: Bounded session token (32-256 chars per the MCP tool input schemas) required by manageSession, manageAutopilot and the MCP intent-lifecycle tools. 401 = missing/invalid token; 403 = session owner verification failed.
  name: session capability token
  spec_declared: false
  type: bearer-scoped
slug: farmdash-authentication
source_filename: farmdash-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: searched\nsource: https://www.farmdash.one/agents/openapi.yaml\ndocs: https://www.farmdash.one/agents\nsecondary_sources:\n- https://www.farmdash.one/.well-known/agent.json\n- https://www.farmdash.one/api/v1/agent/status\n- https://www.farmdash.one/llms.txt\nsummary:\n  types:\n  - http\n  - apiKey-literal\n  - wallet-signature\n  - http-payment\n  oauth2: false\n  openid_connect: false\n  mutual_tls: false\n  scopes: false\n  scopes_note: >-\n    No OAuth. Authorization is by TIER, not by scope — a key is Scout, Pioneer or Syndicate and\n    that determines which routes answer. No scopes/ artifact is emitted; there is no scope\n    surface to record.\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  spec_declared: true\n  description: Pioneer or Syndicate API key.\n  header: 'Authorization: Bearer <key>'\n  issuance: https://www.farmdash.one/api/v1/agent/api-key\n  sources:\n  - openapi/farmdash-agent-api-openapi.yaml\n- name:\
  \ anonymous (Scout)\n  type: none\n  spec_declared: true\n  description: >-\n    12 of 27 operations declare `security: [{bearerAuth: []}, {}]` — the empty scheme makes\n    keyless access an explicit part of the contract. Omit the header entirely, or send the\n    published literal `fd_scout_free`.\n  limit: 5 requests / 24h per IP\n  public_literal: fd_scout_free\n- name: sandbox literal\n  type: apiKey-literal\n  spec_declared: true\n  description: 'Deterministic unmetered mock. Authorization: Bearer fd_sandbox_mock, or ?mock=true, or X-FarmDash-Mock: true.'\n  scope: /v1/agent/protocols and /v1/trail-heat only\n  live_data: false\n- name: eip191\n  type: wallet-signature\n  spec_declared: false\n  description: >-\n    EIP-191 personal_sign required for zero-custody swap execution (executeSwap). Message\n    template: v1:FARMDASH_SWAP:{fromChainId}:{toChainId}:{fromToken}:{toToken}:{fromAmount}:{agentAddress}:{toAddress}\n  failure_status: 401 (invalid signature or expired nonce)\n\
  \  source: https://www.farmdash.one/.well-known/agent.json\n- name: eip712\n  type: wallet-signature\n  spec_declared: false\n  description: >-\n    EIP-712 typed-data signature required for Hyperliquid perp order execution (executeOrder)\n    and for the MCP IntentApproval flow (request_approval_payload -> submit_signed_approval).\n  source: https://www.farmdash.one/agents/openapi.yaml (info.description)\n- name: x402\n  type: http-payment\n  spec_declared: true\n  description: >-\n    One-off USDC payment over HTTP 402. Retry a challenged request with PAYMENT-SIGNATURE, or\n    with the legacy X-Payment-Proof: 0x<txHash>. Declared in the contract via the\n    PaymentRequiredError schema on 24 of 27 operations and verified live (402 observed\n    2026-08-26).\n- name: session capability token\n  type: bearer-scoped\n  spec_declared: false\n  description: >-\n    Bounded session token (32-256 chars per the MCP tool input schemas) required by\n    manageSession, manageAutopilot and the\
  \ MCP intent-lifecycle tools. 401 = missing/invalid\n    token; 403 = session owner verification failed.\ngaps:\n- finding: >-\n    Only 1 of 7 authentication schemes is machine-readable. components.securitySchemes declares\n    bearerAuth alone; the four wallet/payment/session schemes that actually gate every\n    money-moving operation are documented in prose and in the agent card only.\n- finding: >-\n    The header names for the EIP-191 signature and the session capability token are not\n    published anywhere probed. An integrator can learn that a signature is required but not\n    which header carries it without reading unavailable SDK source.\nzero_custody:\n  private_keys_accepted: false\n  statement: >-\n    \"FarmDash does not request seed phrases or raw wallet private keys.\" State-changing flows\n    require local wallet signatures or explicit bounded delegation. Posture string published at\n    /api/v1/agent/status: customer_keys_never_received_customer_controls_signing_and_submission.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/farmdash/refs/heads/main/authentication/farmdash-authentication.yml
summary_line: http/apiKey-literal/wallet-signature/http-payment · 7 schemes
tags:
- DeFi
- DeFAI
- AI Agents
- MCP
- OpenAPI
- x402
- Blockchain
- Crypto
- airdrop tracking
- Developer Tools
- Agent Readiness
- Machine Payments
- Hyperliquid
- Wallet Intelligence
- zero custody
---
