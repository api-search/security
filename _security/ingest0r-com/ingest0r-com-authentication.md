---
anonymous_access: true
api_key_in: []
api_specs:
- filename: ingest0r-com-openapi.yml
  format: yaml
  label: Cook County (Chicago) Property Records API
  slug: cook-county-property-records-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ingest0r-com/refs/heads/main/openapi/ingest0r-com-openapi.yml
auth_types:
- none
- payment
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Ingest0R Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: ingest0r secures its APIs with none and payment across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: ingest0r
provider_slug: ingest0r-com
scheme_count: 2
schemes:
- applies_to:
  - v1_search (GET /v1/search/{q}) — always free, unlimited
  - GET /v1/sample — always free, fixed fixture
  - GET /v1/dossier/09253050270000, /09253060510000, /09253140190000 — always-free live example PINs
  - v1_parcel, v1_dossier, v1_comps — first 25 calls per client per day (metered; X-Free-Tier-Remaining header)
  description: 'Verbatim from the root manifest: "none — no signup, no API key, and no wallet needed to start: address search is always free and the first 25 calls per client per day to the PIN routes return real data free. x402 (USDC) covers anything past that."'
  name: none
  observed: 'GET /v1/search/1%20E%20113th%20St -> 200 (no headers beyond HSTS); GET /v1/dossier/09253050270000 -> 200 with x-free-example: true; GET /v1/parcel/25221090340000 -> 200 with x-free-tier: true, x-free-tier-limit: 25, x-free-tier-remaining: 24. The free-tier metering key ("per client") is not documented further.'
  sources:
  - https://api.ingest0r.com/
  - https://api.ingest0r.com/pricing
  type: none
- applies_to:
  - v1_parcel ($0.01), v1_dossier ($0.03), v1_comps ($0.10) — past the daily free allowance
  - route-template URLs and directory-probe PINs — always 402 (changelog 0.4.2, "so listing verification is unaffected")
  description: 'The OpenAPI carries a top-level x-payment {protocol x402, x402Version 2, accepts[]} and per-operation x-payment-info {price {mode fixed, amount, currency USD}, protocols[{x402{...}}]}; the agent card carries the same terms as the https://x402.org/extensions/payments capability extension. Payment guards documented in the changelog: HEAD never settles, size cap, replay pre-check, and the guards cover both the v2 PAYMENT-SIGNATURE header and legacy X-PAYMENT (0.4.1).'
  facilitator: https://facilitator.payai.network
  in: header (payment on the retried request)
  max_timeout_seconds: 60
  mcp: On the MCP server the 402 is returned in the tool result as _meta["x402/error"] (isError) and payment is supplied via _meta["x402/payment"], with the receipt in _meta["x402/payment-response"] and agents-x402/priceUSD in tool _meta (changelog 0.4.1).
  name: x402
  networks:
  - asset: USDC
    asset_contract: '0x833589fCD6eDb6E08f4c7C32D4f71b54bdA02913'
    chain: Base mainnet
    network: eip155:8453
    pay_to: '0x98D530C0667A4B18e692F182DdCAb1c2bECb5B9B'
  - asset: USDC
    asset_mint: EPjFWdd5AufqSSqeM2qN1xzybapC8G4wEGGkZwyTDt1v
    chain: Solana mainnet
    fee_payer: CjNFTjvBhbJJd2B5ePPMHRLx1ELZpa8dwQgGL727eKww
    network: solana:5eykt4UsFv8P8NJdTREpY1vzqKqZKvdp
    pay_to: G3qr8ahZnuFSYjvrCYM4LLDdoLzFq8Boq9XrURVcA9YF
  observed: GET https://api.ingest0r.com/v1/parcel/%7Bpin%7D -> HTTP 402, cache-control private no-store, PAYMENT-REQUIRED header present, application/json body with x402Version 2 and both accepts[] entries. Nothing was paid.
  prices_atomic_usdc_6dp:
    v1_comps: '100000'
    v1_dossier: '30000'
    v1_parcel: '10000'
    v1_search: '0'
  request_headers:
  - PAYMENT-SIGNATURE (x402 v2)
  - X-PAYMENT (legacy)
  response_headers:
  - PAYMENT-REQUIRED (base64 PaymentRequired)
  - PAYMENT-RESPONSE (settle receipt
  - per x402 v2)
  scheme: exact
  sources:
  - https://api.ingest0r.com/openapi.json
  - https://api.ingest0r.com/.well-known/x402
  - https://api.ingest0r.com/changelog.json
  standard: x402 v2 (HTTP 402)
  type: payment
