---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: solvela-ai-openapi.json
  format: json
  label: Solvela Gateway API
  slug: solvela-gateway-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/solvela-ai/refs/heads/main/openapi/solvela-ai-openapi.json
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 4
method: searched
name: Solvela Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Solvela secures its APIs with apiKey and http across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Solvela
provider_slug: solvela-ai
scheme_count: 4
schemes:
- challenge:
    body: x402 PaymentRequired object (snake_case) at the top level
    header: PAYMENT-REQUIRED — base64 of the canonical camelCase challenge
    observed: 2026-09-19 on POST /v1/chat/completions, POST /v1/messages, POST /v1/search
    schemes_offered:
    - exact
    - escrow
    status: 402
    validity: max_timeout_seconds 300 (observed)
  description: 'x402 payment payload: JSON (raw or base64-encoded) of the form { x402_version, resource: {url, method}, accepted: <one entry from the 402 challenge''s accepts[]>, payload: { transaction } | { deposit_tx, service_id, agent_pubkey } }, where transaction / deposit_tx is a base64-encoded signed Solana versioned transaction. Omit the header to receive the 402 challenge quoting the price. (Quoted from the securityScheme description.)'
  in: header
  name: x402Payment
  not_required_for:
  - listModels
  - getReceipt
  - health
  - createChatCompletion when the quoted cost is exactly 0 atomic USDC (free models)
  parameter: PAYMENT-SIGNATURE
  payload_variants:
  - note: pre-signed USDC-SPL TransferChecked to pay_to for accepts[].amount
    payload: '{ transaction }'
    scheme: exact
  - note: deposit to the Anchor escrow PDA (program 9neDHouXgEgHZDde5SpmqqEZ9Uv35hFcjtFEPxomtHLU); PDA seeds ["escrow", agent_pubkey, service_id]
    payload: '{ deposit_tx, service_id, agent_pubkey }'
    scheme: escrow
  - note: not advertised in accepts[]; opened via POST /v1/channel/open, closed via POST /v1/channel/close
    payload: signed cumulative voucher (domain solvela-channel-voucher-v1) binding channel id, new cumulative, SHA-256 of the request bytes and an expiry slot; signed by the channel session key
    scheme: channel (voucher)
  sources:
  - openapi/solvela-ai-openapi.json
  standard: x402 v2
  type: apiKey
  used_by:
  - createChatCompletion
  - POST /v1/messages
  - POST /v1/search
  - POST /v1/solana/price
  - POST /a2a message/send (as x402.payment.payload metadata)
  verification_pipeline:
  - 50 KB header size limit
  - base64 or raw JSON decode
  - replay check (Redis SET NX EX 120 on the tx signature)
  - VersionedTransaction deserialisation
  - TransferChecked discriminator
  - ATA derivation
  - amount >= quoted
  - recipient = gateway USDC ATA
  - mint = configured USDC
- description: Organisation-scoped API keys for enterprise accounts (org hierarchy, team budgets, audit logs, usage analytics). Keys carry full organisational permissions; the secret is shown once at creation and stored hashed. Rate limiting for key auth is per source IP rather than per wallet (docs comparison table).
  issuance: enterprise account; no self-serve signup documented
  key_prefix: solvela_k_
  name: EnterpriseApiKey
  parameter: 'Authorization: Bearer solvela_k_...'
  scheme: bearer
  sources:
  - https://github.com/solvela-ai/solvela/blob/main/dashboard/content/docs/api/authentication.mdx
  type: http
  used_by:
  - /v1/orgs/... (undeclared in the OpenAPI; live GET /v1/orgs returned 401 "Valid admin token or API key required")
  - 'createChatCompletion (docs example shows Authorization: Bearer solvela_k_ on chat)'
