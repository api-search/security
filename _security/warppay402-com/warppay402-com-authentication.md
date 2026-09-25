---
anonymous_access: false
api_key_in: []
api_specs:
- filename: warppay402-com-openapi.yml
  format: yaml
  label: WarpPay402 Monetized MCP Tools API
  slug: warppay402-monetized-mcp-tools-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/warppay402-com/refs/heads/main/openapi/warppay402-com-openapi.yml
auth_types: []
description: 'WarpPay402 replaces credentials with payment. There is no signup, no API key and no OAuth: an unpaid request to any operation receives HTTP 402 with an x402 v2 challenge, the client signs a USDC transfer for the quoted amount on one of four networks and retries with the signature in a PAYMENT-SIGNATURE header, and the gateway verifies settlement (splitting a platform fee) before proxying the request. The MCP server''s discovery methods (initialize, tools/list, resources/list, prompts/list) are fully anonymous; tool calls are settled the same way through the stdio bridge. A flat-rate monthly access token is offered by email but is undocumented, so it is recorded as a claim, not a scheme.'
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Warppay402 Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: WarpPay402 Studio declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: WarpPay402 Studio
provider_slug: warppay402-com
scheme_count: 2
schemes:
- amount_units: USDC base units, 6 decimals
  applies_to: all 19 REST operations and all 19 MCP tools
  challenge_header: PAYMENT-REQUIRED
  challenge_status: 402
  challenge_ttl_seconds: 300
  client_secret_material: A wallet private key held by the caller (env CUSTOMER_PRIVATE_KEY, alias WALLETPK; CUSTOMER_SOLANA_KEY for Solana in the SDK). It signs locally and is never transmitted; the privacy policy states the provider "never ask[s] for or store[s] private keys or seed phrases".
  evidence:
  - headers:
    - payment-required
    - x-payment-required
    - 'access-control-expose-headers: PAYMENT-REQUIRED, PAYMENT-RESPONSE'
    - 'x-guard-inspected: true'
    method: POST
    status: 402
    url: https://api.warppay402.com/api/v1/tools/web-scraper
  - method: GET
    status: 402
    url: https://api.warppay402.com/api/v1/feeds/base-yields
  - method: GET
    status: 402
    url: https://api.warppay402.com/public_data_feed/index.json
  in: header
  kind: payment-challenge
  name: x402Payment
  networks:
  - asset: '0x833589fCD6eDb6E08f4c7C32D4f71b54bdA02913'
    asset_name: USDC
    authorization: EIP-712 TransferWithAuthorization (gasless)
    caip2: eip155:8453
    chain: Base
  - asset: EPjFWdd5AufqSSqeM2qN1xzybapC8G4wEGGkZwyTDt1v
    asset_name: SPL USDC
    authorization: signed SPL transfer
    caip2: solana:5eykt4UsFv8P8NJdTREpY1vzqKqZKvdp
    chain: Solana mainnet-beta
  - asset: '0xaf88d065e77c8cC2239327C5EDb3A432268e5831'
    asset_name: USDC
    authorization: EIP-712 TransferWithAuthorization
    caip2: eip155:42161
    chain: Arbitrum One
  - asset: '0x0000000000000000000000000000000000000000'
    asset_name: native USDC
    authorization: direct native value transfer
    caip2: eip155:5042
    chain: Arc Mainnet
  receipt_header: PAYMENT-RESPONSE
  replay_protection: server-side nonce store rejects a reused signature (MemoryNonceStore / RedisNonceStore in @warppay402/server)
  request_header: PAYMENT-SIGNATURE
  scheme: exact
  type: x402
  version: 2
- in: unknown
  kind: claimed-undocumented
  name: flatRateAccessToken
  note: 'Homepage: "Access to our endpoints can also be gained through traditional API access tokens. Reach out to us at [obfuscated email] if interested in a flat rate per month." Header name, format and issuance are not published and the OpenAPI declares no scheme, so no agent can use this without a human negotiation.'
  status: offered by email only
  type: apiKey
