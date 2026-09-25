---
anonymous_access: false
api_key_in: []
api_specs:
- filename: elonsusk-com-openapi.json
  format: json
  label: Sandbox Contractor Agent REST API
  slug: sandbox-contractor-agent-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elonsusk-com/refs/heads/main/openapi/elonsusk-com-openapi.json
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 0
method: searched
name: Elonsusk Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: Artem / A2A Sandbox declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Artem / A2A Sandbox
provider_slug: elonsusk-com
scheme_count: 0
schemes: []
slug: elonsusk-com-authentication
source_filename: elonsusk-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: searched\nsource: https://a2a.elonsusk.com/.well-known/agent-card.json\nderived_from: openapi/elonsusk-com-openapi.json\ndocs:\n- https://a2a.elonsusk.com/.well-known/x402.json\n- https://a2a.elonsusk.com/docs\nsummary: >-\n  There is no authentication. The OpenAPI declares no securitySchemes and no security requirement on any\n  of its 24 operations; the agent card's auth block is {\"type\": \"none\", \"header\": null} and its\n  securitySchemes/security are empty; every read (agent card, x402 catalog, health, metrics, the full task\n  list, any task by id) answers anonymously. What gates the paid surface is PAYMENT, in two forms: an x402\n  v2 PAYMENT-SIGNATURE header on POST /x402/{skill} (a call without it returns HTTP 402 with a\n  PAYMENT-REQUIRED challenge), and for the quote-first task API an on-chain invoice whose memo must equal\n  the task id, confirmed by the operator's payment watcher or a checkout-provider webhook. Neither is an\n\
  \  identity: the agent never learns who the caller is, only that a payment settled. No API keys are issued,\n  no OAuth server exists (/.well-known/oauth-authorization-server and /oauth-protected-resource 404), and\n  no signup exists.\nschemes: []\naccess_model:\n  identity: none\n  gate: payment\n  mechanisms:\n  - name: x402 pay-per-call\n    surface: POST /x402/{skill} (x402_pay_per_call_x402__skill__post)\n    request_header: PAYMENT-SIGNATURE\n    challenge: HTTP 402 with PAYMENT-REQUIRED response header (base64 JSON, identical to the body) — x402Version 2, accepts[] of {scheme exact, network, amount, asset, payTo, maxTimeoutSeconds 120, extra}\n    settle_header: PAYMENT-RESPONSE (declared in /.well-known/x402.json; not observed — settlement was not exercised)\n    rails:\n    - {network: 'eip155:8453', asset: '0x833589fCD6eDb6E08f4c7C32D4f71b54bdA02913 (USDC on Base)', verification: evm_rpc}\n    - {network: 'solana:5eykt4UsFv8P8NJdTREpY1vzqKqZKvdp', asset: 'EPjFWdd5AufqSSqeM2qN1xzybapC8G4wEGGkZwyTDt1v\
  \ (USDC on Solana)', verification: solana_rpc}\n    facilitator: https://facilitator.payai.network\n    alternative: >-\n      accepts[].extra.note — \"Send USDC on Base to payTo, then retry with payload.tx_ref = the transaction\n      hash. Verified on-chain (receipt success, USDC contract, correct payee, amount >= price) and usable for\n      exactly one call.\" (invoiceBridge true, settlesRealFunds true)\n    observed: '2026-09-19 — POST https://a2a.elonsusk.com/x402/util.json.format returned 402 with the header and body above; amount \"2000\" for a $0.002 skill.'\n  - name: Quote-first crypto invoice\n    surface: POST /v1/tasks (create_task_v1_tasks_post) or A2A tasks/send on POST /a2a\n    flow: create task -> response carries quote {quote_usd, tokens_estimate, pricing} and invoice {amount_usd, asset, address, memo, expires_at, provider, status} -> pay any enabled method with memo = task id -> state moves payment_required -> paid -> working\n    methods: [SOL, USDC on Solana, ETH,\
  \ USDC on Ethereum, BTC]\n    confirmation: operator payment watcher (solana_rpc per /healthz) or checkout-provider webhook (NOWPayments, CoinGate via POST /v1/payments/webhook/{provider}); a manual fallback is declared in payment_notes.mode\n    source: agent card payment_methods, payment_notes, how_to_order\n  - name: Human lead intake\n    surface: POST /v1/leads (create_public_lead_v1_leads_post)\n    credential: none — contact string 3-240 chars, brief 12-8000 chars, optional budget_usd\n    note: The only channel that carries a human identity, and it is free text.\nopen_operations_of_note:\n- operation: list_tasks_v1_tasks_get\n  note: Returns every task in the queue with inputs, quotes, invoice addresses and memos, payment notes and results, to anyone. Not a documented feature; an observation.\n- operation: mark_paid_v1_tasks__task_id__mark_paid_post\n  note: Published in the public contract with no securityScheme. Whether the server verifies tx_ref before honouring it is not stated;\
  \ treat as operator-side.\n- operation: payment_webhook_v1_payments_webhook__provider__post\n  note: Inbound provider webhook with no declared signature verification scheme in the contract.\ntransport_security:\n  https: true\n  tls_version: TLSv1.2 (Cloudflare edge)\n  hsts: false\n  http_redirect: 301 to https on a2a.elonsusk.com\n  detail: security/elonsusk-com-domain-security.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/elonsusk-com/refs/heads/main/authentication/elonsusk-com-authentication.yml
summary_line: 0 schemes
tags:
- Agents
- Agentic Commerce
- A2A
- x402
- Developer Tools
- Blockchain
- Solana
- Ethereum
- Security
- Code Review
- Code Generation
- Agent-Native
---
