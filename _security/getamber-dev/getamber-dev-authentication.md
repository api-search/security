---
anonymous_access: false
api_key_in: []
auth_types:
- apiKey
- x402-payment
- wallet-signature
- share-token
- session-token
description: ''
kind: authentication
layout: security
mechanism_count: 5
method: searched
name: Getamber Dev Authentication
name_suffix: Authentication
oauth_flows: []
overview: Ambr secures its APIs with apiKey, x402-payment, wallet-signature, share-token, and session-token across 5 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Ambr
provider_slug: getamber-dev
scheme_count: 5
schemes:
- agent_card_declaration: '{"type":"apiKey","in":"header","name":"X-API-Key","description":"Pre-registered API key for businesses with credit-based access"}'
  applies_to: POST /v1/contracts (or x402), GET /v1/contracts/:id (or share token), POST /v1/contracts/:id/revoke (or wallet signature), POST /v1/dashboard, POST /v1/identity/verify (or share token), /v1/delegations; MCP state-changing tools (ambr_create_contract, ambr_agent_handshake)
  header: X-API-Key
  in: header
  issuance: 'POST /api/v1/keys or the /activate page: enter an email, click a one-time magic link (expires in 30 minutes) — that verifies the address and reveals the key. Developer tier is free (25 credits); paid tiers verify a Base L2 USDC tx_hash or Stripe checkout.'
  key_prefix: 'amb_ (docs page: response.api_key → "amb_..."); the developers page''s /v1/keys snippet shows "ambr_live_..." — the two pages disagree and the docs page is the newer wording'
  name: apiKey
  observed: GET /api/v1/contracts without a key -> 401 {"error":"unauthorized","message":"Valid API key required via X-API-Key header, or provide ?wallet= with signature headers"}
  storage: Keys are stored as SHA-256 hashes and shown once; a lost key is replaced by requesting a new link (docs, privacy policy §1).
  type: apiKey
- agent_card_declaration: '{"type":"http","scheme":"x402","description":"Pay-per-contract via USDC on Base L2. Send payment, include tx hash in X-Payment header."}'
  applies_to:
  - POST /v1/contracts
  - MCP ambr_create_contract
  description: 'Pay-per-contract instead of an API key: the client pays on Base L2 (USDC, USDbC, DAI, ETH, WETH, cbETH, cbBTC) and retries with the transaction hash in X-Payment. Unpaid paid-endpoint calls receive HTTP 402 with x402 payment instructions (REST) or JSON-RPC -32001 "Payment required" with the same payload (MCP). Observed live 2026-09-19 on ambr_create_contract: version "2", price 500000, currency USD, chain base, recipient address, accepts [exact, overpay], accepted_tokens[7], pricing per template. "This enables fully autonomous agent-to-agent commerce without pre-registration." (docs)'
  header: X-Payment
  name: x402
  scheme: x402
  type: http
- applies_to:
  - POST /v1/contracts/:id/sign
  - POST /v1/contracts/:id/handshake
  - POST /v1/contracts/:id/revoke
  - POST /v1/contracts/:id/wallet-auth
  - POST /v1/dashboard/wallet-auth
  description: Counterparties and principals authenticate by signing a challenge message with an EVM wallet; the body carries wallet_address, signature and message. Used to sign (message must contain "I am signing Ambr contract <id>" and the SHA-256 hash), to revoke ("I revoke Ambr contract <id> with hash <sha256>"), for handshake approval, and on POST /v1/contracts/:id/wallet-auth which returns a short-lived JWT access_token for contract reads. POST /v1/dashboard/wallet-auth returns a dashboard session_token sent in the Authorization header. "Wallet-as-identity. No profiles, no onboarding forms." (README)
  name: walletSignature
  scheme: ECDSA wallet signature (EIP-191 personal_sign style message)
  type: custom
