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
overview: Catnip secures its APIs with apiKey and http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Catnip
provider_slug: catnip
scheme_count: 3
schemes:
- applies_to:
  - Chatfuel Contacts API
  base_url: https://panel.chatfuel.com/api
  description: An account API token generated in the product at Settings → API, sent as an Authorization Bearer header on Contacts API requests. The automation_id in the path (taken from the automation's URL) scopes the call to one automation.
  docs: https://help.chatfuel.com/create-contacts-in-chatfuel-via-api-23134b06ecf8800683b6efacab24b68d
  header: 'Authorization: Bearer {token}'
  name: ContactsApiToken
  observed:
    body: empty
    probe: POST /api/contacts/{automation_id}/whatsapp/ with no Authorization header
    status: 401
    trace_header: chatfuel-trace-id
  scheme: bearer
  token_source: Settings → API (in-product)
  type: http
- applies_to:
  - Chatfuel Broadcasting API
  base_url: https://api.chatfuel.com
  description: A unique token issued per bot, passed as the chatfuel_token query parameter on every Broadcasting API request. Scopes the call to a single bot. Carrying the credential in the query string means it is logged by every intermediary — an agent should treat the token as exposed.
  docs: null
  docs_retired: https://docs.chatfuel.com/en/articles/790461-broadcasting-api
  docs_status: 404
  in: query
  name: BroadcastingToken
  observed:
    body: '{"result":"Bad Request: Missing required chatfuel_token parameter","success":false,...}'
    note: 'With an unrecognised token the API answers 422 "Bad Data: Bot not found" rather than 401/403, so a bad credential and a bad bot id are indistinguishable.'
    probe: POST /bots/{bot_id}/users/{user_id}/send with no token
    status: 400
  parameter: chatfuel_token
  type: apiKey
- applies_to:
  - Chatfuel Dashboard API
  base_url: https://dashboard.chatfuel.com/api
  description: A Dashboard API Token generated from the account profile (profile photo → Dashboard API Token → generate). Sent as an Authorization Bearer header on every Dashboard API request. The Dashboard API was documented as primarily for internal use and subject to change.
  docs: null
  docs_retired: https://docs.chatfuel.com/en/articles/2706667-dashboard-api
  docs_status: 404
  header: 'Authorization: Bearer {token}'
  name: DashboardApiToken
  observed:
    body: '{"result":"User not found","success":false,"errors":["User not found"],"message":null}'
    probe: GET /api/bots with no Authorization header
    status: 401
  scheme: bearer
  type: http
slug: catnip-authentication
source_filename: catnip-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: >-\n  https://help.chatfuel.com/create-contacts-in-chatfuel-via-api-23134b06ecf8800683b6efacab24b68d\n  (the only live Chatfuel API reference as of 2026-08-13), plus live 400/401/422\n  probes of https://api.chatfuel.com, https://dashboard.chatfuel.com/api and\n  https://panel.chatfuel.com/api. Chatfuel publishes no OpenAPI, so this auth\n  profile is captured from documentation and observed responses.\nprovider: Chatfuel\nproviderId: catnip\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - query\n  http_schemes:\n  - bearer\n  oauth2_flows: []\n  openid_connect: false\n  mutual_tls: false\nschemes:\n- name: ContactsApiToken\n  type: http\n  scheme: bearer\n  description: >-\n    An account API token generated in the product at Settings → API, sent as an\n    Authorization Bearer header on Contacts API requests. The automation_id in the\n    path (taken from the automation's URL) scopes the call to one automation.\n\
  \  applies_to:\n  - Chatfuel Contacts API\n  base_url: https://panel.chatfuel.com/api\n  header: 'Authorization: Bearer {token}'\n  token_source: Settings → API (in-product)\n  docs: https://help.chatfuel.com/create-contacts-in-chatfuel-via-api-23134b06ecf8800683b6efacab24b68d\n  observed:\n    probe: POST /api/contacts/{automation_id}/whatsapp/ with no Authorization header\n    status: 401\n    body: empty\n    trace_header: chatfuel-trace-id\n- name: BroadcastingToken\n  type: apiKey\n  in: query\n  parameter: chatfuel_token\n  description: >-\n    A unique token issued per bot, passed as the chatfuel_token query parameter on\n    every Broadcasting API request. Scopes the call to a single bot. Carrying the\n    credential in the query string means it is logged by every intermediary — an\n    agent should treat the token as exposed.\n  applies_to:\n  - Chatfuel Broadcasting API\n  base_url: https://api.chatfuel.com\n  docs: null\n  docs_retired: https://docs.chatfuel.com/en/articles/790461-broadcasting-api\n\
  \  docs_status: 404\n  observed:\n    probe: POST /bots/{bot_id}/users/{user_id}/send with no token\n    status: 400\n    body: '{\"result\":\"Bad Request: Missing required chatfuel_token parameter\",\"success\":false,...}'\n    note: >-\n      With an unrecognised token the API answers 422 \"Bad Data: Bot not found\"\n      rather than 401/403, so a bad credential and a bad bot id are indistinguishable.\n- name: DashboardApiToken\n  type: http\n  scheme: bearer\n  description: >-\n    A Dashboard API Token generated from the account profile (profile photo →\n    Dashboard API Token → generate). Sent as an Authorization Bearer header on every\n    Dashboard API request. The Dashboard API was documented as primarily for\n    internal use and subject to change.\n  applies_to:\n  - Chatfuel Dashboard API\n  base_url: https://dashboard.chatfuel.com/api\n  header: 'Authorization: Bearer {token}'\n  docs: null\n  docs_retired: https://docs.chatfuel.com/en/articles/2706667-dashboard-api\n  docs_status:\
  \ 404\n  observed:\n    probe: GET /api/bots with no Authorization header\n    status: 401\n    body: '{\"result\":\"User not found\",\"success\":false,\"errors\":[\"User not found\"],\"message\":null}'\nscopes:\n  supported: false\n  note: >-\n    No OAuth2 or scope surface exists. Tokens are all-or-nothing at the bot,\n    automation or account level; there is no way to issue a read-only or\n    least-privilege credential, which is the sharpest auth gap for agent use.\nrotation:\n  documented: false\n  note: No token rotation, expiry or revocation policy is published for any of the three tokens.\nnotes: >-\n  The JSON API plugin (formerly documented at\n  https://docs.chatfuel.com/en/articles/735122-json-api, now 404) is an outbound\n  integration — the bot calls the developer's own backend — so its auth is defined\n  by the external endpoint, not by Chatfuel. No OAuth2, OIDC or mTLS surface is\n  published: /.well-known/oauth-authorization-server and\n  /.well-known/openid-configuration\
  \ 404 on every real Chatfuel host.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/catnip/refs/heads/main/authentication/catnip-authentication.yml
summary_line: apiKey/http · 3 schemes
tags:
- Company
- Chatbots
- Messaging
- Conversational AI
- Marketing Automation
- Facebook Messenger
- Instagram
- WhatsApp
- TikTok
- Customer Engagement
- Lead Qualification
---
