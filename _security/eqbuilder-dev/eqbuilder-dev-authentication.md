---
anonymous_access: false
api_key_in: []
api_specs:
- filename: eqbuilder-dev-openapi.yml
  format: yaml
  label: EQ Scoring Platform API
  slug: eq-scoring-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eqbuilder-dev/refs/heads/main/openapi/eqbuilder-dev-openapi.yml
auth_types:
- none (anonymous free surface)
- x402 payment-as-authorization (header)
- apiKey-style secret token (header)
- ownership proof (query)
- apiKey (header) + cookie session (operator/admin only)
description: ''
kind: authentication
layout: security
mechanism_count: 7
method: searched
name: Eqbuilder Dev Authentication
name_suffix: Authentication
oauth_flows: []
overview: Marz Greta-Lock Network secures its APIs with none (anonymous free surface), x402 payment-as-authorization (header), apiKey-style secret token (header), ownership proof (query), and apiKey (header) + cookie session (operator/admin only) across 7 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Marz Greta-Lock Network
provider_slug: eqbuilder-dev
scheme_count: 7
schemes:
- applies_to:
  - POST /api/simulate
  - POST /api/rewrite
  - POST /api/stress-test
  - POST /api/progress
  - POST /api/training-dataset
  - POST /api/script-check
  - POST /api/duel
  - POST /api/roleplay
  - POST /api/coaching
  - POST /api/bundle
  - POST /api/storelayer/agent/payments/{quote_id}
  description: Payment IS the authorization. An unpaid request to a paid operation returns HTTP 402 with x402Version 2 payment requirements (accepts[] with scheme exact, network, maxAmountRequired, payTo, asset, maxTimeoutSeconds 120, extra.name/version). The client signs the selected requirement as EIP-712 typed data and retries the exact request once with PAYMENT-SIGNATURE; the facilitator submits the authorization (no ETH needed); success carries a PAYMENT-RESPONSE header/receipt. A malformed payment is rejected before money moves; an unused authorization expires at validBefore. Each transaction signature is accepted exactly once (409 on reuse).
  docs:
  - https://eqbuilder.dev/llms.txt
  - https://eqbuilder.dev/.well-known/x402.json
  - https://eqbuilder.dev/api/pricing
  - https://eqbuilder.dev/guides/x402-agent-payments-solana.html
  in: header
  name: x402Payment
  observed:
  - method: GET
    quote: '"x402Version": 2, "accepts": [{"scheme": "exact", "network": "eip155:8453", "maxAmountRequired": "50000", …}]'
    status: 402
    url: https://eqbuilder.dev/api/simulate
  parameter: PAYMENT-SIGNATURE
  protocol: 'x402 v2 (default rail: EIP-3009 USDC TransferWithAuthorization on Base eip155:8453; also Polygon, Arbitrum One, Avalanche C-Chain; Solana mainnet legacy)'
  type: x402
- applies_to: the same paid operations (X-PAYMENT is the declared header parameter on 13 of them)
  description: Legacy x402 payment header; also a finalized Solana transaction signature (tx_hash in the body) signed by wallet_address paying at least the tier fee in lamports to the treasury listed at /api/pricing. "Legacy SOL and X-PAYMENT clients remain compatible."
  docs:
  - https://eqbuilder.dev/llms.txt
  in: header
  name: legacyXPayment
  parameter: X-PAYMENT
  type: x402
- applies_to:
  - POST /api/simulate (basic tier)
  - POST /api/embed/check (via a company-owned host proxy)
  - GET /api/bundle/balance
  description: Secret prepaid-credit token minted by POST /api/bundle (x402) or POST /api/card/claim (card pack), shown exactly once. Redeems basic-tier credits with no per-call payment.
  how_obtained: POST /api/bundle → bundle_token; or GET /api/card/packs → POST /api/card/checkout {wallet_address, pack} → hosted checkout URL + claim_secret → POST /api/card/claim {checkout_id, claim_secret} → bundle_token
  in: header
  name: bundleToken
  observed:
  - quote: '"error": "Missing X-BUNDLE-TOKEN header."'
    status: 400
    url: https://eqbuilder.dev/api/bundle/balance
  parameter: X-BUNDLE-TOKEN
  rotation: null
  type: apiKey
- description: Any settled transaction hash the wallet itself paid with proves keyholder ownership for GET /api/wallet/{wallet_address}/statement; unknown or foreign hashes fail closed with 403. Operators may substitute X-Admin-Token.
  in: query
  name: walletStatementProof
  observed:
  - quote: '"error": "auth_tx_hash does not belong to this wallet''s settled history."'
    status: 403
    url: https://eqbuilder.dev/api/wallet/0x0000000000000000000000000000000000000000/statement?auth_tx_hash=abc
  parameter: auth_tx_hash
  type: ownership-proof