slug: ingest0r-com-authentication
source_filename: ingest0r-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: searched\nsource:\n- https://api.ingest0r.com/openapi.json (x-payment, per-route x-payment-info; no securitySchemes)\n- https://api.ingest0r.com/ (discovery manifest \"auth\" field)\n- https://api.ingest0r.com/pricing\n- https://api.ingest0r.com/.well-known/x402\n- live 402 challenge observed on https://api.ingest0r.com/v1/parcel/{pin}, 2026-09-19\ndocs:\n- https://api.ingest0r.com/llms.txt\nspec: openapi/ingest0r-com-openapi.yml\nsummary:\n  types:\n  - none\n  - payment\n  api_key_in: []\n  oauth2_flows: []\n  bearer: false\n  credential_classes: 2\n  headline: >-\n    No account, no API key, no signup, no wallet to start. The OpenAPI declares no securitySchemes because there\n    is no credential: address search and the sample are always free, the three PIN routes return real data free\n    for the first 25 calls per client per day, and past that allowance the only \"credential\" is an x402 v2\n    payment — the route answers HTTP 402 with\
  \ machine-readable terms and is retried with a signed USDC payment on\n    Base or Solana. derive-authentication.py therefore produced nothing from the spec; this profile is built from\n    the provider's discovery manifest, x402 resource list, pricing endpoint and the live 402 challenge.\nschemes:\n- name: none\n  type: none\n  applies_to:\n  - v1_search (GET /v1/search/{q}) — always free, unlimited\n  - GET /v1/sample — always free, fixed fixture\n  - GET /v1/dossier/09253050270000, /09253060510000, /09253140190000 — always-free live example PINs\n  - v1_parcel, v1_dossier, v1_comps — first 25 calls per client per day (metered; X-Free-Tier-Remaining header)\n  description: >-\n    Verbatim from the root manifest: \"none — no signup, no API key, and no wallet needed to start: address search\n    is always free and the first 25 calls per client per day to the PIN routes return real data free. x402 (USDC)\n    covers anything past that.\"\n  observed: >-\n    GET /v1/search/1%20E%20113th%20St\
  \ -> 200 (no headers beyond HSTS); GET /v1/dossier/09253050270000 -> 200 with\n    x-free-example: true; GET /v1/parcel/25221090340000 -> 200 with x-free-tier: true, x-free-tier-limit: 25,\n    x-free-tier-remaining: 24. The free-tier metering key (\"per client\") is not documented further.\n  sources:\n  - https://api.ingest0r.com/\n  - https://api.ingest0r.com/pricing\n- name: x402\n  type: payment\n  standard: x402 v2 (HTTP 402)\n  in: header (payment on the retried request)\n  request_headers: [PAYMENT-SIGNATURE (x402 v2), X-PAYMENT (legacy)]\n  response_headers: [PAYMENT-REQUIRED (base64 PaymentRequired), PAYMENT-RESPONSE (settle receipt, per x402 v2)]\n  networks:\n  - {network: eip155:8453, chain: Base mainnet, asset: USDC, asset_contract: '0x833589fCD6eDb6E08f4c7C32D4f71b54bdA02913', pay_to: '0x98D530C0667A4B18e692F182DdCAb1c2bECb5B9B'}\n  - {network: solana:5eykt4UsFv8P8NJdTREpY1vzqKqZKvdp, chain: Solana mainnet, asset: USDC, asset_mint: EPjFWdd5AufqSSqeM2qN1xzybapC8G4wEGGkZwyTDt1v,\
  \ pay_to: G3qr8ahZnuFSYjvrCYM4LLDdoLzFq8Boq9XrURVcA9YF, fee_payer: CjNFTjvBhbJJd2B5ePPMHRLx1ELZpa8dwQgGL727eKww}\n  scheme: exact\n  facilitator: https://facilitator.payai.network\n  max_timeout_seconds: 60\n  prices_atomic_usdc_6dp: {v1_search: '0', v1_parcel: '10000', v1_dossier: '30000', v1_comps: '100000'}\n  applies_to:\n  - v1_parcel ($0.01), v1_dossier ($0.03), v1_comps ($0.10) — past the daily free allowance\n  - route-template URLs and directory-probe PINs — always 402 (changelog 0.4.2, \"so listing verification is unaffected\")\n  description: >-\n    The OpenAPI carries a top-level x-payment {protocol x402, x402Version 2, accepts[]} and per-operation\n    x-payment-info {price {mode fixed, amount, currency USD}, protocols[{x402{...}}]}; the agent card carries the\n    same terms as the https://x402.org/extensions/payments capability extension. Payment guards documented in the\n    changelog: HEAD never settles, size cap, replay pre-check, and the guards cover both the v2 PAYMENT-SIGNATURE\n\
  \    header and legacy X-PAYMENT (0.4.1).\n  observed: >-\n    GET https://api.ingest0r.com/v1/parcel/%7Bpin%7D -> HTTP 402, cache-control private no-store, PAYMENT-REQUIRED\n    header present, application/json body with x402Version 2 and both accepts[] entries. Nothing was paid.\n  mcp: >-\n    On the MCP server the 402 is returned in the tool result as _meta[\"x402/error\"] (isError) and payment is\n    supplied via _meta[\"x402/payment\"], with the receipt in _meta[\"x402/payment-response\"] and\n    agents-x402/priceUSD in tool _meta (changelog 0.4.1).\n  sources:\n  - https://api.ingest0r.com/openapi.json\n  - https://api.ingest0r.com/.well-known/x402\n  - https://api.ingest0r.com/changelog.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ingest0r-com/refs/heads/main/authentication/ingest0r-com-authentication.yml
summary_line: none/payment · 2 schemes
tags:
- Company
- Real-Estate
- Property Records
- Property Data
- Public Records
- Open Data
- Government Data
- Parcel
- Geocoding
- Property Tax
- Building Permits
- Comparable Sales
- Valuation
- x402
- Agentic Commerce
- MCP
- A2A
- agent-native
- Chicago
- Illinois
---
