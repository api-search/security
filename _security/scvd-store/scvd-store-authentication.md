---
anonymous_access: true
api_key_in: []
api_specs:
- filename: scvd-store-openapi.json
  format: json
  label: SCVD General Store API
  slug: scvd-general-store-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scvd-store/refs/heads/main/openapi/scvd-store-openapi.json
auth_types:
- none (anonymous)
- x402 payment signature (per-call)
- http bearer (one narrow scope)
- http basic (back office, not for agents)
description: ''
kind: authentication
layout: security
mechanism_count: 4
method: searched
name: Scvd Store Authentication
name_suffix: Authentication
oauth_flows: []
overview: SCVD General Store secures its APIs with none (anonymous), x402 payment signature (per-call), http bearer (one narrow scope), and http basic (back office, not for agents) across 5 declared security schemes, as derived from its OpenAPI definitions.
provider_name: SCVD General Store
provider_slug: scvd-store
scheme_count: 5
schemes:
- applies_to: 'every free door: preflight, conformance, look, before-you-pay, verify, corpus and datasets, menu, openapi.json, MCP tools/list + resources/read + the 14 free tools, all three A2A skills'
  description: Send the request. "If a request to one of these fails, it failed for a reason printed in the body — never because you were not recognised."
  name: anonymous
  sources:
  - https://scvd.store/auth.md
  - well-known/scvd-store-oauth-protected-resource.json
  type: none
- applies_to: the 35 GET /api/buy/{item} doors, the publication pages and the six buy_* MCP tools
  challenge: HTTP 402 with PAYMENT-REQUIRED (base64 x402 v2 terms) and WWW-Authenticate naming resource_metadata; JSON-RPC error 402 over MCP
  description: '"That signature IS the credential: it authenticates nothing about who you are, and it does not have to — it settles the call it paid for and it is good for that call only." Settled in USDC on Base, Polygon, Arbitrum, World or Solana via the Coinbase CDP facilitator; the store never holds funds. Revocation: nothing to revoke — a payment authorises exactly one call.'
  header: PAYMENT-SIGNATURE (legacy X-PAYMENT honoured); over MCP _meta['x402/payment']; over MPP the org.paymentauth/credential meta key
  in: header
  name: x402_payment_signature
  safety: Idempotency-Key (16–128 chars; suggested_key in every 402) prevents a retry loop from double-charging; the store delivers first and settles after so a failed delivery takes no money.
  sources:
  - https://scvd.store/auth.md
  - openapi x-payment-info on each door
  - live 402 on GET /api/buy/small_blessing 2026-09-19
  type: payment (x402 v2)
- applies_to:
  - get_api_purchase_status_purchase_id
  description: Private recovery.status_token returned by a catalogue purchase. This capability reads only its original purchase status. (The only securityScheme declared in the OpenAPI; MCP check_purchase takes it as status_token.)
  name: purchaseStatusToken
  scheme: bearer
  sources:
  - openapi/scvd-store-openapi.json
  type: http
- algorithm: sha256=HMAC-SHA256(secret, timestamp.nonce.body); 300-second window; nonce replay refused
  applies_to:
  - post_api_trade_partner_item_id
  - get_api_trade_partner_claim
  - get_api_trade_partner_statement
  - post_api_trade_partner_check
  - post_api_trade_sandbox_item_id
  - post_api_trade_sandbox_check
  description: Reseller (trade counter) accounts only; secrets are issued out of band by the keeper. A sandbox account with a published secret exists for exercising the dialect (see sandbox/).
  headers:
  - X-Trade-Key
  - X-Trade-Timestamp
  - X-Trade-Nonce
  - X-Trade-Signature
  in: headers
  name: trade_hmac
  note: Not declared as a securityScheme in the OpenAPI (the trade operations declare 401/409 responses); documented at /api/trade/contract.
  sources:
  - https://scvd.store/api/trade/contract
  type: hmac
- applies_to:
  - /admin (not in the contract)
  description: '"HTTP Basic, one human''s password … no agent has business behind it, no credential for it is issued to anyone, and a failed attempt is throttled per address and raises an alarm." Listed because a scanner will find the 401.'
  name: keeper_basic
  scheme: basic
  sources:
  - https://scvd.store/auth.md
  type: http
