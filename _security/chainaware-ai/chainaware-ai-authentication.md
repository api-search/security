---
anonymous_access: false
api_key_in:
- header
- query (MCP SSE URL only)
- tool argument (MCP, in-band)
api_specs:
- filename: chainaware-ai-enterprise-api-openapi.yml
  format: yaml
  label: ChainAware Enterprise API
  slug: chainaware-enterprise-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chainaware-ai/refs/heads/main/openapi/chainaware-ai-enterprise-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 6
method: searched
name: Chainaware Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: ChainAware.ai secures its APIs with apiKey across 6 declared security schemes, as derived from its OpenAPI definitions.
provider_name: ChainAware.ai
provider_slug: chainaware-ai
scheme_count: 6
schemes:
- description: Your ChainAware API key. Available at chainaware.ai/profile. Keep it private — do not expose it in client-side code or public repositories.
  failure: 'Docs: 401 Unauthorized when missing or invalid. Observed: a request with NO key to enterprise.api.chainaware.ai is answered 403 {"message":"Forbidden"} by the AWS API Gateway edge before the application sees it.'
  in: header
  name: ApiKeyAuth
  parameter: x-api-key
  sources:
  - openapi/chainaware-ai-enterprise-api-openapi.yml
  - https://chainaware.ai/learn/api/index.html
  surface: REST Enterprise API (https://enterprise.api.chainaware.ai) and the x402 REST twin at https://api.chainaware.ai/api/*
  type: apiKey
- description: API key for authenticated access. Obtain your key at https://chainaware.ai/pricing.
  in: header
  name: apiKey (A2A card)
  parameter: x-api-key
  sources:
  - a2a/chainaware-ai-agent-card.json
  surface: A2A skills at https://api.chainaware.ai/api/a2a/
  type: apiKey
- description: 'x402 micropayment header. See https://x402.org for payment construction details. An unpaid request returns HTTP 402 with a base64 `payment-required` header (x402 v2 PaymentRequirements: exact scheme, eip155:8453, 150000 units of USDC 0x8335…2913 = $0.15, payTo 0x9e60…CeA08, 300 s validity).'
  evidence: a2a/chainaware-ai-x402-payment-required.json
  in: header
  name: x402Payment
  parameter: X-PAYMENT
  sources:
  - a2a/chainaware-ai-agent-card.json
  - https://api.chainaware.ai/api/capabilities
  surface: A2A skills and https://api.chainaware.ai/api/* (and MCP tool calls when apiKey is omitted, per the README)
  type: apiKey
- description: Documented connection-level key; the connection, initialize and tools/list nevertheless succeed without it.
  in: header
  name: X-API-Key (MCP connection header)
  parameter: X-API-Key
  sources:
  - https://chainaware.ai/learn/prediction-mcp/setup.html
  - mcp/chainaware-ai-mcp.yml
  surface: MCP SSE connection to https://prediction.mcp.chainaware.ai/sse (Claude Code `--header`, Cursor `headers`, SDK requestInit)
  type: apiKey
- description: The setup guide documents the key in the URL for clients that cannot set headers. A key in a URL is logged by intermediaries; the guide does not warn about this.
  in: query
  name: apiKey (MCP SSE query parameter)
  parameter: apiKey
  sources:
  - https://chainaware.ai/learn/prediction-mcp/setup.html
  surface: 'MCP SSE URL for ChatGPT Connectors and Claude Web/Desktop Integrations: https://prediction.mcp.chainaware.ai/sse?apiKey=YOUR_API_KEY'
  type: apiKey
- description: 'The credential travels INSIDE the JSON-RPC tool call, visible to the model. SKILL.md: "Passed as the apiKey parameter in every tool call ... Never logged or included in output. Sourced exclusively from the CHAINAWARE_API_KEY environment variable — never hardcoded." Omit it to pay with x402 instead (README). Failure: 403 "invalid or missing apiKey" as tool-result text.'
  in: tool-argument
  name: apiKey (MCP tool argument)
  parameter: apiKey
  sources:
  - mcp/chainaware-ai-mcp-tools.json
  - skills/chainaware-ai-SKILL.md
  surface: 'Six MCP tools: predictive_fraud, predictive_fraud_batch, predictive_behaviour, predictive_behaviour_batch, predictive_rug_pull, credit_score (required inputSchema property)'
  type: apiKey
slug: chainaware-ai-authentication
source_filename: chainaware-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: searched\nsource: openapi/chainaware-ai-enterprise-api-openapi.yml\ndocs: https://chainaware.ai/learn/api/index.html\nadditional_docs:\n- https://chainaware.ai/learn/prediction-mcp/setup.html\n- https://api.chainaware.ai/.well-known/agent-card.json\n- https://github.com/ChainAware/behavioral-prediction-mcp\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  - query (MCP SSE URL only)\n  - tool argument (MCP, in-band)\n  payment_credential:\n  - x402 (X-PAYMENT header, USDC on Base)\n  oauth2: false\n  openid_connect: false\n  mutual_tls: false\n  key_issuance: https://chainaware.ai/profile (Business or Enterprise subscription; \"custom volume pricing\" by contact)\n  anonymous_access: 'discovery on every surface (agent card, /api/capabilities, MCP initialize + tools/list); eight MCP tools callable with no key; website tools free'\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  surface: REST Enterprise\
  \ API (https://enterprise.api.chainaware.ai) and the x402 REST twin at https://api.chainaware.ai/api/*\n  description: Your ChainAware API key. Available at chainaware.ai/profile. Keep it private — do not expose it in client-side code or public repositories.\n  failure: 'Docs: 401 Unauthorized when missing or invalid. Observed: a request with NO key to enterprise.api.chainaware.ai is answered 403 {\"message\":\"Forbidden\"} by the AWS API Gateway edge before the application sees it.'\n  sources:\n  - openapi/chainaware-ai-enterprise-api-openapi.yml\n  - https://chainaware.ai/learn/api/index.html\n- name: apiKey (A2A card)\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  surface: A2A skills at https://api.chainaware.ai/api/a2a/\n  description: 'API key for authenticated access. Obtain your key at https://chainaware.ai/pricing.'\n  sources:\n  - a2a/chainaware-ai-agent-card.json\n- name: x402Payment\n  type: apiKey\n  in: header\n  parameter: X-PAYMENT\n  surface: A2A skills and\
  \ https://api.chainaware.ai/api/* (and MCP tool calls when apiKey is omitted, per the README)\n  description: 'x402 micropayment header. See https://x402.org for payment construction details. An unpaid request returns HTTP 402 with a base64 `payment-required` header (x402 v2 PaymentRequirements: exact scheme, eip155:8453, 150000 units of USDC 0x8335…2913 = $0.15, payTo 0x9e60…CeA08, 300 s validity).'\n  evidence: a2a/chainaware-ai-x402-payment-required.json\n  sources:\n  - a2a/chainaware-ai-agent-card.json\n  - https://api.chainaware.ai/api/capabilities\n- name: X-API-Key (MCP connection header)\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  surface: MCP SSE connection to https://prediction.mcp.chainaware.ai/sse (Claude Code `--header`, Cursor `headers`, SDK requestInit)\n  description: Documented connection-level key; the connection, initialize and tools/list nevertheless succeed without it.\n  sources:\n  - https://chainaware.ai/learn/prediction-mcp/setup.html\n  - mcp/chainaware-ai-mcp.yml\n\
  - name: apiKey (MCP SSE query parameter)\n  type: apiKey\n  in: query\n  parameter: apiKey\n  surface: 'MCP SSE URL for ChatGPT Connectors and Claude Web/Desktop Integrations: https://prediction.mcp.chainaware.ai/sse?apiKey=YOUR_API_KEY'\n  description: The setup guide documents the key in the URL for clients that cannot set headers. A key in a URL is logged by intermediaries; the guide does not warn about this.\n  sources:\n  - https://chainaware.ai/learn/prediction-mcp/setup.html\n- name: apiKey (MCP tool argument)\n  type: apiKey\n  in: tool-argument\n  parameter: apiKey\n  surface: 'Six MCP tools: predictive_fraud, predictive_fraud_batch, predictive_behaviour, predictive_behaviour_batch, predictive_rug_pull, credit_score (required inputSchema property)'\n  description: 'The credential travels INSIDE the JSON-RPC tool call, visible to the model. SKILL.md: \"Passed as the apiKey parameter in every tool call ... Never logged or included in output. Sourced exclusively from the CHAINAWARE_API_KEY\
  \ environment variable — never hardcoded.\" Omit it to pay with x402 instead (README). Failure: 403 \"invalid or missing apiKey\" as tool-result text.'\n  sources:\n  - mcp/chainaware-ai-mcp-tools.json\n  - skills/chainaware-ai-SKILL.md\nnote: >-\n  One credential (a ChainAware API key) presented five ways across three surfaces, plus x402 payment as a\n  credential-free alternative on the agent surfaces. No OAuth 2.0, OIDC, scopes or client registration exist,\n  and no RFC 8414 / 9728 discovery document is served on any host (see well-known/). Keys are per account with\n  no documented test/live prefix, rotation or expiry.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chainaware-ai/refs/heads/main/authentication/chainaware-ai-authentication.yml
summary_line: apiKey · 6 schemes
tags:
- Blockchain
- Web3
- DeFi
- Fraud Detection
- AML
- Compliance
- Credit Scoring
- Risk Scoring
- Smart Contract Security
- Agent Trust
- MCP
- A2A
- x402
- Agents
- Agent-Native
- Estonia
---
