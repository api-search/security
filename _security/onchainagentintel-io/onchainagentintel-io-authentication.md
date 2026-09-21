---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: onchainagentintel-io-openapi.yml
  format: yaml
  label: Agent Zero ERC-8004 Agent Intelligence API
  slug: agent-zero-erc-8004-agent-intelligence-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/onchainagentintel-io/refs/heads/main/openapi/onchainagentintel-io-openapi.yml
auth_types:
- apiKey
description: Account-less and key-less. The docs state "All endpoints are x402-gated. No accounts or API keys required." The free /v1/public/* operations, the discovery documents and the MCP server need nothing; every paid operation (tag paid-x402) answers HTTP 402 first and treats a valid x402 payment proof as the credential. There is no OAuth, no OIDC, no bearer token and no user identity — the payer wallet address is the only principal, and a 30-day subscription binds entitlement to that wallet (wallet=<addr> query parameter). Baseline derived from the single securityScheme in the OpenAPI, upgraded from the docs' Quick Start, x402 Payment Flow and USDC via EIP-3009 sections and the services page.
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Onchainagentintel Io Authentication
name_suffix: Authentication
oauth_flows: []
overview: Agent Zero secures its APIs with apiKey across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Agent Zero
provider_slug: onchainagentintel-io
scheme_count: 3
schemes:
- assets:
    base: '0x833589fCD6eDb6E08f4c7C32D4f71b54bdA02913'
    ethereum: '0xA0b86991c6218b36c1d19D4a2e9Eb0cE3606eB48'
  description: x402 v1 payment envelope (base64-encoded JSON). Paid endpoints return HTTP 402 with an `accepts[]` list of accepted payment methods (USDC on Base/Ethereum via EIP-3009, or native ETH). Sign a payment authorization matching one of those entries, base64-encode it, and retry with this header set to receive the 200 response.
  flow:
  - Call the paid operation with no header; read the 402 body (x402Version, accepts[], payment_options[], preview, and the server-issued id such as intel_id or sub_id).
  - Choose an accepts[] entry for a chain you can sign on (base-mainnet chainId 8453 or ethereum-mainnet chainId 1).
  - Sign an EIP-3009 transferWithAuthorization over the USDC contract named in accepts[].asset (EIP-712 domain name "USD Coin", version "2"), with a fresh random 32-byte nonce and a validBefore of roughly 300 seconds (maxTimeoutSeconds 300).
  - Base64-encode the x402 v1 payload and retry the identical URL and method with X-PAYMENT set; a 200 carries the paid body.
  in: header
  name: x402
  parameter: X-PAYMENT
  pay_to: '0xaCd134d2AAd0b868EDb395F7d151864188caaF1a'
  sources:
  - openapi/onchainagentintel-io-openapi.yml
  - https://onchainagentintel.io/docs#x402-flow
  - https://onchainagentintel.io/docs#usdc-eip3009
  type: apiKey
  x-x402:
    settlement_networks:
    - base
    - ethereum
    version: 1
- description: 'Fallback documented in the provider''s SKILL.md and services page, not declared in the OpenAPI: send the exact ETH amount quoted in payment_options[] to the Safe with calldata `{prefix}{id}` (INTEL-, SUB-, AUDIT- or EVAL-), then retry with X-PAYMENT-TX set to the transaction hash; the payment monitor fulfils the request on confirmation. The 402 response also mirrors this offer in x-payment-address, x-payment-amount-eth, x-payment-calldata, x-payment-chain-id and x-payment-network headers.'
  in: header
  name: x402-native-eth
  parameter: X-PAYMENT-TX
  sources:
  - https://onchainagentintel.io/skill.md
  - https://onchainagentintel.io/services
  type: apiKey
- description: 'Entitlement, not authentication: after POST /v1/intel/subscribe is paid, passing wallet=<subscriber_addr> on the seven covered intel operations returns 200 without a per-call payment for 30 days. Status is polled free at GET /v1/intel/subscription/{sub_id} (PENDING | ACTIVE | EXPIRED).'
  in: query
  name: subscription-wallet
  parameter: wallet
  sources:
  - https://onchainagentintel.io/docs
  - https://api.onchainagentintel.io/agent.json
  type: query
slug: onchainagentintel-io-authentication
source_filename: onchainagentintel-io-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: searched\nsource: openapi/onchainagentintel-io-openapi.yml\ndocs: https://onchainagentintel.io/docs#x402-flow\ndescription: >-\n  Account-less and key-less. The docs state \"All endpoints are x402-gated. No accounts or API keys\n  required.\" The free /v1/public/* operations, the discovery documents and the MCP server need nothing;\n  every paid operation (tag paid-x402) answers HTTP 402 first and treats a valid x402 payment proof as the\n  credential. There is no OAuth, no OIDC, no bearer token and no user identity — the payer wallet address\n  is the only principal, and a 30-day subscription binds entitlement to that wallet\n  (wallet=<addr> query parameter). Baseline derived from the single securityScheme in the OpenAPI, upgraded\n  from the docs' Quick Start, x402 Payment Flow and USDC via EIP-3009 sections and the services page.\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  accounts_required: false\n  api_keys_issued: false\n\
  \  oauth2: false\n  oidc: false\nschemes:\n- name: x402\n  type: apiKey\n  in: header\n  parameter: X-PAYMENT\n  description: >-\n    x402 v1 payment envelope (base64-encoded JSON). Paid endpoints return HTTP 402 with an `accepts[]`\n    list of accepted payment methods (USDC on Base/Ethereum via EIP-3009, or native ETH). Sign a payment\n    authorization matching one of those entries, base64-encode it, and retry with this header set to\n    receive the 200 response.\n  flow:\n  - Call the paid operation with no header; read the 402 body (x402Version, accepts[], payment_options[], preview, and the server-issued id such as intel_id or sub_id).\n  - Choose an accepts[] entry for a chain you can sign on (base-mainnet chainId 8453 or ethereum-mainnet chainId 1).\n  - Sign an EIP-3009 transferWithAuthorization over the USDC contract named in accepts[].asset (EIP-712 domain name \"USD Coin\", version \"2\"), with a fresh random 32-byte nonce and a validBefore of roughly 300 seconds (maxTimeoutSeconds\
  \ 300).\n  - Base64-encode the x402 v1 payload and retry the identical URL and method with X-PAYMENT set; a 200 carries the paid body.\n  pay_to: '0xaCd134d2AAd0b868EDb395F7d151864188caaF1a'\n  assets:\n    base: '0x833589fCD6eDb6E08f4c7C32D4f71b54bdA02913'\n    ethereum: '0xA0b86991c6218b36c1d19D4a2e9Eb0cE3606eB48'\n  x-x402: {version: 1, settlement_networks: [base, ethereum]}\n  sources:\n  - openapi/onchainagentintel-io-openapi.yml\n  - https://onchainagentintel.io/docs#x402-flow\n  - https://onchainagentintel.io/docs#usdc-eip3009\n- name: x402-native-eth\n  type: apiKey\n  in: header\n  parameter: X-PAYMENT-TX\n  description: >-\n    Fallback documented in the provider's SKILL.md and services page, not declared in the OpenAPI: send the\n    exact ETH amount quoted in payment_options[] to the Safe with calldata `{prefix}{id}` (INTEL-, SUB-,\n    AUDIT- or EVAL-), then retry with X-PAYMENT-TX set to the transaction hash; the payment monitor fulfils\n    the request on confirmation. The\
  \ 402 response also mirrors this offer in x-payment-address,\n    x-payment-amount-eth, x-payment-calldata, x-payment-chain-id and x-payment-network headers.\n  sources:\n  - https://onchainagentintel.io/skill.md\n  - https://onchainagentintel.io/services\n- name: subscription-wallet\n  type: query\n  in: query\n  parameter: wallet\n  description: >-\n    Entitlement, not authentication: after POST /v1/intel/subscribe is paid, passing wallet=<subscriber_addr>\n    on the seven covered intel operations returns 200 without a per-call payment for 30 days. Status is\n    polled free at GET /v1/intel/subscription/{sub_id} (PENDING | ACTIVE | EXPIRED).\n  sources:\n  - https://onchainagentintel.io/docs\n  - https://api.onchainagentintel.io/agent.json\nmcp:\n  endpoint: https://api.onchainagentintel.io/mcp\n  auth: none\n  protected_resource_metadata: absent (404 at /.well-known/oauth-protected-resource on the API host)\na2a:\n  endpoint: https://api.onchainagentintel.io/a2a/v1\n  auth: a2a-x402\
  \ v0.2 payment extension (required); no securitySchemes declared in the card\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/onchainagentintel-io/refs/heads/main/authentication/onchainagentintel-io-authentication.yml
summary_line: apiKey · 3 schemes
tags:
- Agents
- Agent Intelligence
- ERC-8004
- x402
- Agentic Commerce
- Blockchain
- Ethereum
- Base
- Web3
- MCP
- A2A
- Smart Contracts
- Security Audits
- agent-native
---
