---
anonymous_access: true
api_key_in:
- header
api_specs:
- filename: mercury-hq-com-x402-storefront-openapi.yml
  format: yaml
  label: MERCURY x402 Storefront API
  slug: mercury-x402-storefront-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mercury-hq-com/refs/heads/main/openapi/mercury-hq-com-x402-storefront-openapi.yml
auth_types:
- x402-payment
- apiKey
- none
description: 'MERCURY has no credential to obtain before calling: the contract is payment-as-authorization. An unpaid request to any paid /buy/* route is answered HTTP 402 with an x402 v1 challenge and succeeds when replayed with an X-PAYMENT header carrying a signed USDC payment for the exact amount. As an alternative "door" the same routes accept a Mercury API key as a Bearer token - a free sandbox key (mk_test_, 100 credits) minted with one anonymous POST, or a Stripe-billed live key (mk_live_). The hosted MCP server gates tools/call on that same key while leaving initialize and tools/list open; the stdio MCP package instead pays over x402 from a wallet private key. Discovery, verification and the A2A free preview are anonymous. No OAuth 2.0, OpenID Connect, mutual TLS or per-user identity exists anywhere, and the OpenAPI declares none of this - its securitySchemes are absent, which is the gap an agent reading only the spec would hit. derive-authentication.py therefore produced no baseline;
  this profile is written from the docs and the wire.'
