---
anonymous_access: false
api_key_in: []
api_specs:
- filename: anchor-x402-openapi.json
  format: json
  label: anchor-x402 API
  slug: anchor-x402-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anchor-x402/refs/heads/main/openapi/anchor-x402-openapi.json
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Anchor X402 Authentication
name_suffix: Authentication
oauth_flows: []
overview: anchor-x402 declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: anchor-x402
provider_slug: anchor-x402
scheme_count: 2
schemes:
- applies_to: all 18 paid /v1/* routes and MCP tools/call
  description: x402 v2 pay-per-call. Modeled in the A2A agent card as an apiKey-in-header scheme because that is the closest A2A primitive; it is not a static credential - the header value is a signed, single-use, amount-bound payment authorization.
  id: x402
  in: header
  legacy_name: X-PAYMENT
  legacy_note: The deprecated x402 V1 X-PAYMENT header spelling is still accepted alongside the V2 name.
  name: PAYMENT-SIGNATURE
  protocol: x402 v2
  type: apiKey
- algorithm: ed25519
  applies_to: the four anchor-x402 extension methods on POST /v1/a2a (peer/hello, capabilities/list, peer/quote, peer/receipt)
  audience: https://api.anchor-x402.com
  digest: sha256:<hex> over compact key-sorted canonical JSON
  id: a2a-ed25519-envelope
  key_discovery: Peer identity bootstraps from DNS + TLS. A calling agent publishes an Ed25519 public key as a base64 DER SubjectPublicKeyInfo in its own /.well-known/agent-card.json under any extensions.<namespace> block, either as a flat {key_id, public_key_der_base64} pair or a keys[] array for gapless rotation. anchor-x402 fetches that card and verifies against it. No human step and no registration.
  replay_protection:
    exp_window_seconds: 300
    nonce: single-use, 8-128 chars
  revocation: Delete the block or mark that key with a "status" of "retired"; either takes effect within 1h.
  server_keys:
    custody: AWS KMS
    location: extensions["anchor-x402:a2a"].keys in the agent card
    note: Two distinct key sets serve two jobs - signatures[] proves the card itself is authentic, while extensions["anchor-x402:a2a"].keys is what peers use to sign requests. The A2A spec has no field for the latter, which is why it lives in an extension.
  signed_fields:
  - aud
  - body
  - exp
  - key_id
  - method
  - nonce
  - origin
  spec_methods_unsigned: The A2A spec methods themselves (message/send, tasks/get, tasks/cancel) are accepted unsigned, because a conformant A2A client will not produce this envelope; authorization there is the x402 payment.
  type: signature
slug: anchor-x402-authentication
source_filename: anchor-x402-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-11'\nmethod: searched\nsource: >-\n  https://anchor-x402.com/llms.txt, https://api.anchor-x402.com/.well-known/agent-card.json,\n  https://api.anchor-x402.com/.well-known/mcp/server-card.json, and a live 402 challenge observed at\n  POST https://api.anchor-x402.com/v1/price/token\ndocs: https://anchor-x402.com/llms.txt\nmodel: payment-as-authorization\naccounts: false\napi_keys: false\noauth: false\nsummary: >-\n  There is no account, no registration, no API key and no bearer token anywhere in this API. Authorization\n  IS payment. A request without a signed payment gets an HTTP 402 PaymentRequired carrying an accepts[]\n  array of settlement options; the caller signs an EIP-3009 transferWithAuthorization for one of them and\n  retries the identical request with the signed payload in a PAYMENT-SIGNATURE header. The x402 facilitator\n  verifies and settles, and the service answers. Identity is a wallet, and it is presented per call rather\n  than per session.\n\
  schemes:\n- id: x402\n  type: apiKey\n  in: header\n  name: PAYMENT-SIGNATURE\n  legacy_name: X-PAYMENT\n  legacy_note: The deprecated x402 V1 X-PAYMENT header spelling is still accepted alongside the V2 name.\n  protocol: x402 v2\n  applies_to: all 18 paid /v1/* routes and MCP tools/call\n  description: >-\n    x402 v2 pay-per-call. Modeled in the A2A agent card as an apiKey-in-header scheme because that is the\n    closest A2A primitive; it is not a static credential - the header value is a signed, single-use,\n    amount-bound payment authorization.\n- id: a2a-ed25519-envelope\n  type: signature\n  applies_to: the four anchor-x402 extension methods on POST /v1/a2a (peer/hello, capabilities/list, peer/quote, peer/receipt)\n  algorithm: ed25519\n  digest: 'sha256:<hex> over compact key-sorted canonical JSON'\n  signed_fields: [aud, body, exp, key_id, method, nonce, origin]\n  audience: https://api.anchor-x402.com\n  replay_protection:\n    nonce: single-use, 8-128 chars\n    exp_window_seconds:\
  \ 300\n  key_discovery: >-\n    Peer identity bootstraps from DNS + TLS. A calling agent publishes an Ed25519 public key as a base64\n    DER SubjectPublicKeyInfo in its own /.well-known/agent-card.json under any extensions.<namespace> block,\n    either as a flat {key_id, public_key_der_base64} pair or a keys[] array for gapless rotation.\n    anchor-x402 fetches that card and verifies against it. No human step and no registration.\n  revocation: >-\n    Delete the block or mark that key with a \"status\" of \"retired\"; either takes effect within 1h.\n  server_keys:\n    location: extensions[\"anchor-x402:a2a\"].keys in the agent card\n    custody: AWS KMS\n    note: >-\n      Two distinct key sets serve two jobs - signatures[] proves the card itself is authentic, while\n      extensions[\"anchor-x402:a2a\"].keys is what peers use to sign requests. The A2A spec has no field for\n      the latter, which is why it lives in an extension.\n  spec_methods_unsigned: >-\n    The A2A spec methods\
  \ themselves (message/send, tasks/get, tasks/cancel) are accepted unsigned, because a\n    conformant A2A client will not produce this envelope; authorization there is the x402 payment.\nsettlement_rails:\n- network: eip155:8453\n  name: Base mainnet\n  asset: USDC\n  asset_contract: '0x833589fCD6eDb6E08f4c7C32D4f71b54bdA02913'\n  pay_to: '0x127462e296fAc1A7F5cF33bA57bB2f0FFf5cD0B6'\n  facilitator: https://api.cdp.coinbase.com/platform/v2/x402\n  max_timeout_seconds: 300\n- network: 'solana:5eykt4UsFv8P8NJdTREpY1vzqKqZKvdp'\n  name: Solana mainnet\n  asset: USDC\n  asset_contract: EPjFWdd5AufqSSqeM2qN1xzybapC8G4wEGGkZwyTDt1v\n  pay_to: 6apuZvJQ51Led9iEjnHw6f5jfnXL4qjt8S1h58PeXzuR\n  fee_payer: CjNFTjvBhbJJd2B5ePPMHRLx1ELZpa8dwQgGL727eKww\n  facilitator: https://api.cdp.coinbase.com/platform/v2/x402\n  max_timeout_seconds: 300\n- network: 'eip155:137'\n  name: Polygon mainnet\n  asset: JPYC\n  asset_contract: '0x431D5dfF03120AFA4bDf332c61A6e1766eF37BDB'\n  asset_decimals: 18\n  pay_to:\
  \ '0x127462e296fAc1A7F5cF33bA57bB2f0FFf5cD0B6'\n  facilitator: in-process\n  max_timeout_seconds: 300\n  caveat: >-\n    The yen amounts are fixed tiers, not a live FX conversion - pegged at an assumed ~JPY200/USD with no\n    oracle, so the USD-equivalent of a JPYC payment floats against the USD price in both directions. The\n    provider states this plainly in llms.txt rather than burying it.\nfree_and_anonymous:\n- GET /health\n- GET /openapi.json\n- GET /docs\n- GET /redoc\n- POST /v1/attest/verify\n- MCP server/discover, initialize and tools/list\n- POST /v1/a2a spec methods and capabilities/list\nspec_gap: >-\n  openapi.json declares no components.securitySchemes and carries no security requirement on any operation,\n  so the published OpenAPI reads as an entirely open API. Everything in this file was reconstructed from the\n  agent card, the MCP server card, llms.txt and a live 402 response. A securitySchemes block naming the\n  PAYMENT-SIGNATURE header would make the contract self-describing.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/anchor-x402/refs/heads/main/authentication/anchor-x402-authentication.yml
summary_line: 2 schemes
tags:
- Company
- x402
- Agents
- Payments
- Blockchain
- MCP
- Web3
- Pay Per Call
- Agent Payments
- Stablecoins
- Compliance
- Attestation
---