- audience: operator
  description: Constant-time-compared operator token gating /metrics, /v1/escrow/health, /v1/admin/stats and POST /v1/services/register. When unset, /metrics is hidden (404).
  name: AdminToken
  observed: GET /metrics -> 401 "unauthorized"; GET /v1/admin/stats -> 401 {"error":"unauthorized"}
  parameter: 'Authorization: Bearer <SOLVELA_ADMIN_TOKEN>'
  scheme: bearer
  sources:
  - https://github.com/solvela-ai/solvela/blob/main/dashboard/content/docs/operations/security.mdx
  type: http
- description: 'Unguessable identifiers that are themselves the credential: the UUIDv4 receipt id returned in the X-Solvela-Receipt header (GET /v1/receipts/{receipt_id}; unknown and malformed ids return identical 404s, rate-capped per IP) and the A2A task id (tasks/get for ~10 minutes after the last state change). The provider documents both as bearer capabilities to be kept secret.'
  name: BearerCapabilities
  sources:
  - openapi/solvela-ai-openapi.json
  - https://github.com/solvela-ai/solvela/blob/main/dashboard/content/docs/concepts/a2a.mdx
  type: capability
slug: solvela-ai-authentication
source_filename: solvela-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: searched\nsource: openapi/solvela-ai-openapi.json\ndocs:\n- https://github.com/solvela-ai/solvela/blob/main/dashboard/content/docs/api/authentication.mdx\n- https://github.com/solvela-ai/solvela/blob/main/dashboard/content/docs/concepts/x402.mdx\n- https://github.com/solvela-ai/solvela/blob/main/dashboard/content/docs/operations/security.mdx\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\n  oauth2_flows: []\n  bearer: true\n  credential_classes: 4\n  headline: >-\n    No account and no signup for the public API: payment IS the authorization. A paid operation answers 402\n    with an x402 quote; the client signs a Solana USDC-SPL transaction (or an escrow deposit, or a spend-down\n    channel voucher) and resubmits with the signed payload in the PAYMENT-SIGNATURE header. Free ($0) models\n    need no header at all. Identity is the payer wallet (base58 pubkey) recovered from the signed transaction;\n    rate limits key on\
  \ it. Two Bearer-token schemes exist outside the four-operation contract: organisation API\n    keys prefixed solvela_k_ for the enterprise org/team/budget routes, and an admin token for /metrics,\n    /v1/escrow/health and marketplace registration. Receipt ids and A2A task ids are bearer capabilities.\n    No OAuth 2, no OIDC, no discovery documents on any host.\nschemes:\n- name: x402Payment\n  type: apiKey\n  in: header\n  parameter: PAYMENT-SIGNATURE\n  standard: x402 v2\n  description: >-\n    x402 payment payload: JSON (raw or base64-encoded) of the form { x402_version, resource: {url, method},\n    accepted: <one entry from the 402 challenge's accepts[]>, payload: { transaction } | { deposit_tx, service_id,\n    agent_pubkey } }, where transaction / deposit_tx is a base64-encoded signed Solana versioned transaction.\n    Omit the header to receive the 402 challenge quoting the price. (Quoted from the securityScheme description.)\n  challenge:\n    status: 402\n    body: x402 PaymentRequired\
  \ object (snake_case) at the top level\n    header: PAYMENT-REQUIRED — base64 of the canonical camelCase challenge\n    validity: max_timeout_seconds 300 (observed)\n    schemes_offered: [exact, escrow]\n    observed: '2026-09-19 on POST /v1/chat/completions, POST /v1/messages, POST /v1/search'\n  verification_pipeline: [50 KB header size limit, base64 or raw JSON decode, replay check (Redis SET NX EX 120 on the tx signature), VersionedTransaction deserialisation, TransferChecked discriminator, ATA derivation, amount >= quoted, recipient = gateway USDC ATA, mint = configured USDC]\n  payload_variants:\n  - {scheme: exact, payload: '{ transaction }', note: 'pre-signed USDC-SPL TransferChecked to pay_to for accepts[].amount'}\n  - {scheme: escrow, payload: '{ deposit_tx, service_id, agent_pubkey }', note: 'deposit to the Anchor escrow PDA (program 9neDHouXgEgHZDde5SpmqqEZ9Uv35hFcjtFEPxomtHLU); PDA seeds [\"escrow\", agent_pubkey, service_id]'}\n  - {scheme: channel (voucher), payload: 'signed\
  \ cumulative voucher (domain solvela-channel-voucher-v1) binding channel id, new cumulative, SHA-256 of the request bytes and an expiry slot; signed by the channel session key', note: 'not advertised in accepts[]; opened via POST /v1/channel/open, closed via POST /v1/channel/close'}\n  used_by: [createChatCompletion, 'POST /v1/messages', 'POST /v1/search', 'POST /v1/solana/price', 'POST /a2a message/send (as x402.payment.payload metadata)']\n  not_required_for: [listModels, getReceipt, health, 'createChatCompletion when the quoted cost is exactly 0 atomic USDC (free models)']\n  sources:\n  - openapi/solvela-ai-openapi.json\n- name: EnterpriseApiKey\n  type: http\n  scheme: bearer\n  parameter: 'Authorization: Bearer solvela_k_...'\n  key_prefix: solvela_k_\n  description: >-\n    Organisation-scoped API keys for enterprise accounts (org hierarchy, team budgets, audit logs, usage\n    analytics). Keys carry full organisational permissions; the secret is shown once at creation and stored\n\
  \    hashed. Rate limiting for key auth is per source IP rather than per wallet (docs comparison table).\n  used_by: ['/v1/orgs/... (undeclared in the OpenAPI; live GET /v1/orgs returned 401 \"Valid admin token or API key required\")', 'createChatCompletion (docs example shows Authorization: Bearer solvela_k_ on chat)']\n  issuance: enterprise account; no self-serve signup documented\n  sources:\n  - https://github.com/solvela-ai/solvela/blob/main/dashboard/content/docs/api/authentication.mdx\n- name: AdminToken\n  type: http\n  scheme: bearer\n  parameter: 'Authorization: Bearer <SOLVELA_ADMIN_TOKEN>'\n  audience: operator\n  description: Constant-time-compared operator token gating /metrics, /v1/escrow/health, /v1/admin/stats and POST /v1/services/register. When unset, /metrics is hidden (404).\n  observed: 'GET /metrics -> 401 \"unauthorized\"; GET /v1/admin/stats -> 401 {\"error\":\"unauthorized\"}'\n  sources:\n  - https://github.com/solvela-ai/solvela/blob/main/dashboard/content/docs/operations/security.mdx\n\
  - name: BearerCapabilities\n  type: capability\n  description: >-\n    Unguessable identifiers that are themselves the credential: the UUIDv4 receipt id returned in the\n    X-Solvela-Receipt header (GET /v1/receipts/{receipt_id}; unknown and malformed ids return identical 404s,\n    rate-capped per IP) and the A2A task id (tasks/get for ~10 minutes after the last state change). The\n    provider documents both as bearer capabilities to be kept secret.\n  sources:\n  - openapi/solvela-ai-openapi.json\n  - https://github.com/solvela-ai/solvela/blob/main/dashboard/content/docs/concepts/a2a.mdx\nwallet_identity:\n  format: Solana base58 public key\n  derived_from: the signer of the payment transaction (or the funding wallet of a channel)\n  used_for: [rate limiting, spend ledger, receipts (payer_wallet), enterprise org membership]\n  pii: none — the provider's regulatory-position document states no names, emails or identifiers are collected\ndiscovery_documents:\n  probed: '2026-09-19 on\
  \ api.solvela.ai and solvela-gateway.fly.dev'\n  openid_configuration: 404\n  oauth_authorization_server: 404\n  oauth_protected_resource: 404\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/solvela-ai/refs/heads/main/authentication/solvela-ai-authentication.yml
summary_line: apiKey/http · 4 schemes
tags:
- Company
- Payments
- Artificial Intelligence
- LLM Gateway
- x402
- Solana
- Stablecoins
- AI Agents
- MCP
- A2A
- Agentic Commerce
---
