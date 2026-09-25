---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 0
method: probed
name: Scalpstream Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: ScalpStream declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: ScalpStream
provider_slug: scalpstream-com
scheme_count: 0
schemes: []
slug: scalpstream-com-authentication
source_filename: scalpstream-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: probed\nsource: agent cards (securitySchemes/security), /.well-known/x402 documents, live 402 challenges and the marketing site (\"no accounts, no API keys, no subscriptions\"), 2026-09-19\nsummary: >-\n  There is no authentication. Every surface is anonymous by design: the A2A JSON-RPC endpoints\n  and free previews need nothing at all, and the paid HTTP resources are gated by PAYMENT, not\n  identity - an x402 v2 challenge (HTTP 402 + PAYMENT-REQUIRED header) that any wallet on one of\n  five rails can satisfy per request. No API keys, OAuth, OIDC, mTLS, sign-up or account exist,\n  and the agent cards declare securitySchemes {} and security []. The one non-payment gate is a\n  required attestation header on the research feed.\nschemes: []\nschemes_note: no securityScheme of any kind - apiKey, http, oauth2, openIdConnect and mutualTLS are all absent\naccess_model:\n  free:\n    surfaces: [GET /preview on every host (+ feed /preview-dividends\
  \ /preview-crypto /preview-yields /schema), POST /a2a (A2A JSON-RPC), /.well-known/agent-card.json, /.well-known/x402, /llms.txt]\n    auth: none\n  paid:\n    surfaces: [GET /recalls, GET /air, GET /crossings, GET /fuel, GET /picks, GET /dividends, GET /crypto, GET /yields]\n    gate: x402 v2 payment challenge (HTTP 402) - see x402/scalpstream-com-x402.yml\n    identity_required: false\n    payment_header: PAYMENT-REQUIRED (server) / payment payload per x402 v2 (client); legacy X-PAYMENT-REQUIRED also emitted\n    rails: [USDC on Base, USDC on Arbitrum, USDC on Polygon, XRP on XRPL, RLUSD on XRPL]\n    price_usd: '0.01'\nrequired_headers:\n- header: X-Compliance-Attestation\n  value: not-sanctioned-party\n  applies_to: paid resources on feed.scalpstream.com only\n  behaviour: request refused with HTTP 403 before settlement when absent\n  source: https://feed.scalpstream.com/.well-known/x402\nfirst_party_client:\n  name: scalpmcp (github.com/DV1-321/scalpstream-mcp)\n  buyer_secret: EVM_BASE_PRIVATE_KEY\
  \ held in process memory on the buyer's machine; never sent to ScalpStream\n  note: the only key anywhere in the flow is the buyer's own wallet key, per the README\ndocs: https://www.scalpstream.com/ (\"The x402 Flow\")\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/scalpstream-com/refs/heads/main/authentication/scalpstream-com-authentication.yml
summary_line: 0 schemes
tags:
- Company
- Agents
- A2A
- x402
- Micropayments
- MCP
- Open Data
- Product Recalls
- Air Quality
- Border Crossings
- Fuel Prices
- Market Research
- Public Safety
- Cryptocurrency
- USDC
- XRP Ledger
- llms-txt
- JSON Schema
---
