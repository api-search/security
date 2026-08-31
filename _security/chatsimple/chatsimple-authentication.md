---
api_key_in:
- header
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Chatsimple Authentication
name_suffix: Authentication
oauth_flows: []
overview: Chatsimple secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Chatsimple
provider_slug: chatsimple
scheme_count: 1
schemes:
- applies_to:
  - GET https://api.expertise.ai/v0/users/zapier
  - POST https://api.expertise.ai/v0/users/zapier/subscribe
  - DELETE https://api.expertise.ai/v0/users/zapier/unsubscribe
  - GET https://api.expertise.ai/v0/users/zapier/get_leads
  description: The API key issued by Chatsimple / Expertise AI. Documented on every Zapier endpoint. Issued from the authenticated dashboard; the docs do not publish a key format or prefix.
  in: header
  name: apiKeyHeader
  parameter_name: X-API-KEY
  source: https://docs.expertise.ai/live/integrations/zapier
  type: apiKey
slug: chatsimple-authentication
source_filename: chatsimple-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://docs.expertise.ai/live/integrations/zapier\ndocs: https://docs.expertise.ai/live/integrations/zapier\nnote: >-\n  NOT DERIVED FROM A SPEC — Chatsimple / Expertise AI publishes no OpenAPI, so\n  derive-authentication.py had nothing to read. Everything below was read from\n  the provider's own published Zapier integration reference (the only page on\n  docs.expertise.ai that documents HTTP endpoints) and from live probes of the\n  API host. No scheme was invented.\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  oauth2_flows: []\n  oauth_supported: false\n  oauth_evidence: >-\n    api.expertise.ai implements the RFC 8414 / RFC 9728 discovery routes and\n    answers them with HTTP 404 and the JSON body {\"error\":\"oauth_not_supported\"}\n    — an explicit machine-readable statement that this API does not use OAuth.\n    scopes/ is therefore correctly skipped for this provider.\nschemes:\n- name: apiKeyHeader\n\
  \  type: apiKey\n  in: header\n  parameter_name: X-API-KEY\n  description: >-\n    The API key issued by Chatsimple / Expertise AI. Documented on every Zapier\n    endpoint. Issued from the authenticated dashboard; the docs do not publish a\n    key format or prefix.\n  source: https://docs.expertise.ai/live/integrations/zapier\n  applies_to:\n  - GET https://api.expertise.ai/v0/users/zapier\n  - POST https://api.expertise.ai/v0/users/zapier/subscribe\n  - DELETE https://api.expertise.ai/v0/users/zapier/unsubscribe\n  - GET https://api.expertise.ai/v0/users/zapier/get_leads\ntenancy_headers:\n- header: X-USER-ID\n  required: true\n  description: Identifies the Expertise AI account the call acts on behalf of.\n- header: X-CHATBOT-ID\n  required: true\n  description: Identifies the specific agent/chatbot within that account.\n- header: X-HTML-SNIPPET\n  required: false\n  description: >-\n    Used only on the connection/login call; the embed snippet is parsed\n    server-side to recover\
  \ user_id and chatbot_id.\n- header: X-HOOKURL\n  required: false\n  description: Target callback URL, sent on the webhook subscribe call.\ntenancy_note: >-\n  The API key alone does not scope a request. Every documented call also carries\n  X-USER-ID and X-CHATBOT-ID, so the effective credential is a triple\n  (key + account + agent) rather than a single bearer token. There is no scope,\n  permission or role vocabulary published anywhere.\nmcp:\n  endpoint: https://api.expertise.ai/mcp\n  auth: gated\n  observed: >-\n    Anonymous JSON-RPC initialize and tools/list both return HTTP 401 with\n    {\"error\":{\"code\":-32001,\"message\":\"Unauthorized\"}} and no WWW-Authenticate\n    header, so the challenge is not discoverable — a client cannot learn from\n    the response how to authenticate.\n  documented: false\n  documented_note: >-\n    The MCP server is not mentioned anywhere in the public documentation, so how\n    a caller obtains and presents credentials for it is unpublished.\n\
  console:\n  dashboard: https://my.expertise.ai\n  note: >-\n    API keys, the embed snippet and integration credentials are all issued from\n    the authenticated dashboard. API access itself is sold on the Enterprise\n    tier (\"Custom API integration\"), per the public pricing page.\ngaps:\n- No published authentication guide outside the Zapier page.\n- No key format, prefix, rotation policy, expiry or revocation procedure published.\n- No OAuth, no OIDC, no scopes, no mTLS.\n- MCP auth entirely undocumented.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chatsimple/refs/heads/main/authentication/chatsimple-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- AI Agents
- Conversational AI
- Chatbot
- Lead Generation
- Sales Automation
- CRM Integration
- Voice AI
- Go-To-Market
- Customer Engagement
---
