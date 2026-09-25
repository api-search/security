---
anonymous_access: true
api_key_in: []
api_specs:
- filename: dualregistry-dev-openapi.yml
  format: yaml
  label: Scro Orphan Desk Intent Echo API
  slug: intent-echo-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dualregistry-dev/refs/heads/main/openapi/dualregistry-dev-openapi.yml
auth_types:
- none
- x402-payment-proof
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Dualregistry Dev Authentication
name_suffix: Authentication
oauth_flows: []
overview: Scro Orphan Desk secures its APIs with none and x402-payment-proof across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Scro Orphan Desk
provider_slug: dualregistry-dev
scheme_count: 3
schemes:
- applies_to:
  - listEchoes
  - getStats
  - redeemEcho with ?preview=1 or on a non-open echo
  - quoteFee exploratory (firm false/omitted)
  - GET /fill_hint.json, /PROMO.json, /ORPHANDUST.json, /PRODUCT.json, /SPOTLIGHT.json, /DIRECTORY.json, /MIRROR.json, /ACROSS.json
  - GET /api/feedback (self-description)
  declared_in_spec: implicitly — no securitySchemes, no security requirement on any of the 7 operations
  name: none
  sources:
  - well-known/dualregistry-dev-ai-plugin.json auth.type none
  - https://dualregistry.dev/llms.txt
  type: none