kind: authentication
layout: security
mechanism_count: 4
method: searched
name: Mercury Hq Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: MERCURY secures its APIs with x402-payment, apiKey, and none across 5 declared security schemes, as derived from its OpenAPI definitions.
provider_name: MERCURY
provider_slug: mercury-hq-com
scheme_count: 5
schemes:
- description: 'Unpaid call -> 402 application/json {x402Version: 1, error: "X-PAYMENT header is required", accepts: [{scheme: exact, network: base, maxAmountRequired: "<USDC base units, 6 decimals>", resource, payTo: 0xe10B9d44e72A29B9c19da02981FFCd875308e3C1, maxTimeoutSeconds: 60, asset: 0x833589fCD6eDb6E08f4c7C32D4f71b54bdA02913, outputSchema, extra: {name: USD Coin, version: 2}}]}. The client signs an EIP-3009 style USDC transfer for the amount with any x402 client (the docs show x402-fetch wrapFetchWithPayment with a viem account; x402-axios also named) and replays the request with the X-PAYMENT header; settlement goes through the Coinbase CDP facilitator (https://api.cdp.coinbase.com/platform/v2/x402) on Base mainnet (eip155:8453), testnet false. The price is declared per operation in x-payment-info / x-x402 and in /catalog and /.well-known/x402; the challenge carries the same number. No account, no key, no signup. /buy/fetch offers three accepts tiers (3000 / 6000 / 12000 base units).
    The agent card expresses this as securitySchemes.x402 {type: x402, scheme: exact, network: eip155:8453, asset: USDC} with security [{x402: []}].'
  name: x402
  probe:
    maxAmountRequired: '3000'
    method: GET (unpaid)
    status: 402
    url: https://network.mercury-hq.com/buy/fetch?url=https://example.com
    x402Version: 1
  sources:
  - openapi/mercury-hq-com-x402-storefront-openapi.yml
  - a2a/mercury-hq-com-agent-card.json
  - well-known/mercury-hq-com-x402.json
  surface: all 18 paid /buy/* operations (buy_web_fetch ... buy_cited_redirect); the A2A card's declared scheme for the paid result
  type: payment (x402)
- description: '"Prefer a prepaid key? The same routes accept Authorization: Bearer mk_live_... - issue one at /developers." Issuance: POST /api/dev/keys?live=false&label=... (anonymous) returns 201 {ok, key, keyId, env, tail, usage, save_it}; the raw key is shown ONCE and only its sha256 plus a 4-character tail are stored; issuance is capped at 20 keys per IP per hour. Sandbox keys carry 100 credits at 5 requests per minute; live keys are enabled by a Stripe Checkout subscription (Pro $29 / Business $199 / Enterprise $1500 per month) or a one-time credit top-up, metered at 1 credit = $0.001 per call. Balance: GET /api/dev/balance (401 without a key, observed). The /university hub labels the paid tier "Building" while /developers and /pricing describe it as live - recorded as stated.'
  in: header
  key_prefixes:
  - mk_test_
  - mk_live_
  name: mercuryApiKey
  parameter: 'Authorization: Bearer <key>'
  probe:
    credentials: none
    method: GET
    status: 401
    url: https://network.mercury-hq.com/api/dev/balance
  sources:
  - https://network.mercury-hq.com/developers
  - https://network.mercury-hq.com/university/developers
  - https://network.mercury-hq.com/pricing
  surface: the same 18 /buy/* routes; POST /mcp tools/call; the key-management routes /api/dev/keys, /api/dev/balance, /api/dev/topup (outside the OpenAPI)
  type: apiKey
- description: 'initialize and tools/list answered without credentials (18 tools with inputSchema); the server descriptor and initialize.instructions state that tools/call needs Authorization: Bearer mk_.... No OAuth: /.well-known/oauth-protected-resource and /.well-known/oauth-authorization-server are 404 on the MCP host, so there is no RFC 9728 / dynamic client registration path - a client must hold a key minted out of band (or via the anonymous POST /api/dev/keys).'
  name: mcpRemote
  probe:
    credentials: none
    method: POST tools/list
    status: 200
    url: https://network.mercury-hq.com/mcp
  sources:
  - mcp/mercury-hq-com-mcp.yml
  surface: POST https://network.mercury-hq.com/mcp
  type: apiKey (same Mercury key) over MCP
- description: The stdio server reads MERCURY_PRIVATE_KEY (a funded Base-mainnet wallet) and pays each tool call over x402 with x402-fetch; no Mercury key. mercury_catalog and mercury_verify work without a wallet (npm README; not run here).
  name: mcpStdioWallet
  sources:
  - packages/mercury-hq-com-packages.yml
  surface: npx -y mercury-x402-mcp
  type: wallet-key (x402 via environment)
- description: Free, keyless discovery and receipt verification. The receipt verification needs no MERCURY call at all (offline EIP-191 ecrecover against the pinned key at /.well-known/mercury-attestation).
  name: anonymous
  sources:
  - https://network.mercury-hq.com/llms.txt
  surface: GET /catalog, /.well-known/x402, /x402/discovery, /openapi.json, /llms.txt, /manifest, /health, /vs, /market, /scoreboard, /proof, /buy/signal ($0), /x402/attestation/sample, /x402/verify, POST /verify, POST /a2a message/send (free preview), GET /terms, /privacy, /trust
  type: none
slug: mercury-hq-com-authentication
source_filename: mercury-hq-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: searched\nsource:\n- openapi/mercury-hq-com-x402-storefront-openapi.yml (NO securitySchemes and no security requirements; per-operation x-payment-info / x-x402 declare the payment terms instead)\n- live unpaid GET https://network.mercury-hq.com/buy/fetch?url=https://example.com -> 402 {x402Version 1, error \"X-PAYMENT header is required\", accepts[]}\n- https://network.mercury-hq.com/developers and /university/developers (API-key rail: mk_test_/mk_live_ Bearer keys, POST /api/dev/keys)\n- \"https://network.mercury-hq.com/.well-known/agent-card.json (securitySchemes.x402, security [{x402: []}])\"\n- POST https://network.mercury-hq.com/mcp initialize / tools/list (anonymous) and GET /mcp descriptor (\"tools/call needs a Mercury API key (Authorization: Bearer mk_…)\")\n- https://registry.npmjs.org/mercury-x402-mcp (stdio server pays from MERCURY_PRIVATE_KEY)\n- GET https://network.mercury-hq.com/api/dev/balance -> 401 without a key\ndocs: https://network.mercury-hq.com/university/developers\n\
  description: >-\n  MERCURY has no credential to obtain before calling: the contract is payment-as-authorization. An unpaid\n  request to any paid /buy/* route is answered HTTP 402 with an x402 v1 challenge and succeeds when\n  replayed with an X-PAYMENT header carrying a signed USDC payment for the exact amount. As an\n  alternative \"door\" the same routes accept a Mercury API key as a Bearer token - a free sandbox key\n  (mk_test_, 100 credits) minted with one anonymous POST, or a Stripe-billed live key (mk_live_). The\n  hosted MCP server gates tools/call on that same key while leaving initialize and tools/list open; the\n  stdio MCP package instead pays over x402 from a wallet private key. Discovery, verification and the A2A\n  free preview are anonymous. No OAuth 2.0, OpenID Connect, mutual TLS or per-user identity exists\n  anywhere, and the OpenAPI declares none of this - its securitySchemes are absent, which is the gap an\n  agent reading only the spec would hit. derive-authentication.py\
  \ therefore produced no baseline; this\n  profile is written from the docs and the wire.\nsummary:\n  types: [x402-payment, apiKey, none]\n  api_key_in: [header]\n  api_key_header: 'Authorization: Bearer mk_test_... | mk_live_...'\n  oauth2_flows: []\n  openapi_security_schemes_declared: 0\nschemes:\n- name: x402\n  type: payment (x402)\n  surface: all 18 paid /buy/* operations (buy_web_fetch ... buy_cited_redirect); the A2A card's declared scheme for the paid result\n  description: >-\n    Unpaid call -> 402 application/json {x402Version: 1, error: \"X-PAYMENT header is required\", accepts:\n    [{scheme: exact, network: base, maxAmountRequired: \"<USDC base units, 6 decimals>\", resource, payTo:\n    0xe10B9d44e72A29B9c19da02981FFCd875308e3C1, maxTimeoutSeconds: 60, asset:\n    0x833589fCD6eDb6E08f4c7C32D4f71b54bdA02913, outputSchema, extra: {name: USD Coin, version: 2}}]}. The\n    client signs an EIP-3009 style USDC transfer for the amount with any x402 client (the docs show\n    x402-fetch\
  \ wrapFetchWithPayment with a viem account; x402-axios also named) and replays the request\n    with the X-PAYMENT header; settlement goes through the Coinbase CDP facilitator\n    (https://api.cdp.coinbase.com/platform/v2/x402) on Base mainnet (eip155:8453), testnet false. The\n    price is declared per operation in x-payment-info / x-x402 and in /catalog and /.well-known/x402; the\n    challenge carries the same number. No account, no key, no signup. /buy/fetch offers three accepts\n    tiers (3000 / 6000 / 12000 base units). The agent card expresses this as securitySchemes.x402 {type:\n    x402, scheme: exact, network: eip155:8453, asset: USDC} with security [{x402: []}].\n  sources: [openapi/mercury-hq-com-x402-storefront-openapi.yml, a2a/mercury-hq-com-agent-card.json, well-known/mercury-hq-com-x402.json]\n  probe: {url: 'https://network.mercury-hq.com/buy/fetch?url=https://example.com', method: 'GET (unpaid)', status: 402, x402Version: 1, maxAmountRequired: '3000'}\n- name: mercuryApiKey\n\
  \  type: apiKey\n  in: header\n  parameter: 'Authorization: Bearer <key>'\n  key_prefixes: [mk_test_, mk_live_]\n  surface: the same 18 /buy/* routes; POST /mcp tools/call; the key-management routes /api/dev/keys, /api/dev/balance, /api/dev/topup (outside the OpenAPI)\n  description: >-\n    \"Prefer a prepaid key? The same routes accept Authorization: Bearer mk_live_... - issue one at\n    /developers.\" Issuance: POST /api/dev/keys?live=false&label=... (anonymous) returns 201 {ok, key, keyId,\n    env, tail, usage, save_it}; the raw key is shown ONCE and only its sha256 plus a 4-character tail are\n    stored; issuance is capped at 20 keys per IP per hour. Sandbox keys carry 100 credits at 5 requests\n    per minute; live keys are enabled by a Stripe Checkout subscription (Pro $29 / Business $199 /\n    Enterprise $1500 per month) or a one-time credit top-up, metered at 1 credit = $0.001 per call.\n    Balance: GET /api/dev/balance (401 without a key, observed). The /university hub labels\
  \ the paid tier\n    \"Building\" while /developers and /pricing describe it as live - recorded as stated.\n  sources: [https://network.mercury-hq.com/developers, https://network.mercury-hq.com/university/developers, https://network.mercury-hq.com/pricing]\n  probe: {url: 'https://network.mercury-hq.com/api/dev/balance', method: GET, status: 401, credentials: none}\n- name: mcpRemote\n  type: apiKey (same Mercury key) over MCP\n  surface: POST https://network.mercury-hq.com/mcp\n  description: >-\n    initialize and tools/list answered without credentials (18 tools with inputSchema); the server\n    descriptor and initialize.instructions state that tools/call needs Authorization: Bearer mk_.... No\n    OAuth: /.well-known/oauth-protected-resource and /.well-known/oauth-authorization-server are 404 on\n    the MCP host, so there is no RFC 9728 / dynamic client registration path - a client must hold a key\n    minted out of band (or via the anonymous POST /api/dev/keys).\n  sources: [mcp/mercury-hq-com-mcp.yml]\n\
  \  probe: {url: 'https://network.mercury-hq.com/mcp', method: 'POST tools/list', status: 200, credentials: none}\n- name: mcpStdioWallet\n  type: wallet-key (x402 via environment)\n  surface: npx -y mercury-x402-mcp\n  description: 'The stdio server reads MERCURY_PRIVATE_KEY (a funded Base-mainnet wallet) and pays each tool call over x402 with x402-fetch; no Mercury key. mercury_catalog and mercury_verify work without a wallet (npm README; not run here).'\n  sources: [packages/mercury-hq-com-packages.yml]\n- name: anonymous\n  type: none\n  surface: GET /catalog, /.well-known/x402, /x402/discovery, /openapi.json, /llms.txt, /manifest, /health, /vs, /market, /scoreboard, /proof, /buy/signal ($0), /x402/attestation/sample, /x402/verify, POST /verify, POST /a2a message/send (free preview), GET /terms, /privacy, /trust\n  description: Free, keyless discovery and receipt verification. The receipt verification needs no MERCURY call at all (offline EIP-191 ecrecover against the pinned key at\
  \ /.well-known/mercury-attestation).\n  sources: [https://network.mercury-hq.com/llms.txt]\nreceipt_verification:\n  note: not an authentication scheme for callers but the trust anchor for results\n  signer: '0xACB40253BD71Bb9a5d491b2c6EFF755F2A33Fc75'\n  key_pin: https://network.mercury-hq.com/.well-known/mercury-attestation\n  alg: EIP-191-personal_sign over \"mercury-x402:fetch-attestation:v1\\nurl=...\\nstatus=...\\nsha256=...\\nfetchedAt=...\\nnonce=...\"\nscopes: none (no OAuth; no scope surface - scopes/ deliberately not written)\ncross_links:\n  conventions: conventions/mercury-hq-com-conventions.yml\n  plans: plans/mercury-hq-com-plans-pricing.yml\n  rate_limits: rate-limits/mercury-hq-com-rate-limits.yml\n  mcp: mcp/mercury-hq-com-mcp.yml\n  agent_card: a2a/mercury-hq-com-a2a.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mercury-hq-com/refs/heads/main/authentication/mercury-hq-com-authentication.yml
summary_line: x402-payment/apiKey/none · 5 schemes
tags:
- Company
- Agents
- A2A
- MCP
- x402
- HTTP 402
- Machine Payments
- Web Data
- Web Scraping
- Data Extraction
- Provenance
- Stablecoins
- Artificial Intelligence
---
