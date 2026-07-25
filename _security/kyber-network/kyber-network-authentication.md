---
api_key_in: []
api_specs:
- filename: kyber-network-general-api-openapi.yml
  format: yaml
  label: Kyber Network General API
  slug: kyber-network-general-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kyber-network/refs/heads/main/openapi/kyber-network-general-api-openapi.yml
- filename: kyber-network-maker-api-openapi.yml
  format: yaml
  label: Kyber Network Maker API
  slug: kyber-network-maker-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kyber-network/refs/heads/main/openapi/kyber-network-maker-api-openapi.yml
- filename: kyber-network-service-api-openapi.yml
  format: yaml
  label: Kyber Network Service API
  slug: kyber-network-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kyber-network/refs/heads/main/openapi/kyber-network-service-api-openapi.yml
- filename: kyber-network-swap-api-openapi.yml
  format: yaml
  label: Kyber Network swap API
  slug: kyber-network-swap-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kyber-network/refs/heads/main/openapi/kyber-network-swap-api-openapi.yml
- filename: kyber-network-taker-api-openapi.yml
  format: yaml
  label: Kyber Network Taker API
  slug: kyber-network-taker-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kyber-network/refs/heads/main/openapi/kyber-network-taker-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Kyber Network Authentication
name_suffix: Authentication
oauth_flows: []
overview: Kyber Network declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Kyber Network
provider_slug: kyber-network
scheme_count: 1
schemes:
- applies_to:
  - aggregator
  - limit-order
  - zaas
  evidence: '"KyberSwap APIs do not require authentication. There are no API keys, tokens, or secrets."'
  type: none
slug: kyber-network-authentication
source_filename: kyber-network-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://docs.kyberswap.com/developer-guide/start-here/rate-limits-and-client-id\ndocs: https://docs.kyberswap.com/developer-guide/start-here\nsummary: >-\n  KyberSwap's three public APIs require no authentication. There are no API\n  keys, tokens or secrets. Callers instead identify themselves with an\n  x-client-id header, which is an attribution and rate-limit-tiering mechanism\n  rather than a credential. Authorization is enforced on-chain: state-changing\n  actions are authorized by the user's own wallet signature (EIP-712 for limit\n  orders, EIP-2612/EIP-4494 permits for token approvals), never by the API.\nauthenticated: false\nschemes:\n- type: none\n  applies_to:\n  - aggregator\n  - limit-order\n  - zaas\n  evidence: >-\n    \"KyberSwap APIs do not require authentication. There are no API keys,\n    tokens, or secrets.\"\nclient_identification:\n- header: x-client-id\n  required: recommended on every request; documented\
  \ as required on the Aggregator\n    V1 route and route/build endpoints\n  value: your application or company name\n  purpose: rate-limit tiering and integration attribution\n  example: 'x-client-id: MyAwesomeApp'\n  grpc_equivalent: X-Client-ID\n  whitelisting: >-\n    Contact business@kyber.network (also published as bd@kyber.network in the\n    ZaaS proto contact block) to have a client id whitelisted for a higher rate\n    limit tier.\n- header: Origin\n  required: conditional\n  purpose: >-\n    The Limit Order API returns HTTP 401 when a required Origin header is absent\n    or invalid.\n  evidence: https://docs.kyberswap.com/developer-guide/limit-order-api/api-reference/error-code-reference\non_chain_authorization:\n- mechanism: EIP-712 typed-data signature\n  used_for: limit order creation, gasless cancellation, operator co-signing\n  notes: The signature must match the Maker's address; error 4004 (invalid signature)\n    and 4202 (invalid cancel signature) enforce this.\n- mechanism:\
  \ EIP-2612 permit (ERC-20)\n  used_for: gasless token approval prior to a swap or zap\n  docs: https://docs.kyberswap.com/developer-guide/aggregator-api/how-to-guides/permit\n- mechanism: EIP-4494 permit (NFT)\n  used_for: approving a liquidity position NFT for a zap in a single transaction\n  contract: KSZapRouterPositionPermit\ncustody: >-\n  No KyberSwap API or the first-party MCP server ever holds private keys. Build\n  endpoints return unsigned calldata for the caller's wallet to sign.\noauth: false\nscopes: not applicable — no OAuth surface\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kyber-network/refs/heads/main/authentication/kyber-network-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Crypto
- DeFi
- Blockchain
- Decentralized Exchange
- Token Swap
- Liquidity
- Trading
- Web3
- Ethereum
---
