---
anonymous_access: true
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Coolant Authentication
name_suffix: Authentication
oauth_flows: []
overview: Coolant declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Coolant
provider_slug: coolant-run
scheme_count: 2
schemes:
- acquisition: GET /t/key (day pass) or GET /t/room_key (key plus room); unpaid requests receive HTTP 402 with x-402-price, x-402-network and x-402-address headers.
  applies_to: key-tier instruments over REST (/t/<instrument>) and MCP (/mcp)
  description: 'Instruments marked free need nothing. The rest need a room key: call GET /t/key ($0.01, settled over x402 on eip155:8453) and send the key back as "Authorization: Bearer <key>" on any request, REST or MCP. The key carries its own expiry and signature; no account is created.'
  header: 'Authorization: Bearer <key>'
  name: roomKey
  revocation: Keys cannot be revoked individually; rotating the server signing secret invalidates every key at once (https://coolant.run/terms).
  scheme: bearer
  type: http
- applies_to: free instruments, /cycle, /health, /.well-known/coolant.json
  name: none
  type: none
slug: coolant-run-authentication
source_filename: coolant-run-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://coolant.run/llms.txt\ndocs: https://coolant.run/how\nschemes:\n- name: roomKey\n  type: http\n  scheme: bearer\n  header: 'Authorization: Bearer <key>'\n  applies_to: key-tier instruments over REST (/t/<instrument>) and MCP (/mcp)\n  description: 'Instruments marked free need nothing. The rest need a room key: call GET /t/key ($0.01, settled over x402 on eip155:8453) and send the key back as \"Authorization: Bearer <key>\" on any request, REST or MCP. The key carries its own expiry and signature; no account is created.'\n  acquisition: GET /t/key (day pass) or GET /t/room_key (key plus room); unpaid requests receive HTTP 402 with x-402-price, x-402-network and x-402-address headers.\n  revocation: Keys cannot be revoked individually; rotating the server signing secret invalidates every key at once (https://coolant.run/terms).\n- name: none\n  type: none\n  applies_to: free instruments, /cycle, /health, /.well-known/coolant.json\n\
  payment_protocol:\n  name: x402\n  network: eip155:8453\n  facilitator: https://api.cdp.coinbase.com/platform/v2/x402\n  source: https://coolant.run/.well-known/coolant.json\nresponse_signing:\n  algorithm: Ed25519\n  key_id: 614b4d4f602cf6cc\n  input: canonical JSON of the response body with the \"sig\" field removed\n  encoding: base64url\n  source: https://coolant.run/.well-known/coolant.json\n"
source_yaml_url: https://artifacts.apis.io/coolant-run/authentication/coolant-run-authentication.yml
summary_line: 2 schemes
tags:
- Company
- AI Agents
- MCP
- x402
- Agent Tools
- Micropayments
- Developer Utilities
---