slug: warppay402-com-authentication
source_filename: warppay402-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: searched\nsource: >-\n  https://www.warppay402.com/ (\"No API Keys or Token Management Needed ... they simply send a raw crypto micro-transaction\n  ($0.01–$0.35 USDC) on Base or Solana directly inside the request header. ... Access to our endpoints can also be gained\n  through traditional API access tokens. Reach out to us ... if interested in a flat rate per month.\"), the\n  @warppay402/server README (x402 V2 headers PAYMENT-REQUIRED / PAYMENT-SIGNATURE / PAYMENT-RESPONSE, EIP-712 gasless\n  TransferWithAuthorization, SPL-USDC, native USDC on Arc), the @warppay402/sdk and @warppay402/mcp-client READMEs\n  (CUSTOMER_PRIVATE_KEY / WALLETPK), and live 402 responses on https://api.warppay402.com observed 2026-09-19.\n  derive-authentication.py produced nothing because the provider's OpenAPI declares no securitySchemes.\ndocs: https://www.warppay402.com/\ndescription: >-\n  WarpPay402 replaces credentials with payment. There is no signup, no\
  \ API key and no OAuth: an unpaid request to any\n  operation receives HTTP 402 with an x402 v2 challenge, the client signs a USDC transfer for the quoted amount on one of\n  four networks and retries with the signature in a PAYMENT-SIGNATURE header, and the gateway verifies settlement\n  (splitting a platform fee) before proxying the request. The MCP server's discovery methods (initialize, tools/list,\n  resources/list, prompts/list) are fully anonymous; tool calls are settled the same way through the stdio bridge. A\n  flat-rate monthly access token is offered by email but is undocumented, so it is recorded as a claim, not a scheme.\nschemes:\n- name: x402Payment\n  type: x402\n  kind: payment-challenge\n  in: header\n  request_header: PAYMENT-SIGNATURE\n  challenge_header: PAYMENT-REQUIRED\n  receipt_header: PAYMENT-RESPONSE\n  challenge_status: 402\n  version: 2\n  scheme: exact\n  applies_to: all 19 REST operations and all 19 MCP tools\n  networks:\n  - {caip2: 'eip155:8453', chain:\
  \ Base, asset: '0x833589fCD6eDb6E08f4c7C32D4f71b54bdA02913', asset_name: USDC, authorization: EIP-712 TransferWithAuthorization (gasless)}\n  - {caip2: 'solana:5eykt4UsFv8P8NJdTREpY1vzqKqZKvdp', chain: Solana mainnet-beta, asset: EPjFWdd5AufqSSqeM2qN1xzybapC8G4wEGGkZwyTDt1v, asset_name: SPL USDC, authorization: signed SPL transfer}\n  - {caip2: 'eip155:42161', chain: Arbitrum One, asset: '0xaf88d065e77c8cC2239327C5EDb3A432268e5831', asset_name: USDC, authorization: EIP-712 TransferWithAuthorization}\n  - {caip2: 'eip155:5042', chain: Arc Mainnet, asset: '0x0000000000000000000000000000000000000000', asset_name: native USDC, authorization: direct native value transfer}\n  challenge_ttl_seconds: 300\n  amount_units: USDC base units, 6 decimals\n  client_secret_material: >-\n    A wallet private key held by the caller (env CUSTOMER_PRIVATE_KEY, alias WALLETPK; CUSTOMER_SOLANA_KEY for Solana in\n    the SDK). It signs locally and is never transmitted; the privacy policy states the provider\
  \ \"never ask[s] for or\n    store[s] private keys or seed phrases\".\n  replay_protection: server-side nonce store rejects a reused signature (MemoryNonceStore / RedisNonceStore in @warppay402/server)\n  evidence:\n  - {url: 'https://api.warppay402.com/api/v1/tools/web-scraper', method: POST, status: 402, headers: ['payment-required', 'x-payment-required', 'access-control-expose-headers: PAYMENT-REQUIRED, PAYMENT-RESPONSE', 'x-guard-inspected: true']}\n  - {url: 'https://api.warppay402.com/api/v1/feeds/base-yields', method: GET, status: 402}\n  - {url: 'https://api.warppay402.com/public_data_feed/index.json', method: GET, status: 402}\n- name: flatRateAccessToken\n  type: apiKey\n  kind: claimed-undocumented\n  in: unknown\n  status: offered by email only\n  note: >-\n    Homepage: \"Access to our endpoints can also be gained through traditional API access tokens. Reach out to us at\n    [obfuscated email] if interested in a flat rate per month.\" Header name, format and issuance are\
  \ not published and\n    the OpenAPI declares no scheme, so no agent can use this without a human negotiation.\nanonymous_surfaces:\n- {url: 'https://api.warppay402.com/mcp', methods: [initialize, tools/list, resources/list, prompts/list], status: 200}\n- {url: 'https://api.warppay402.com/openapi.json', status: 200}\n- {url: 'https://api.warppay402.com/.well-known/agent.json', status: 200}\n- {url: 'https://api.warppay402.com/.well-known/mcp.json', status: 200}\n- {url: 'https://api.warppay402.com/.well-known/x402-manifest.json', status: 200}\n- {url: 'https://api.warppay402.com/agent-offers.json', status: 200}\n- {url: 'https://api.warppay402.com/llms.txt', status: 200}\n- {url: 'https://api.warppay402.com/health', status: 200}\noauth2: false\noidc: false\ndelegated_identity: false\ndynamic_client_registration: false\nprotected_resource_metadata: false\nmcp_auth:\n  discovery: none (anonymous)\n  invocation: x402 payment signed by the @warppay402/mcp-client bridge from CUSTOMER_PRIVATE_KEY;\
  \ an unauthenticated tools/call from this crawler returned a JSON-RPC 200 with an empty result object\n  local_bridge: npx -y @warppay402/mcp-client\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/warppay402-com/refs/heads/main/authentication/warppay402-com-authentication.yml
summary_line: 2 schemes
tags:
- x402
- Micropayments
- AI Agents
- MCP
- A2A
- Agent-Native
- Web Scraping
- Data Extraction
- Blockchain
- DeFi
- Base
- Solana
- Smart Contracts
- Data Feed
- Developer Tools
---
