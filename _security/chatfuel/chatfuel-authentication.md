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
overview: Chatfuel secures its APIs with http and apiKey across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Chatfuel
provider_slug: chatfuel
scheme_count: 3
schemes:
- applies_to: Chatfuel Contacts API (https://panel.chatfuel.com/api)
  description: 'Account API token supplied as `Authorization: Bearer {your_api_token}`. Obtained from Settings -> API -> "Copy API key" inside the Chatfuel panel. Paired with an `{automation_id}` path parameter, read from the browser address bar of the automation being targeted.'
  name: PanelBearerToken
  scheme: bearer
  source: https://help.chatfuel.com/create-contacts-in-chatfuel-via-api-23134b06ecf8800683b6efacab24b68d
  status: current
  type: http
  verified: POST https://panel.chatfuel.com/api/contacts/{automation_id}/whatsapp/ with no Authorization header returned HTTP 401 on 2026-08-13, confirming the scheme is enforced.
- applies_to: Chatfuel Dashboard API (https://dashboard.chatfuel.com/api)
  description: 'Dashboard API Token supplied as `Authorization: Bearer {token}`. Was generated from the dashboard profile ("Dashboard API Token" -> "Generate Token"); shown once and had to be saved on creation or revoked and regenerated.'
  name: DashboardBearerToken
  note: 'Recorded from the previous enrichment round (2026-07-18), when this page was live. Re-probed 2026-08-13: docs.chatfuel.com returns HTTP 404 on every path — the Intercom help center behind it has been retired and no replacement page exists on help.chatfuel.com. Retained as history; not verifiable today.'
  scheme: bearer
  source: https://docs.chatfuel.com/api/dashboard-api
  source_status: 404
  status: undocumented
  type: http
- applies_to: Chatfuel Broadcasting API (https://api.chatfuel.com)
  description: Per-bot broadcasting token supplied as the `chatfuel_token` request parameter on Broadcasting API calls to https://api.chatfuel.com/bots/{BOT_ID}/users/{USER_ID}/send. Was retrieved from the bot's Configure tab -> "Broadcasting API Token".
  in: query
  name: BroadcastToken
  note: 'The route still exists — a GET against the send path returned HTTP 405 Method Not Allowed on 2026-08-13 rather than the host''s usual JSON 404 — but its documentation is gone. A query-string bearer credential is also the weakest placement available: it lands in proxy logs, browser history and Referer headers.'
  parameter: chatfuel_token
  source: https://docs.chatfuel.com/en/articles/790461-broadcasting-api
  source_status: 404
  status: undocumented
  type: apiKey
slug: chatfuel-authentication
source_filename: chatfuel-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://help.chatfuel.com/create-contacts-in-chatfuel-via-api-23134b06ecf8800683b6efacab24b68d\ndocs: https://help.chatfuel.com/other-guides-18234b06ecf8804cb046d94bbc701ff0\nsummary:\n  types:\n  - http\n  - apiKey\n  api_key_in:\n  - query\n  oauth2_flows: []\n  notes: >-\n    Chatfuel has no OpenAPI to derive from, so this profile is read from the\n    published docs. The current, documented scheme is a per-account Bearer API\n    token copied from Settings -> API in the Chatfuel panel and sent in the\n    Authorization header against panel.chatfuel.com. Two older schemes — the\n    Dashboard API bearer token and the per-bot chatfuel_token query parameter\n    for the Broadcasting API — were documented on docs.chatfuel.com, which\n    Chatfuel has since taken down; their hosts still answer, but the auth\n    documentation is gone. No OAuth 2.0 or OpenID Connect surface exists on any\n    host: /.well-known/openid-configuration\
  \ and\n    /.well-known/oauth-authorization-server were probed on api, panel,\n    dashboard, app and chatfuel.com and none returns a real document (see\n    well-known/chatfuel-well-known.yml).\nschemes:\n- name: PanelBearerToken\n  type: http\n  scheme: bearer\n  status: current\n  description: >-\n    Account API token supplied as `Authorization: Bearer {your_api_token}`.\n    Obtained from Settings -> API -> \"Copy API key\" inside the Chatfuel panel.\n    Paired with an `{automation_id}` path parameter, read from the browser\n    address bar of the automation being targeted.\n  applies_to: Chatfuel Contacts API (https://panel.chatfuel.com/api)\n  verified: >-\n    POST https://panel.chatfuel.com/api/contacts/{automation_id}/whatsapp/ with\n    no Authorization header returned HTTP 401 on 2026-08-13, confirming the\n    scheme is enforced.\n  source: https://help.chatfuel.com/create-contacts-in-chatfuel-via-api-23134b06ecf8800683b6efacab24b68d\n- name: DashboardBearerToken\n  type:\
  \ http\n  scheme: bearer\n  status: undocumented\n  description: >-\n    Dashboard API Token supplied as `Authorization: Bearer {token}`. Was\n    generated from the dashboard profile (\"Dashboard API Token\" -> \"Generate\n    Token\"); shown once and had to be saved on creation or revoked and\n    regenerated.\n  applies_to: Chatfuel Dashboard API (https://dashboard.chatfuel.com/api)\n  source: https://docs.chatfuel.com/api/dashboard-api\n  source_status: 404\n  note: >-\n    Recorded from the previous enrichment round (2026-07-18), when this page was\n    live. Re-probed 2026-08-13: docs.chatfuel.com returns HTTP 404 on every path\n    — the Intercom help center behind it has been retired and no replacement\n    page exists on help.chatfuel.com. Retained as history; not verifiable today.\n- name: BroadcastToken\n  type: apiKey\n  in: query\n  parameter: chatfuel_token\n  status: undocumented\n  description: >-\n    Per-bot broadcasting token supplied as the `chatfuel_token` request\n\
  \    parameter on Broadcasting API calls to\n    https://api.chatfuel.com/bots/{BOT_ID}/users/{USER_ID}/send. Was retrieved\n    from the bot's Configure tab -> \"Broadcasting API Token\".\n  applies_to: Chatfuel Broadcasting API (https://api.chatfuel.com)\n  source: https://docs.chatfuel.com/en/articles/790461-broadcasting-api\n  source_status: 404\n  note: >-\n    The route still exists — a GET against the send path returned HTTP 405\n    Method Not Allowed on 2026-08-13 rather than the host's usual JSON 404 — but\n    its documentation is gone. A query-string bearer credential is also the\n    weakest placement available: it lands in proxy logs, browser history and\n    Referer headers.\ngated_surfaces:\n- surface: https://api.chatfuel.com/swagger.json\n  observed: 302 -> accounts.google.com\n  detail: >-\n    The API host does serve a Swagger route, but it sits behind a Google-SSO\n    OAuth2 proxy: /swagger.json, /swagger and /swagger-ui all redirect to\n    accounts.google.com with\
  \ redirect_uri https://auth.chatfuel.com/oauth2/callback\n    and the original URL preserved in the state parameter, whereas every\n    undefined path on the same host returns a plain JSON 404. The contract\n    exists and is not public.\n- surface: https://panel.chatfuel.com/graphql\n  observed: 400 / introspection disabled\n  detail: >-\n    A live GraphQL endpoint answers with a real error envelope. Introspection is\n    switched off at the gateway — \"GraphQL introspection is disabled by Cosmo\n    Router\" — so no SDL can be read anonymously and none is published elsewhere.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chatfuel/refs/heads/main/authentication/chatfuel-authentication.yml
summary_line: http/apiKey · 3 schemes
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
- TikTok
- No-Code
- AI Agents
---
