---
anonymous_access: false
api_key_in: []
api_specs:
- filename: berrergate-com-openapi.json
  format: json
  label: BerrerGate Tool & Provider Intelligence API
  slug: berrergate-tool-provider-intelligence-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/berrergate-com/refs/heads/main/openapi/berrergate-com-openapi.json
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 0
method: searched
name: Berrergate Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: Berrer declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Berrer
provider_slug: berrergate-com
scheme_count: 0
schemes: []
slug: berrergate-com-authentication
source_filename: berrergate-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: searched\nsource: https://api.berrergate.com/llms.txt\nderived_from: openapi/berrergate-com-openapi.json\ndocs:\n- https://api.berrergate.com/skill.md\n- https://api.berrergate.com/.well-known/x402.json\nsummary: >-\n  BerrerGate has NO authentication scheme: the OpenAPI declares no securitySchemes and no security\n  requirement, the A2A card declares securitySchemes {} and securityRequirements [], and no OAuth/OIDC\n  metadata is served on any host. Every read route and the free preview POSTs answer anonymously. Access to\n  the paid routes is gated economically, per request, by x402 payment: the first call returns HTTP 402 with\n  PaymentRequirements, and the retry carries a PAYMENT-SIGNATURE header settling USDC on Base. There are no\n  accounts, API keys, tokens or signups (\"without creating a traditional account\"). derive-authentication.py\n  produced no profile because the contract declares nothing; this file was written from the observed\n\
  \  requests and the provider's own docs.\nschemes: []\naccess_model:\n  anonymous_reads: true\n  anonymous_free_writes: ['POST /v1/agent/procurement/preview', 'POST /v1/agent/discovery/preview', 'POST /v1/agent/trial/query (free, x-idempotency-key required)', 'POST /a2a/jsonrpc', 'POST /a2a/v1/message:send']\n  payment_gated_writes: ['POST /v1/research ($0.020)', 'POST /v1/agent/beta/query ($0.01)', 'POST /v1/agent/utility/inference ($0.00125-$0.00225 dynamic)', 'POST /v1/agent/utility/spend-router ($0.001, currently disabled)', 'GET /v1/agent/canary/browser-automation-select ($0.01 one-shot)']\n  payment:\n    protocol: x402\n    version: 2\n    request_header: PAYMENT-SIGNATURE\n    challenge_header: PAYMENT-REQUIRED\n    response_header: PAYMENT-RESPONSE\n    scheme: exact\n    network: eip155:8453 (Base mainnet)\n    asset: '0x833589fCD6eDb6E08f4c7C32D4f71b54bdA02913 (USD Coin, version 2)'\n    pay_to: '0x1090DDAf854Ff0f6A65F24a866C29C46fdDa0a8a'\n    max_timeout_seconds: 60\n    observed:\
  \ 'POST /v1/research -> 402 with PAYMENT-REQUIRED header and x402Version 2 body, 2026-09-19'\n    note: Payment is per request and is not an identity; the provider states raw agent identifiers are not retained.\nrequest_headers:\n- name: x-idempotency-key\n  required: true\n  on: ['POST /v1/research', 'POST /v1/agent/beta/query', 'POST /v1/agent/trial/query', 'POST /v1/agent/utility/inference', 'POST /v1/agent/utility/spend-router', 'POST /v1/agent/wisdom/provider-select']\n  observed: 'omitting it on POST /v1/research -> 400 IDEMPOTENCY_KEY_REQUIRED'\n- name: x-agent-id\n  required: false\n  on: ['POST /v1/agent/trial/query (declared)']\n  note: Optional caller-supplied agent identifier; the CORS allow-list also names x-bcg-agent-id, x-bcg-client-version, x-bcg-telemetry-class and x-bcg-discovery-source, none of which the contract documents.\n- name: x-bcg-admin-token\n  required: false\n  note: Appears only in the Access-Control-Allow-Headers list. An operator credential, never documented\
  \ or issued; not a customer scheme.\n- name: MCP-Protocol-Version\n  required: true\n  on: ['POST /mcp']\n  value: '2026-07-28'\nmcp:\n  auth: none\n  oauth_metadata: {oauth_authorization_server: 404, oauth_protected_resource: 404, openid_configuration: 404}\na2a:\n  securitySchemes: {}\n  securityRequirements: []\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/berrergate-com/refs/heads/main/authentication/berrergate-com-authentication.yml
summary_line: 0 schemes
tags:
- Agents
- Agentic Commerce
- A2A
- MCP
- x402
- Procurement
- Tool Discovery
- API Discovery
- Inference
- Research
- Agent-Native
---
