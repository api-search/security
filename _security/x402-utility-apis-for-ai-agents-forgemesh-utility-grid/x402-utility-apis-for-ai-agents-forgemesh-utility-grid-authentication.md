---
anonymous_access: false
api_key_in: []
api_specs:
- filename: x402-utility-apis-for-ai-agents-forgemesh-utility-grid-openapi.json
  format: json
  label: x402 Utility Grid API
  slug: x402-utility-grid-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/x402-utility-apis-for-ai-agents-forgemesh-utility-grid/refs/heads/main/openapi/x402-utility-apis-for-ai-agents-forgemesh-utility-grid-openapi.json
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: X402 Utility Apis For Ai Agents Forgemesh Utility Grid Authentication
name_suffix: Authentication
oauth_flows: []
overview: x402 Utility APIs for AI Agents — ForgeMesh Utility Grid declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: x402 Utility APIs for AI Agents — ForgeMesh Utility Grid
provider_slug: x402-utility-apis-for-ai-agents-forgemesh-utility-grid
scheme_count: 1
schemes:
- asset: USDC
  description: 'HTTP 402 payment challenge; pay in USDC on Base (eip155:8453) via signed EIP-3009 authorization and retry. Facilitator: Coinbase CDP (https://api.cdp.coinbase.com/platform/v2/x402).'
  id: x402
  in: header
  name: PAYMENT-SIGNATURE
  network: eip155:8453
  pay_to:
  - '0x850363a27F0aC6fEb9C7a3eC4C1d295262dF9432'
  - '0x84A1827F1705C257e80771fDc2B152Aea4A57a08'
  type: x402
slug: x402-utility-apis-for-ai-agents-forgemesh-utility-grid-authentication
source_filename: x402-utility-apis-for-ai-agents-forgemesh-utility-grid-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-17'\nmethod: searched\nsource: agent-card securitySchemes + /.well-known/x402.json + OpenAPI x-payment-info\ndocs: https://x402.forgemesh.io/llms.txt\nsummary: 'No API keys, no OAuth, no accounts. The sole credential is an x402 payment: every route answers\n  HTTP 402 with a machine-readable payment challenge; the caller signs an EIP-3009 USDC authorization\n  on Base (eip155:8453) and retries with the PAYMENT-SIGNATURE header. Catalog/discovery is unauthenticated\n  and free.'\nschemes:\n- id: x402\n  type: x402\n  in: header\n  name: PAYMENT-SIGNATURE\n  description: 'HTTP 402 payment challenge; pay in USDC on Base (eip155:8453) via signed EIP-3009 authorization\n    and retry. Facilitator: Coinbase CDP (https://api.cdp.coinbase.com/platform/v2/x402).'\n  network: eip155:8453\n  asset: USDC\n  pay_to:\n  - '0x850363a27F0aC6fEb9C7a3eC4C1d295262dF9432'\n  - '0x84A1827F1705C257e80771fDc2B152Aea4A57a08'\nnotes: OpenAPI declares no components.securitySchemes\
  \ because the credential is out-of-band (payment),\n  not an API-key/OAuth scheme; the auth model is published via the agent card securitySchemes block and\n  the x402 discovery manifest.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/x402-utility-apis-for-ai-agents-forgemesh-utility-grid/refs/heads/main/authentication/x402-utility-apis-for-ai-agents-forgemesh-utility-grid-authentication.yml
summary_line: 1 scheme
tags:
- x402
- agent-native
- mcp-server
- llms-txt
- openapi
- pay-per-call
- usdc
- base-l2
- micropayments
- ai-agents
- utility-api
- geo
- weather
- vision
- ocr
- embeddings
- web-extraction
- dns-domains
- conversions
- economic-data
---