slug: scvd-store-authentication
source_filename: scvd-store-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: searched\nsource: https://scvd.store/auth.md\nderived_from: openapi/scvd-store-openapi.json\ndocs:\n- https://scvd.store/auth.md\n- https://scvd.store/.well-known/oauth-protected-resource\n- https://scvd.store/developers\nsummary:\n  types:\n  - none (anonymous)\n  - x402 payment signature (per-call)\n  - http bearer (one narrow scope)\n  - http basic (back office, not for agents)\n  identity_types_supported:\n  - anonymous\n  api_key_in: []\n  oauth2_flows: []\n  registration_required: false\n  signup_url: null\n  api_key_url: null\nstatement: '\"There is no account here. No key to request, no signup form, no approval queue, no waitlist, no tier\n  you get promoted into.\" (auth.md). The RFC 9728 document encodes the same: identity_types_supported [anonymous],\n  register_uri / claim_uri / revocation_uri null, bearer_methods_supported [], scopes_supported [], and NO authorization_servers\n  because no OAuth server exists.'\nschemes:\n- name:\
  \ anonymous\n  type: none\n  applies_to: 'every free door: preflight, conformance, look, before-you-pay, verify, corpus and datasets, menu,\n    openapi.json, MCP tools/list + resources/read + the 14 free tools, all three A2A skills'\n  description: Send the request. \"If a request to one of these fails, it failed for a reason printed in the body\n    — never because you were not recognised.\"\n  sources:\n  - https://scvd.store/auth.md\n  - well-known/scvd-store-oauth-protected-resource.json\n- name: x402_payment_signature\n  type: payment (x402 v2)\n  in: header\n  header: PAYMENT-SIGNATURE (legacy X-PAYMENT honoured); over MCP _meta['x402/payment']; over MPP the org.paymentauth/credential\n    meta key\n  challenge: HTTP 402 with PAYMENT-REQUIRED (base64 x402 v2 terms) and WWW-Authenticate naming resource_metadata;\n    JSON-RPC error 402 over MCP\n  applies_to: the 35 GET /api/buy/{item} doors, the publication pages and the six buy_* MCP tools\n  description: '\"That signature IS the\
  \ credential: it authenticates nothing about who you are, and it does not have\n    to — it settles the call it paid for and it is good for that call only.\" Settled in USDC on Base, Polygon, Arbitrum,\n    World or Solana via the Coinbase CDP facilitator; the store never holds funds. Revocation: nothing to revoke\n    — a payment authorises exactly one call.'\n  safety: Idempotency-Key (16–128 chars; suggested_key in every 402) prevents a retry loop from double-charging;\n    the store delivers first and settles after so a failed delivery takes no money.\n  sources:\n  - https://scvd.store/auth.md\n  - openapi x-payment-info on each door\n  - live 402 on GET /api/buy/small_blessing 2026-09-19\n- name: purchaseStatusToken\n  type: http\n  scheme: bearer\n  applies_to:\n  - get_api_purchase_status_purchase_id\n  description: Private recovery.status_token returned by a catalogue purchase. This capability reads only its original\n    purchase status. (The only securityScheme declared in the\
  \ OpenAPI; MCP check_purchase takes it as status_token.)\n  sources:\n  - openapi/scvd-store-openapi.json\n- name: trade_hmac\n  type: hmac\n  in: headers\n  headers:\n  - X-Trade-Key\n  - X-Trade-Timestamp\n  - X-Trade-Nonce\n  - X-Trade-Signature\n  algorithm: sha256=HMAC-SHA256(secret, timestamp.nonce.body); 300-second window; nonce replay refused\n  applies_to:\n  - post_api_trade_partner_item_id\n  - get_api_trade_partner_claim\n  - get_api_trade_partner_statement\n  - post_api_trade_partner_check\n  - post_api_trade_sandbox_item_id\n  - post_api_trade_sandbox_check\n  description: Reseller (trade counter) accounts only; secrets are issued out of band by the keeper. A sandbox account\n    with a published secret exists for exercising the dialect (see sandbox/).\n  note: Not declared as a securityScheme in the OpenAPI (the trade operations declare 401/409 responses); documented\n    at /api/trade/contract.\n  sources:\n  - https://scvd.store/api/trade/contract\n- name: keeper_basic\n\
  \  type: http\n  scheme: basic\n  applies_to:\n  - /admin (not in the contract)\n  description: '\"HTTP Basic, one human''s password … no agent has business behind it, no credential for it is issued\n    to anyone, and a failed attempt is throttled per address and raises an alarm.\" Listed because a scanner will\n    find the 401.'\n  sources:\n  - https://scvd.store/auth.md\ndiscovery:\n  protected_resource_metadata: https://scvd.store/.well-known/oauth-protected-resource\n  authorization_servers: null\n  openid_configuration: '404'\n  oauth_authorization_server: '404'\n  www_authenticate_on_402: X402 resource_metadata=\"<origin>/.well-known/oauth-protected-resource\" per the spec header\n    description; observed as a Payment challenge (MPP) on 2026-09-19\nwhat_the_store_never_asks_for: credentials, API keys, seed phrases, private keys, or wallet secrets — \"Anything\n  that asks you for one of those while claiming to be this store is not this store.\"\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/scvd-store/refs/heads/main/authentication/scvd-store-authentication.yml
summary_line: none (anonymous)/x402 payment signature (per-call)/http bearer (one narrow scope)/http basic (back office, not for agents) · 5 schemes
tags:
- Agents
- Agentic Commerce
- x402
- Payments
- Micropayments
- Stablecoins
- USDC
- Verification
- Conformance
- Attestation
- Observability
- MCP
- A2A
- Universal Commerce Protocol
- Signatures
- Agent-Native
- United States
---
