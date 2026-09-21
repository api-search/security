---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: seshat-markets-agent-api-openapi.yml
  format: yaml
  label: Seshat Markets Agent API
  slug: seshat-markets-agent-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/seshat-markets/refs/heads/main/openapi/seshat-markets-agent-api-openapi.yml
- filename: seshat-markets-agent-intelligence-api-openapi.yml
  format: yaml
  label: Seshat Markets Agent Intelligence API
  slug: seshat-markets-agent-intelligence-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/seshat-markets/refs/heads/main/openapi/seshat-markets-agent-intelligence-api-openapi.yml
- filename: seshat-markets-analysis-api-openapi.yml
  format: yaml
  label: Seshat Markets Analysis API
  slug: seshat-markets-analysis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/seshat-markets/refs/heads/main/openapi/seshat-markets-analysis-api-openapi.yml
- filename: seshat-markets-discovery-api-openapi.yml
  format: yaml
  label: Seshat Markets Discovery API
  slug: seshat-markets-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/seshat-markets/refs/heads/main/openapi/seshat-markets-discovery-api-openapi.yml
- filename: seshat-markets-experimental-api-openapi.yml
  format: yaml
  label: Seshat Markets Experimental API
  slug: seshat-markets-experimental-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/seshat-markets/refs/heads/main/openapi/seshat-markets-experimental-api-openapi.yml
- filename: seshat-markets-forecast-api-openapi.yml
  format: yaml
  label: Seshat Markets Forecast API
  slug: seshat-markets-forecast-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/seshat-markets/refs/heads/main/openapi/seshat-markets-forecast-api-openapi.yml
- filename: seshat-markets-market-intelligence-api-openapi.yml
  format: yaml
  label: Seshat Markets Market Intelligence API
  slug: seshat-markets-market-intelligence-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/seshat-markets/refs/heads/main/openapi/seshat-markets-market-intelligence-api-openapi.yml
- filename: seshat-markets-semantic-similarity-api-openapi.yml
  format: yaml
  label: Seshat Markets Semantic Similarity API
  slug: seshat-markets-semantic-similarity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/seshat-markets/refs/heads/main/openapi/seshat-markets-semantic-similarity-api-openapi.yml
- filename: seshat-markets-signal-api-openapi.yml
  format: yaml
  label: Seshat Markets Signal API
  slug: seshat-markets-signal-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/seshat-markets/refs/heads/main/openapi/seshat-markets-signal-api-openapi.yml
- filename: seshat-markets-verification-api-openapi.yml
  format: yaml
  label: Seshat Markets Verification API
  slug: seshat-markets-verification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/seshat-markets/refs/heads/main/openapi/seshat-markets-verification-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Seshat Markets Authentication
name_suffix: Authentication
oauth_flows: []
overview: Seshat Markets secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Seshat Markets
provider_slug: seshat-markets
scheme_count: 1
schemes:
- description: x402 v2 payment payload. Required for paid endpoints when the service manifest at /.well-known/x402 has enforcement=active_mainnet. Send the signed payment in this header (or the legacy X-PAYMENT header) to satisfy the 402 challenge.
  in: header
  name: x402Payment
  parameter: PAYMENT-SIGNATURE
  sources:
  - openapi/seshat-markets-kronos-quant-signal-api-openapi.json
  type: apiKey
slug: seshat-markets-authentication
source_filename: seshat-markets-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: searched\nsource: openapi/seshat-markets-kronos-quant-signal-api-openapi.json\ndocs: https://kronos.seshat.markets/docs#x402\nmodel: >-\n  Keyless by design: x402 micropayments ARE the authentication. Paid endpoints answer HTTP\n  402 with a signed payment requirement (price, USDC asset, destination, network); the\n  buyer-controlled wallet signs an authorization and the client retries with the payment in\n  the PAYMENT-SIGNATURE (or legacy X-PAYMENT) header. Settlement is real USDC on Solana\n  mainnet (~400ms) or Base L2 (~2s) via the PayAI facilitator, using EIP-3009/Permit2 (EVM)\n  or exact SVM (Solana) schemes - see /.well-known/x402 (saved in well-known/). Free\n  endpoints require no credentials at all; there is no signup, no API key, and no OAuth.\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: x402Payment\n  type: apiKey\n  in: header\n  parameter: PAYMENT-SIGNATURE\n  description: x402 v2 payment payload.\
  \ Required for paid endpoints when the service manifest\n    at /.well-known/x402 has enforcement=active_mainnet. Send the signed payment in this header\n    (or the legacy X-PAYMENT header) to satisfy the 402 challenge.\n  sources:\n  - openapi/seshat-markets-kronos-quant-signal-api-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/seshat-markets/refs/heads/main/authentication/seshat-markets-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Finance
- Fintech
- Crypto
- Commodities
- Forecasting
- Predictions
- Market Data
- Trading Signals
- Research
- AI Agents
- MCP
- A2A
- x402
- llms-txt
- Agent Skills
---