- applies_to:
  - redeemEcho on an open echo (GET /api/echo?echo_id=, GET /*.echo.json)
  - quoteFee firm accept (402 invoice with quote_id)
  - buyOrphanDustCredits (402 for the SKU)
  challenge:
    body: application/json type x402_payment_required with accepts[] (scheme exact, network eip155:8453 | base, USDC asset 0x8335…2913, maxAmountRequired in 6-decimal units, maxTimeoutSeconds 600) and accepted[] (USDC/Base preferred; USDT/BSC; USDC and USDT on Ethereum)
    headers_observed:
    - 'PAYMENT-REQUIRED: <base64 JSON {x402Version: 1, accepts[]}>'
    - 'x-payment-required: true'
    - 'x402-asset: USDC'
    - 'x402-network: eip155:8453'
    - 'x402-pay-to: 0x459cF7359e37B45A0d2a2479656cD96cdA9F7dBb'
    - 'x402-price: 0.50'
    status: 402
  declared_in_spec: as the 402 responses on redeemEcho, quoteFee and buyOrphanDustCredits; not a securityScheme (OpenAPI has no type for it)
  name: x402-payment-proof
  proof:
    binding_headers:
    - X-QUOTE-ID — binds a firm quote (final_usdc) to the unlock; quote TTL 20 minutes
    - X-CREDIT-TOKEN or ?credit_token=odc_… — spends one OrphanDust unlock credit instead of a per-echo fee
    - X-BOND-WAIVER — bond waiver id (bond is 0; kept for compatibility)
    headers:
    - X-PAYMENT-TX (0x… transaction hash)
    - X-PAYMENT-CHAIN (base|bsc|ethereum)
    - X-PAYMENT-ASSET (USDC|USDT, optional)
    - X-PAYMENT-AMOUNT (optional)
    - X-PAYMENT-PAYER (optional)
    - X-PAYMENT (generic x402 header, allowed by CORS)
    - PAYMENT-TX / PAYMENT-CHAIN (unprefixed aliases, allowed by CORS)
    manual_path: POST /api/settle_fee {quote_id|echo_id, tx_hash, chain, amount_usdc|amount, asset?, payer?} -> receipt (same RPC verification)
    query_equivalents:
    - tx_hash
    - chain
    - asset
    - amount
    verification_verbatim: Server RPC-verifies Transfer to fee wallet (fail-closed) then auto settle_fee.
  receive_wallet: 397420814417713553602400438560121680136127872443
  receive_wallet_note: One EVM address on Ethereum (eip155:1), Base (eip155:8453) and BSC (eip155:56); published in every JSON document, the x402 discovery file and the agent card's agentWallet services.
  sources:
  - https://dualregistry.dev/llms.txt
  - https://dualregistry.dev/.well-known/x402
  - live 402 on GET /api/echo?echo_id=echo_a25e7551ed53c3018600f816 (2026-09-19)
  - https://dualregistry.dev/AGENT.md step 6
  standard: x402 v1
  type: payment
- applies_to:
  - POST /api/orphandust/unlock {echo_id, credit_token}
  - GET /api/echo?echo_id=…&credit_token=odc_…
  declared_in_spec: false
  how: 'Buy a SKU at POST /api/orphandust/buy (402 -> pay 0.50 USDC on Base -> retry with X-PAYMENT-TX + X-PAYMENT-CHAIN) and receive credits; a credit_token (prefix odc_) spends one credit per unlock. Refusals: invalid_credit_token, credit_expired, credit_exhausted (source orphandust.js). Credit TTL not published.'
  name: orphandust-credit-token
  sources:
  - https://dualregistry.dev/ORPHANDUST.json
  - live 402 on GET /api/orphandust/buy
  - GET /api/orphandust/unlock -> 405 note
  type: bearer-like-credit
slug: dualregistry-dev-authentication
source_filename: dualregistry-dev-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: searched\nsource: >-\n  openapi/dualregistry-dev-openapi.yml (no securitySchemes, no security — derive-authentication.py\n  produced nothing), upgraded from https://dualregistry.dev/llms.txt (\"Per-Echo GET (x402 paywall)\",\n  \"OBO→pay\"), https://dualregistry.dev/AGENT.md, the agent card's x402_paywall block,\n  well-known/dualregistry-dev-ai-plugin.json (auth {type: none}), well-known/dualregistry-dev-x402.json,\n  the live 402 responses on /api/echo and /api/orphandust/buy (headers + body), the CORS\n  Access-Control-Allow-Headers list observed on every /api/* response, and the provider's\n  vercel.json / verify_payment.js in github.com/manhatton31-svg/orphan-desk-source.\ndocs: https://dualregistry.dev/llms.txt\nchecked: '2026-09-19'\nsummary:\n  types: [none, x402-payment-proof]\n  model: no-identity-payment-is-the-gate\n  model_note: >-\n    There is no authentication: no API key, no token, no OAuth, no signup, no account. The\n    ai-plugin\
  \ manifest says auth {type: none} and the OpenAPI declares no securitySchemes. Access\n    control is economic — the free surfaces (index, stats, fill_hint, catalogs, previews,\n    exploratory quotes, non-open echoes) answer 200 to anyone, and the paid surface (an open echo's\n    unsealed legs, an OrphanDust credit) answers HTTP 402 with an x402 v1 invoice until the same\n    request is retried carrying proof of an on-chain stablecoin transfer to the desk's receive\n    wallet, which the server verifies against the chain (\"fail-closed\") before serving. Three proof\n    forms exist: payment-proof headers (or the equivalent query parameters), a quote_id that binds\n    a negotiated price, and a credit_token bought through OrphanDust.\n  oauth2: false\n  openid_connect: false\n  mtls: false\n  api_key_in: []\n  scopes: false\n  scopes_note: 'No scopes/ artifact and no OAuthScopes pointer: nothing declares oauth2 or any permission model.'\nschemes:\n- name: none\n  type: none\n  declared_in_spec:\
  \ 'implicitly — no securitySchemes, no security requirement on any of the 7 operations'\n  applies_to: [listEchoes, getStats, 'redeemEcho with ?preview=1 or on a non-open echo', 'quoteFee exploratory (firm false/omitted)', 'GET /fill_hint.json, /PROMO.json, /ORPHANDUST.json, /PRODUCT.json, /SPOTLIGHT.json, /DIRECTORY.json, /MIRROR.json, /ACROSS.json', 'GET /api/feedback (self-description)']\n  sources: ['well-known/dualregistry-dev-ai-plugin.json auth.type none', 'https://dualregistry.dev/llms.txt']\n- name: x402-payment-proof\n  type: payment\n  standard: x402 v1\n  declared_in_spec: 'as the 402 responses on redeemEcho, quoteFee and buyOrphanDustCredits; not a securityScheme (OpenAPI has no type for it)'\n  applies_to: ['redeemEcho on an open echo (GET /api/echo?echo_id=, GET /*.echo.json)', 'quoteFee firm accept (402 invoice with quote_id)', 'buyOrphanDustCredits (402 for the SKU)']\n  challenge:\n    status: 402\n    headers_observed: ['PAYMENT-REQUIRED: <base64 JSON {x402Version: 1,\
  \ accepts[]}>', 'x-payment-required: true', 'x402-asset: USDC', 'x402-network: eip155:8453', 'x402-pay-to: 0x459cF7359e37B45A0d2a2479656cD96cdA9F7dBb', 'x402-price: 0.50']\n    body: 'application/json type x402_payment_required with accepts[] (scheme exact, network eip155:8453 | base, USDC asset 0x8335…2913, maxAmountRequired in 6-decimal units, maxTimeoutSeconds 600) and accepted[] (USDC/Base preferred; USDT/BSC; USDC and USDT on Ethereum)'\n  proof:\n    headers: ['X-PAYMENT-TX (0x… transaction hash)', 'X-PAYMENT-CHAIN (base|bsc|ethereum)', 'X-PAYMENT-ASSET (USDC|USDT, optional)', 'X-PAYMENT-AMOUNT (optional)', 'X-PAYMENT-PAYER (optional)', 'X-PAYMENT (generic x402 header, allowed by CORS)', 'PAYMENT-TX / PAYMENT-CHAIN (unprefixed aliases, allowed by CORS)']\n    query_equivalents: [tx_hash, chain, asset, amount]\n    binding_headers: ['X-QUOTE-ID — binds a firm quote (final_usdc) to the unlock; quote TTL 20 minutes', 'X-CREDIT-TOKEN or ?credit_token=odc_… — spends one OrphanDust unlock\
  \ credit instead of a per-echo fee', 'X-BOND-WAIVER — bond waiver id (bond is 0; kept for compatibility)']\n    verification_verbatim: 'Server RPC-verifies Transfer to fee wallet (fail-closed) then auto settle_fee.'\n    manual_path: 'POST /api/settle_fee {quote_id|echo_id, tx_hash, chain, amount_usdc|amount, asset?, payer?} -> receipt (same RPC verification)'\n  receive_wallet: 0x459cF7359e37B45A0d2a2479656cD96cdA9F7dBb\n  receive_wallet_note: 'One EVM address on Ethereum (eip155:1), Base (eip155:8453) and BSC (eip155:56); published in every JSON document, the x402 discovery file and the agent card''s agentWallet services.'\n  sources: ['https://dualregistry.dev/llms.txt', 'https://dualregistry.dev/.well-known/x402', 'live 402 on GET /api/echo?echo_id=echo_a25e7551ed53c3018600f816 (2026-09-19)', 'https://dualregistry.dev/AGENT.md step 6']\n- name: orphandust-credit-token\n  type: bearer-like-credit\n  declared_in_spec: false\n  applies_to: ['POST /api/orphandust/unlock {echo_id, credit_token}',\
  \ 'GET /api/echo?echo_id=…&credit_token=odc_…']\n  how: 'Buy a SKU at POST /api/orphandust/buy (402 -> pay 0.50 USDC on Base -> retry with X-PAYMENT-TX + X-PAYMENT-CHAIN) and receive credits; a credit_token (prefix odc_) spends one credit per unlock. Refusals: invalid_credit_token, credit_expired, credit_exhausted (source orphandust.js). Credit TTL not published.'\n  sources: ['https://dualregistry.dev/ORPHANDUST.json', 'live 402 on GET /api/orphandust/buy', 'GET /api/orphandust/unlock -> 405 note']\nagent_guidance: >-\n  Do not look for a key. Read /index.json free, preview an echo free with ?preview=1, quote free\n  with firm omitted, and only when you intend to pay follow the 402: pay the accepts[] amount in\n  USDC on Base to payTo, then repeat the SAME request with X-PAYMENT-TX and X-PAYMENT-CHAIN. The\n  payment is an irreversible on-chain transfer — see conventions/ (reversibility: none).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dualregistry-dev/refs/heads/main/authentication/dualregistry-dev-authentication.yml
summary_line: none/x402-payment-proof · 3 schemes
tags:
- AI Agents
- x402
- A2A
- DeFi
- Crypto
- Stablecoins
- Payments
- Intent Trading
- Machine Economy
- Agent-Native
---
