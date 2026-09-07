---
anonymous_access: true
api_key_in: []
api_specs:
- filename: ontopx402-bidding-api-openapi.yml
  format: yaml
  label: OnTopX402 Bidding API
  slug: ontopx402-bidding-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ontopx402/refs/heads/main/openapi/ontopx402-bidding-api-openapi.yml
- filename: ontopx402-leaderboard-api-openapi.yml
  format: yaml
  label: OnTopX402 Leaderboard API
  slug: ontopx402-leaderboard-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ontopx402/refs/heads/main/openapi/ontopx402-leaderboard-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Ontopx402 Authentication
name_suffix: Authentication
oauth_flows: []
overview: OnTopX402 declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: OnTopX402
provider_slug: ontopx402
scheme_count: 2
schemes:
- applies_to:
  - api_leaderboard_api_leaderboard_get
  - api_entry_api_entry_get
  description: GET /api/leaderboard and GET /api/entry are free and need no key. Free reads are rate limited per address (429).
  name: none (anonymous reads)
  type: none
- applies_to:
  - api_bid_api_bid_post
  description: POST /api/bid with no payment header answers 402 carrying x402Version 2 payment requirements priced at the caller-named amount, payable in USDC on Base (eip155:8453, facilitator https://api.cdp.coinbase.com/platform/v2/x402) or Solana. The caller pays and resends the identical request with the X-PAYMENT header; the settlement receipt returns in X-PAYMENT-RESPONSE. A settled transaction is never credited twice.
  name: x402 payment (X-PAYMENT header)
  type: x402
slug: ontopx402-authentication
source_filename: ontopx402-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-03'\nmethod: searched\nsource: https://ontopx402.com/llms.txt\ndocs: https://ontopx402.com/llms.txt\nnote: >-\n  There are no accounts, API keys, OAuth flows or cards, by design — \"the payment is\n  the account.\" The OpenAPI declares no securitySchemes. Reads are anonymous; the\n  only write is gated by an x402 v2 payment challenge instead of credentials.\nschemes:\n- name: none (anonymous reads)\n  type: none\n  applies_to:\n  - api_leaderboard_api_leaderboard_get\n  - api_entry_api_entry_get\n  description: GET /api/leaderboard and GET /api/entry are free and need no key. Free reads are rate limited per address (429).\n- name: x402 payment (X-PAYMENT header)\n  type: x402\n  applies_to:\n  - api_bid_api_bid_post\n  description: >-\n    POST /api/bid with no payment header answers 402 carrying x402Version 2 payment\n    requirements priced at the caller-named amount, payable in USDC on Base\n    (eip155:8453, facilitator https://api.cdp.coinbase.com/platform/v2/x402)\
  \ or\n    Solana. The caller pays and resends the identical request with the X-PAYMENT\n    header; the settlement receipt returns in X-PAYMENT-RESPONSE. A settled\n    transaction is never credited twice.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ontopx402/refs/heads/main/authentication/ontopx402-authentication.yml
summary_line: 2 schemes
tags:
- x402
- USDC
- Agent Payments
- paid-placement
- Leaderboard
---
