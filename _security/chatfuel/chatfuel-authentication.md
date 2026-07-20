---
api_key_in:
- query
auth_types:
- http
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Chatfuel Authentication
name_suffix: Authentication
oauth_flows: []
overview: Chatfuel secures its APIs with http and apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Chatfuel
provider_slug: chatfuel
scheme_count: 2
schemes:
- applies_to: Chatfuel Dashboard API (https://dashboard.chatfuel.com/api)
  description: 'Dashboard API Token supplied as `Authorization: Bearer {token}`. Generated from the dashboard profile ("Dashboard API Token" -> "Generate Token"); shown once and must be saved on creation or revoked and regenerated.'
  name: DashboardBearerToken
  scheme: bearer
  source: https://docs.chatfuel.com/api/dashboard-api
  type: http
- applies_to: Chatfuel Broadcasting API (https://api.chatfuel.com)
  description: Per-bot broadcasting token supplied as the `chatfuel_token` request parameter on Broadcasting API calls to https://api.chatfuel.com/bots/{BOT_ID}/users/{USER_ID}/send.
  in: query
  name: BroadcastToken
  parameter: chatfuel_token
  source: https://docs.chatfuel.com/en/articles/790461-broadcasting-api
  type: apiKey
slug: chatfuel-authentication
source_filename: chatfuel-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://docs.chatfuel.com/api/dashboard-api\ndocs: https://docs.chatfuel.com/en/collections/168839-api\nsummary:\n  types:\n  - http\n  - apiKey\n  api_key_in:\n  - query\n  oauth2_flows: []\n  notes: >-\n    Chatfuel uses two distinct token schemes. The Dashboard API authenticates\n    with a Bearer \"Dashboard API Token\" in the Authorization header; the token is\n    generated once from the dashboard profile and cannot be retrieved again. The\n    Broadcasting API authenticates with a per-bot chatfuel_token passed as a\n    request parameter alongside the bot and user identifiers. No OAuth 2.0 or\n    OpenID Connect surface is documented.\nschemes:\n- name: DashboardBearerToken\n  type: http\n  scheme: bearer\n  description: >-\n    Dashboard API Token supplied as `Authorization: Bearer {token}`. Generated\n    from the dashboard profile (\"Dashboard API Token\" -> \"Generate Token\"); shown\n    once and must be saved on\
  \ creation or revoked and regenerated.\n  applies_to: Chatfuel Dashboard API (https://dashboard.chatfuel.com/api)\n  source: https://docs.chatfuel.com/api/dashboard-api\n- name: BroadcastToken\n  type: apiKey\n  in: query\n  parameter: chatfuel_token\n  description: >-\n    Per-bot broadcasting token supplied as the `chatfuel_token` request\n    parameter on Broadcasting API calls to\n    https://api.chatfuel.com/bots/{BOT_ID}/users/{USER_ID}/send.\n  applies_to: Chatfuel Broadcasting API (https://api.chatfuel.com)\n  source: https://docs.chatfuel.com/en/articles/790461-broadcasting-api\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chatfuel/refs/heads/main/authentication/chatfuel-authentication.yml
summary_line: http/apiKey · 2 schemes
tags:
- Company
- Chatbots
- Conversational AI
- Messaging
- Marketing Automation
- Customer Support
- WhatsApp
- Instagram
- Facebook Messenger
- No-Code
---