- description: Per-participant secret issued when opening or joining a role-play room; sent on POST /api/roleplay/turn and /api/roleplay/status. The joiner gets its own secret, never the opener's.
  docs:
  - https://eqbuilder.dev/llms.txt
  in: body
  name: roleplaySessionSecret
  parameter: session_secret
  type: apiKey
- description: Operator/admin bearer-style token for the /api/admin/*, /api/operator/*, ledger export, calibration review, profile vault, fleet plan, funnel and visits endpoints. Not available to API consumers.
  in: header
  name: adminToken
  observed:
  - quote: '"error": "Admin token required (X-Admin-Token header)."'
    status: 403
    url: https://eqbuilder.dev/api/admin/network-config
  parameter: X-Admin-Token
  type: apiKey
- description: 'POST /api/operator/login exchanges the operator key for a server-managed HttpOnly session cookie; GET /api/operator/session reports {"authorized": false} anonymously; POST /api/operator/logout clears it.'
  in: cookie
  name: operatorSession
  observed:
  - quote: '{"authorized": false}'
    status: 200
    url: https://eqbuilder.dev/api/operator/session
  parameter: HttpOnly operator session cookie (name not declared)
  type: cookie
slug: eqbuilder-dev-authentication
source_filename: eqbuilder-dev-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: searched\nsource: https://eqbuilder.dev/llms.txt (Start here, Permanent tool setup, Paid validation, Prepaid bundles, Card-paid\n  credit packs, Spend & usage statement), https://eqbuilder.dev/api/pricing, the OpenAPI header parameters (PAYMENT-SIGNATURE,\n  X-PAYMENT, X-BUNDLE-TOKEN, Idempotency-Key) and operation descriptions (X-Admin-Token, operator session), live\n  402/400/403 responses 2026-09-19\nsummary:\n  types:\n  - none (anonymous free surface)\n  - x402 payment-as-authorization (header)\n  - apiKey-style secret token (header)\n  - ownership proof (query)\n  - apiKey (header) + cookie session (operator/admin only)\n  oauth2: false\n  openid_connect: false\n  api_keys_or_accounts: false\n  public_surface: No account or API key exists anywhere. Profiles, pricing, stats, leaderboard, duel prompts, proof\n    cards, public results, certificates, price quotes (GET on paid paths → 402), the starter kit, every /.well-known\n    document\
  \ and the whole MCP server answer anonymously (observed live). Three free POST /api/score calls per caller\n    are keyed by the proxy-derived caller identity, not a credential.\n  note: The OpenAPI declares NO securitySchemes; derive-authentication.py therefore produced nothing and this profile\n    was assembled from the header parameters, operation descriptions, llms.txt and live responses. The overlay (overlays/eqbuilder-dev-openapi-overlay.yaml)\n    adds equivalent securitySchemes for consumers.\nschemes:\n- name: x402Payment\n  type: x402\n  in: header\n  parameter: PAYMENT-SIGNATURE\n  protocol: 'x402 v2 (default rail: EIP-3009 USDC TransferWithAuthorization on Base eip155:8453; also Polygon, Arbitrum\n    One, Avalanche C-Chain; Solana mainnet legacy)'\n  description: Payment IS the authorization. An unpaid request to a paid operation returns HTTP 402 with x402Version\n    2 payment requirements (accepts[] with scheme exact, network, maxAmountRequired, payTo, asset, maxTimeoutSeconds\n\
  \    120, extra.name/version). The client signs the selected requirement as EIP-712 typed data and retries the exact\n    request once with PAYMENT-SIGNATURE; the facilitator submits the authorization (no ETH needed); success carries\n    a PAYMENT-RESPONSE header/receipt. A malformed payment is rejected before money moves; an unused authorization\n    expires at validBefore. Each transaction signature is accepted exactly once (409 on reuse).\n  applies_to:\n  - POST /api/simulate\n  - POST /api/rewrite\n  - POST /api/stress-test\n  - POST /api/progress\n  - POST /api/training-dataset\n  - POST /api/script-check\n  - POST /api/duel\n  - POST /api/roleplay\n  - POST /api/coaching\n  - POST /api/bundle\n  - POST /api/storelayer/agent/payments/{quote_id}\n  observed:\n  - url: https://eqbuilder.dev/api/simulate\n    method: GET\n    status: 402\n    quote: '\"x402Version\": 2, \"accepts\": [{\"scheme\": \"exact\", \"network\": \"eip155:8453\", \"maxAmountRequired\": \"50000\",\n      …}]'\n\
  \  docs:\n  - https://eqbuilder.dev/llms.txt\n  - https://eqbuilder.dev/.well-known/x402.json\n  - https://eqbuilder.dev/api/pricing\n  - https://eqbuilder.dev/guides/x402-agent-payments-solana.html\n- name: legacyXPayment\n  type: x402\n  in: header\n  parameter: X-PAYMENT\n  description: Legacy x402 payment header; also a finalized Solana transaction signature (tx_hash in the body) signed\n    by wallet_address paying at least the tier fee in lamports to the treasury listed at /api/pricing. \"Legacy SOL\n    and X-PAYMENT clients remain compatible.\"\n  applies_to: the same paid operations (X-PAYMENT is the declared header parameter on 13 of them)\n  docs:\n  - https://eqbuilder.dev/llms.txt\n- name: bundleToken\n  type: apiKey\n  in: header\n  parameter: X-BUNDLE-TOKEN\n  description: Secret prepaid-credit token minted by POST /api/bundle (x402) or POST /api/card/claim (card pack),\n    shown exactly once. Redeems basic-tier credits with no per-call payment.\n  applies_to:\n  - POST\
  \ /api/simulate (basic tier)\n  - POST /api/embed/check (via a company-owned host proxy)\n  - GET /api/bundle/balance\n  how_obtained: POST /api/bundle → bundle_token; or GET /api/card/packs → POST /api/card/checkout {wallet_address,\n    pack} → hosted checkout URL + claim_secret → POST /api/card/claim {checkout_id, claim_secret} → bundle_token\n  rotation: null\n  observed:\n  - url: https://eqbuilder.dev/api/bundle/balance\n    status: 400\n    quote: '\"error\": \"Missing X-BUNDLE-TOKEN header.\"'\n- name: walletStatementProof\n  type: ownership-proof\n  in: query\n  parameter: auth_tx_hash\n  description: Any settled transaction hash the wallet itself paid with proves keyholder ownership for GET /api/wallet/{wallet_address}/statement;\n    unknown or foreign hashes fail closed with 403. Operators may substitute X-Admin-Token.\n  observed:\n  - url: https://eqbuilder.dev/api/wallet/0x0000000000000000000000000000000000000000/statement?auth_tx_hash=abc\n    status: 403\n    quote: '\"\
  error\": \"auth_tx_hash does not belong to this wallet''s settled history.\"'\n- name: roleplaySessionSecret\n  type: apiKey\n  in: body\n  parameter: session_secret\n  description: Per-participant secret issued when opening or joining a role-play room; sent on POST /api/roleplay/turn\n    and /api/roleplay/status. The joiner gets its own secret, never the opener's.\n  docs:\n  - https://eqbuilder.dev/llms.txt\n- name: adminToken\n  type: apiKey\n  in: header\n  parameter: X-Admin-Token\n  description: Operator/admin bearer-style token for the /api/admin/*, /api/operator/*, ledger export, calibration\n    review, profile vault, fleet plan, funnel and visits endpoints. Not available to API consumers.\n  observed:\n  - url: https://eqbuilder.dev/api/admin/network-config\n    status: 403\n    quote: '\"error\": \"Admin token required (X-Admin-Token header).\"'\n- name: operatorSession\n  type: cookie\n  in: cookie\n  parameter: HttpOnly operator session cookie (name not declared)\n  description:\
  \ 'POST /api/operator/login exchanges the operator key for a server-managed HttpOnly session cookie;\n    GET /api/operator/session reports {\"authorized\": false} anonymously; POST /api/operator/logout clears it.'\n  observed:\n  - url: https://eqbuilder.dev/api/operator/session\n    status: 200\n    quote: '{\"authorized\": false}'\nconsent_gates_on_the_free_tier:\n  data_consent: must be true on every free POST /api/score (400 data_consent_required otherwise, no round consumed)\n  wishlist_required: one POST /api/wishlist before the third free score (400 wishlist_required otherwise)\n  source: optional campaign attribution; unknown values are rejected before a round is consumed\ndocs:\n- https://eqbuilder.dev/llms.txt\n- https://eqbuilder.dev/api/pricing\n- https://eqbuilder.dev/.well-known/x402.json\n- https://eqbuilder.dev/api/starter-kit/PAY_AND_SCORE.md\n- https://eqbuilder.dev/guides/permanent-agent-tool-setup.html\nnotes: '\"The platform holds no private keys.\" The recommended\
  \ posture (llms.txt) is a dedicated burner wallet funded\n  with USDC on Base that the SDK signs with; the SDKs never auto-replay a paid authorization after a timeout. MCP\n  is anonymous and read-only; RFC 9728 protected-resource metadata is not published (404) and is not needed.'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/eqbuilder-dev/refs/heads/main/authentication/eqbuilder-dev-authentication.yml
summary_line: none (anonymous free surface)/x402 payment-as-authorization (header)/apiKey-style secret token (header)/ownership proof (query)/apiKey (header) + cookie session (operator/admin only) · 7 schemes
tags:
- Company
- AI Agents
- Agent Evaluation
- Benchmarking
- Text Analysis
- Emotional Intelligence
- Conversational AI
- x402
- Agentic Payments
- MCP
- A2A
- Developer Tools
---