- applies_to:
  - GET /v1/contracts/:id
  - /reader/*
  - handshake and sign flows
  description: 'A time-limited read token embedded in the reader_url returned on contract creation (https://getamber.dev/reader/<hash>?token=...). Grants the counterparty read access to the full contract without an API key. Privacy policy: default expiry 7 days, maximum 1 year, validated server-side.'
  in: query
  name: shareToken
  parameter: token
  type: apiKey
- applies_to:
  - POST /v1/dashboard
  description: Dashboard session token returned by POST /v1/dashboard/wallet-auth, "use in Authorization header for dashboard API".
  name: sessionToken
  scheme: bearer
  type: http
slug: getamber-dev-authentication
source_filename: getamber-dev-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: searched\nsource: >-\n  https://getamber.dev/docs (Get a Free Developer Key, REST API, x402 Pay-per-mandate, Wallet Auth),\n  https://getamber.dev/developers (endpoint table, /v1/keys, /wallet-auth, /dashboard/wallet-auth), the A2A\n  agent card securitySchemes (a2a/getamber-dev-agent-card.json), the MCP tools/list descriptions\n  (mcp/getamber-dev-mcp-tools.json) and live anonymous responses observed 2026-09-19. Ambr publishes no\n  OpenAPI, so derive-authentication.py (which reads securitySchemes) produced nothing; this profile is\n  hand-written from the documentation and the agent card, which is the one machine-readable place Ambr\n  declares its schemes.\ndocs: https://getamber.dev/docs\nsummary:\n  types: [apiKey, x402-payment, wallet-signature, share-token, session-token]\n  primary: apiKey\n  oauth2: false\n  oidc: false\n  discovery: 'none — /.well-known/oauth-authorization-server, /oauth-protected-resource and /openid-configuration\
  \ 404 on getamber.dev and ambr.run'\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  header: X-API-Key\n  key_prefix: 'amb_ (docs page: response.api_key → \"amb_...\"); the developers page''s /v1/keys snippet shows \"ambr_live_...\" — the two pages disagree and the docs page is the newer wording'\n  issuance: 'POST /api/v1/keys or the /activate page: enter an email, click a one-time magic link (expires in 30 minutes) — that verifies the address and reveals the key. Developer tier is free (25 credits); paid tiers verify a Base L2 USDC tx_hash or Stripe checkout.'\n  storage: 'Keys are stored as SHA-256 hashes and shown once; a lost key is replaced by requesting a new link (docs, privacy policy §1).'\n  applies_to: 'POST /v1/contracts (or x402), GET /v1/contracts/:id (or share token), POST /v1/contracts/:id/revoke (or wallet signature), POST /v1/dashboard, POST /v1/identity/verify (or share token), /v1/delegations; MCP state-changing tools (ambr_create_contract, ambr_agent_handshake)'\n\
  \  observed: 'GET /api/v1/contracts without a key -> 401 {\"error\":\"unauthorized\",\"message\":\"Valid API key required via X-API-Key header, or provide ?wallet= with signature headers\"}'\n  agent_card_declaration: '{\"type\":\"apiKey\",\"in\":\"header\",\"name\":\"X-API-Key\",\"description\":\"Pre-registered API key for businesses with credit-based access\"}'\n- name: x402\n  type: http\n  scheme: x402\n  header: X-Payment\n  description: >-\n    Pay-per-contract instead of an API key: the client pays on Base L2 (USDC, USDbC, DAI, ETH, WETH, cbETH,\n    cbBTC) and retries with the transaction hash in X-Payment. Unpaid paid-endpoint calls receive HTTP 402\n    with x402 payment instructions (REST) or JSON-RPC -32001 \"Payment required\" with the same payload\n    (MCP). Observed live 2026-09-19 on ambr_create_contract: version \"2\", price 500000, currency USD,\n    chain base, recipient address, accepts [exact, overpay], accepted_tokens[7], pricing per template.\n    \"This enables\
  \ fully autonomous agent-to-agent commerce without pre-registration.\" (docs)\n  applies_to: [POST /v1/contracts, MCP ambr_create_contract]\n  agent_card_declaration: '{\"type\":\"http\",\"scheme\":\"x402\",\"description\":\"Pay-per-contract via USDC on Base L2. Send payment, include tx hash in X-Payment header.\"}'\n- name: walletSignature\n  type: custom\n  scheme: ECDSA wallet signature (EIP-191 personal_sign style message)\n  description: >-\n    Counterparties and principals authenticate by signing a challenge message with an EVM wallet; the body\n    carries wallet_address, signature and message. Used to sign (message must contain \"I am signing Ambr\n    contract <id>\" and the SHA-256 hash), to revoke (\"I revoke Ambr contract <id> with hash <sha256>\"),\n    for handshake approval, and on POST /v1/contracts/:id/wallet-auth which returns a short-lived JWT\n    access_token for contract reads. POST /v1/dashboard/wallet-auth returns a dashboard session_token\n    sent in the Authorization\
  \ header. \"Wallet-as-identity. No profiles, no onboarding forms.\" (README)\n  applies_to: ['POST /v1/contracts/:id/sign', 'POST /v1/contracts/:id/handshake', 'POST /v1/contracts/:id/revoke', 'POST /v1/contracts/:id/wallet-auth', 'POST /v1/dashboard/wallet-auth']\n- name: shareToken\n  type: apiKey\n  in: query\n  parameter: token\n  description: >-\n    A time-limited read token embedded in the reader_url returned on contract creation\n    (https://getamber.dev/reader/<hash>?token=...). Grants the counterparty read access to the full\n    contract without an API key. Privacy policy: default expiry 7 days, maximum 1 year, validated\n    server-side.\n  applies_to: ['GET /v1/contracts/:id', '/reader/*', 'handshake and sign flows']\n- name: sessionToken\n  type: http\n  scheme: bearer\n  description: Dashboard session token returned by POST /v1/dashboard/wallet-auth, \"use in Authorization header for dashboard API\".\n  applies_to: [POST /v1/dashboard]\npublic_endpoints:\n  note: 'These\
  \ need no credential at all (docs endpoint table Auth = None, plus observed 200s).'\n  list:\n  - GET /api/v1/templates\n  - GET /api/v1/pricing\n  - GET /api/health\n  - 'GET /api/v1/contracts/:id/status'\n  - GET /.well-known/agent-card.json\n  - MCP initialize, tools/list and read-only tools\n  - A2A message/send routing\nmcp_auth: 'X-API-Key header on the MCP HTTP request (client config in docs); read-only tools anonymous; paid tools x402 or key'\na2a_auth: 'card security: [{apiKey: []}, {x402: []}]'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/getamber-dev/refs/heads/main/authentication/getamber-dev-authentication.yml
summary_line: apiKey/x402-payment/wallet-signature/share-token/session-token · 5 schemes
tags:
- Company
- AI Agents
- Agentic Commerce
- Contracts
- Legal
- Ricardian Contracts
- Delegation
- Blockchain
- Base L2
- MCP
- A2A
- x402
- Agent-Native
---
