---
anonymous_access: false
api_key_in: []
api_specs:
- filename: cables-openapi.yml
  format: yaml
  label: TensorFlow.js Social Media MCP Server
  slug: tensorflowjs-social-media-mcp-server
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cables/refs/heads/main/openapi/cables-openapi.yml
auth_types:
- none-for-discovery
- x402-payment-for-execution
description: ''
kind: authentication
layout: security
mechanism_count: 0
method: searched
name: Cables Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cables secures its APIs with none-for-discovery and x402-payment-for-execution across 0 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Cables
provider_slug: cables
scheme_count: 0
schemes: []
slug: cables-authentication
source_filename: cables-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-18'\nmethod: searched\nsource: https://mcp.cables.live/openapi.json + live MCP handshake\nsummary:\n  types:\n  - none-for-discovery\n  - x402-payment-for-execution\n  security_schemes_declared: 0\nmodel: 'The OpenAPI declares NO securitySchemes and applies no global security. Discovery is fully anonymous:\n  GET /openapi.json, the MCP initialize/tools/list handshake, and GET /health all succeed without credentials.\n  ACCESS CONTROL IS ECONOMIC, not credential-based: executing any tool requires an x402 micropayment.\n  An unpaid call returns HTTP 402 with a Base64-encoded x402 PaymentRequired object in the Payment-Required\n  header; the agent settles $0.05 USDC on Solana devnet (scheme \"exact\", payTo a fixed Solana address)\n  and retries.'\npayment:\n  protocol: x402\n  network: solana:5eykt4UsFv8P8NJdTREpY1vzqKqZKvdp\n  scheme: exact\n  price_usd: 0.05\n  settlement: USDC on Solana devnet\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cables/refs/heads/main/authentication/cables-authentication.yml
summary_line: none-for-discovery/x402-payment-for-execution · 0 schemes
tags:
- MCP Server
- agent-native
- x402
- pay-per-call
- Machine-Learning
- tensorflow-js
- NLP
- Computer-Vision
- Social Media Analytics
- OpenAPI
- Solana
- Crypto Payments
- testnet-devnet
---
