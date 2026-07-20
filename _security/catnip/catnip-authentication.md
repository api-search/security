---
api_key_in:
- query
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: searched
name: Catnip Authentication
name_suffix: Authentication
oauth_flows: []
overview: Catnip secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Catnip
provider_slug: catnip
scheme_count: 2
schemes:
- applies_to:
  - Chatfuel Broadcasting API
  base_url: https://api.chatfuel.com
  description: A unique token issued per bot, passed as the chatfuel_token query parameter on every Broadcasting API request. Scopes the call to a single bot.
  docs: https://docs.chatfuel.com/en/articles/790461-broadcasting-api
  in: query
  name: BroadcastingToken
  parameter: chatfuel_token
  type: apiKey
- applies_to:
  - Chatfuel Dashboard API
  base_url: https://dashboard.chatfuel.com/api
  description: A Dashboard API Token generated from the account profile (profile photo → Dashboard API Token → generate). Sent as an Authorization Bearer header on every Dashboard API request. The Dashboard API is documented as primarily for internal use and subject to change.
  docs: https://docs.chatfuel.com/en/articles/2706667-dashboard-api
  header: 'Authorization: Bearer {token}'
  name: DashboardApiToken
  scheme: bearer
  type: http
slug: catnip-authentication
source_filename: catnip-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: >-\n  https://docs.chatfuel.com/en/articles/790461-broadcasting-api and\n  https://docs.chatfuel.com/en/articles/2706667-dashboard-api — Chatfuel publishes\n  no OpenAPI, so this auth profile is captured directly from the developer docs.\nprovider: Chatfuel\nproviderId: catnip\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - query\n  http_schemes:\n  - bearer\nschemes:\n- name: BroadcastingToken\n  type: apiKey\n  in: query\n  parameter: chatfuel_token\n  description: >-\n    A unique token issued per bot, passed as the chatfuel_token query parameter on\n    every Broadcasting API request. Scopes the call to a single bot.\n  applies_to:\n  - Chatfuel Broadcasting API\n  base_url: https://api.chatfuel.com\n  docs: https://docs.chatfuel.com/en/articles/790461-broadcasting-api\n- name: DashboardApiToken\n  type: http\n  scheme: bearer\n  description: >-\n    A Dashboard API Token generated from the account profile\
  \ (profile photo →\n    Dashboard API Token → generate). Sent as an Authorization Bearer header on every\n    Dashboard API request. The Dashboard API is documented as primarily for internal\n    use and subject to change.\n  applies_to:\n  - Chatfuel Dashboard API\n  base_url: https://dashboard.chatfuel.com/api\n  header: 'Authorization: Bearer {token}'\n  docs: https://docs.chatfuel.com/en/articles/2706667-dashboard-api\nnotes: >-\n  The JSON API plugin (https://docs.chatfuel.com/en/articles/735122-json-api) is an\n  outbound integration — the bot calls the developer's own backend — so its auth is\n  defined by the external endpoint, not by Chatfuel. No OAuth2/OIDC surface is\n  published.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/catnip/refs/heads/main/authentication/catnip-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Company
- Chatbots
- Messaging
- Conversational AI
- Marketing Automation
- Facebook Messenger
- Instagram
- WhatsApp
- Customer Engagement
---
