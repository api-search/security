---
anonymous_access: true
api_key_in: []
api_specs:
- filename: gonna-bond-legit-openapi.yml
  format: yaml
  label: LEGIT Trust API
  slug: legit-trust-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gonna-bond/refs/heads/main/openapi/gonna-bond-legit-openapi.yml
auth_types:
- none
- x402
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Gonna Bond Authentication
name_suffix: Authentication
oauth_flows: []
overview: GONNA secures its APIs with none and x402 across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: GONNA
provider_slug: gonna-bond
scheme_count: 3
schemes:
- applies_to: 'Every operation except the five paid ones: health, leaderboard, stats, check, receipts, route, report, batch-check, trending, pulse, chain-logos, networks, merchant identity, arena/preview, .well-known/legit, watches/{watch_id}, watches/{watch_id}/events, referee, referee/reproduce.py, and the MCP endpoint''s initialize and tools/list.'
  name: anonymous
  sources:
  - https://legit.gonna.bond/.well-known/agent.json
  - https://legit.gonna.bond/llms.txt
  type: none
- applies_to:
  - compare_v1_compare_get
  - arena_v1_arena_get
  - history_v1_history_get
  - create_watch_v1_watch_post
  - deep_check_v1_deep_check_post
  challenge_header: PAYMENT-REQUIRED
  flow:
  - Call the paid operation with no payment. It answers HTTP 402; the body is an x402 PaymentRequired document ({x402Version: 2, error, resource, accepts[], extensions}) and the same document is carried base64-encoded in a PAYMENT-REQUIRED response header.
  - accepts[] lists one USDC offer per rail — scheme exact, network (CAIP-2), amount in USDC base units, asset, payTo, maxTimeoutSeconds 300 — algorand-mainnet 4000 (= $0.004) and eip155:8453 (Base) 5000 (= $0.005) on 2026-09-19.
  - Pay on one rail (Algorand via facilitator.goplausible.xyz, gasless; Base via facilitator.payai.network) and retry the identical request with the PAYMENT-SIGNATURE request header carrying the payment payload. The server exposes PAYMENT-RESPONSE via Access-Control-Expose-Headers.
  name: x402
  observed:
    content_type: application/json
    fetched: '2026-09-19'
    http_status: 402
    url: https://legit.gonna.bond/v1/compare?addresses=A,B
  request_header: PAYMENT-SIGNATURE
  response_header: PAYMENT-RESPONSE
  scheme: x402 v2 (HTTP 402 challenge + PAYMENT-SIGNATURE retry)
  sources:
  - https://legit.gonna.bond/llms.txt
  - https://legit.gonna.bond/.well-known/agent.json
  - https://legit.gonna.bond/.well-known/x402
  type: payment
- applies_to:
  - watch_status_v1_watches__watch_id__get
  - watch_events_v1_watches__watch_id__events_get
  description: '"The watch id is a bearer capability": whoever knows the watch UUID reads its status and event feed for free. The docs tell integrators to keep it out of public logs, screenshots and client-side code.'
  name: watch-id-capability
  sources:
  - https://legit.gonna.bond/docs
  type: capability-url
slug: gonna-bond-authentication
source_filename: gonna-bond-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: searched\ndocs: https://legit.gonna.bond/llms.txt\nsource: >-\n  The OpenAPI at https://legit.gonna.bond/openapi.json declares NO components.securitySchemes and no\n  security[] (derive-authentication.py therefore produced nothing), so this profile is searched from the\n  provider's own statements: the agent card's `authentication` block, the llms.txt \"Payments (x402)\" section,\n  the x-guidance in info, and a live unauthenticated GET on https://legit.gonna.bond/v1/compare (HTTP 402,\n  2026-09-19).\nsummary:\n  types: [none, x402]\n  api_key_in: []\n  oauth2_flows: []\n  accounts_required: false\n  api_keys_issued: false\n  note: >-\n    \"No accounts, no API keys.\" Free operations need no credential at all; the five paid operations use the\n    x402 payment protocol in place of authentication — the caller proves payment, not identity.\nschemes:\n- name: anonymous\n  type: none\n  applies_to: >-\n    Every operation except the five paid\
  \ ones: health, leaderboard, stats, check, receipts, route, report,\n    batch-check, trending, pulse, chain-logos, networks, merchant identity, arena/preview, .well-known/legit,\n    watches/{watch_id}, watches/{watch_id}/events, referee, referee/reproduce.py, and the MCP endpoint's\n    initialize and tools/list.\n  sources: [https://legit.gonna.bond/.well-known/agent.json, https://legit.gonna.bond/llms.txt]\n- name: x402\n  type: payment\n  scheme: x402 v2 (HTTP 402 challenge + PAYMENT-SIGNATURE retry)\n  applies_to: [compare_v1_compare_get, arena_v1_arena_get, history_v1_history_get, create_watch_v1_watch_post, deep_check_v1_deep_check_post]\n  flow:\n  - Call the paid operation with no payment. It answers HTTP 402; the body is an x402 PaymentRequired document ({x402Version: 2, error, resource, accepts[], extensions}) and the same document is carried base64-encoded in a PAYMENT-REQUIRED response header.\n  - accepts[] lists one USDC offer per rail — scheme exact, network (CAIP-2),\
  \ amount in USDC base units, asset, payTo, maxTimeoutSeconds 300 — algorand-mainnet 4000 (= $0.004) and eip155:8453 (Base) 5000 (= $0.005) on 2026-09-19.\n  - Pay on one rail (Algorand via facilitator.goplausible.xyz, gasless; Base via facilitator.payai.network) and retry the identical request with the PAYMENT-SIGNATURE request header carrying the payment payload. The server exposes PAYMENT-RESPONSE via Access-Control-Expose-Headers.\n  request_header: PAYMENT-SIGNATURE\n  challenge_header: PAYMENT-REQUIRED\n  response_header: PAYMENT-RESPONSE\n  sources: [https://legit.gonna.bond/llms.txt, https://legit.gonna.bond/.well-known/agent.json, https://legit.gonna.bond/.well-known/x402]\n  observed:\n    url: https://legit.gonna.bond/v1/compare?addresses=A,B\n    http_status: 402\n    content_type: application/json\n    fetched: '2026-09-19'\n- name: watch-id-capability\n  type: capability-url\n  applies_to: [watch_status_v1_watches__watch_id__get, watch_events_v1_watches__watch_id__events_get]\n\
  \  description: >-\n    \"The watch id is a bearer capability\": whoever knows the watch UUID reads its status and event feed for\n    free. The docs tell integrators to keep it out of public logs, screenshots and client-side code.\n  sources: [https://legit.gonna.bond/docs]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gonna-bond/refs/heads/main/authentication/gonna-bond-authentication.yml
summary_line: none/x402 · 3 schemes
tags:
- Company
- Agents
- Agentic Commerce
- x402
- Trust
- Merchant Trust
- MCP
- A2A
- Algorand
- Blockchain
- Payments
- Agent-Native
---
