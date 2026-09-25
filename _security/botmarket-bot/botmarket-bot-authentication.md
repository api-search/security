---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 0
method: searched
name: Botmarket Bot Authentication
name_suffix: Authentication
oauth_flows: []
overview: KOA Labs declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: KOA Labs
provider_slug: botmarket-bot
scheme_count: 0
schemes: []
slug: botmarket-bot-authentication
source_filename: botmarket-bot-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: searched\nsource: https://botmarket.bot/llms.txt\ndocs:\n- https://botmarket.bot/llms.txt\n- https://botmarket.bot/.well-known/mcp/server-card.json\n- https://botmarket.bot/.well-known/ai-plugin.json\nsummary:\n  types: []\n  api_key_in: []\n  oauth2_flows: []\n  bearer: false\n  credential_classes: 0\n  headline: >-\n    No authentication of any kind. BotMarket's REST surface (/v1), MCP server (/mcp) and submission endpoint\n    (POST /v1/submit) are anonymous by design — \"Free for bots. No signup.\" and \"10 req/sec, 100/min,\n    1000/hour per IP. Free. No token required.\" (llms.txt). The MCP server card declares \"auth\":\"none\", the\n    ai-plugin manifest declares auth {type: none}, and every live probe (initialize, tools/list, tools/call\n    get_stats, GET /v1/mcps, /v1/agents, /v1/protocols, /v1/quests) succeeded with no credential. Access\n    control is per-IP rate limiting, not identity. No OAuth, no OIDC, no API keys, no bearer\
  \ tokens, and no\n    discovery documents on the host (/.well-known/openid-configuration, /oauth-authorization-server and\n    /oauth-protected-resource all 404).\nschemes: []\npayment_signals:\n  header: 'x-payment-optional: x402,mtp'\n  tip_url: https://botmarket.bot/payments\n  observed_on: every /v1 and /mcp response\n  note: >-\n    Optional agent-native tipping (x402 / MTP) advertised in a response header. It is not an auth scheme and\n    not a gate — no request returned 402 — so it is recorded here as a signal an agent may see, not as a\n    credential class.\nopenapi: null\nnote: >-\n  No OpenAPI exists to derive from (https://botmarket.bot/openapi.json is a 0-byte 404 despite being advertised\n  by llms.txt and ai-plugin.json), so derive-authentication.py had nothing to read; this profile is written\n  from the provider's published text and live probes.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/botmarket-bot/refs/heads/main/authentication/botmarket-bot-authentication.yml
summary_line: 0 schemes
tags:
- Agents
- MCP
- A2A
- Agent Discovery
- Marketplace
- Directory
- Protocol
- x402
- Open Data
- Agent-Native
- Non-Profit
- Mexico
---
