---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: CodaPhone Authentication
name_suffix: Authentication
oauth_flows: []
overview: CodaPhone declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: CodaPhone
provider_slug: codaphone-app
scheme_count: 2
schemes:
- docs: https://codaphone.app/docs/api
  format: 'Authorization: Bearer cp_test_... | cp_live_...'
  header: Authorization
  in: header
  name: bearerApiKey
  scheme: bearer
  type: http
- docs: https://codaphone.app/docs/api
  header: x-api-key
  in: header
  name: apiKeyHeader
  note: '"The header x-api-key: <key> is also accepted."'
  type: apiKey
slug: codaphone-app-authentication
source_filename: codaphone-app-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://codaphone.app/docs/api\ndocs: https://codaphone.app/docs/api\nsummary: 'Every request is authenticated with an API key created in the dashboard (Settings -> API keys), sent as a bearer token in the Authorization header; the header x-api-key is also accepted. The full key is shown once at creation; only its prefix is viewable afterward. Keys are test (cp_test_) or live (cp_live_) and carry one or more scopes; a missing scope returns 403 insufficient_scope naming required_scope. The hosted MCP server (https://mcp.codaphone.app) uses the same API key as a bearer token. No OAuth is documented.'\nschemes:\n- name: bearerApiKey\n  type: http\n  scheme: bearer\n  in: header\n  header: Authorization\n  format: 'Authorization: Bearer cp_test_... | cp_live_...'\n  docs: https://codaphone.app/docs/api\n- name: apiKeyHeader\n  type: apiKey\n  in: header\n  header: x-api-key\n  note: '\"The header x-api-key: <key> is also accepted.\"\
  '\n  docs: https://codaphone.app/docs/api\nkey_prefixes:\n- prefix: cp_test_\n  meaning: the simulated path; nothing is sent to a real phone and no number is purchased\n- prefix: cp_live_\n  meaning: the live path (enabled as your account is approved)\nkey_scopes:\n- {scope: read, description: 'read account, numbers, messages, threads, contacts, lists, campaigns, and webhooks'}\n- {scope: send, description: send messages}\n- {scope: contacts, description: 'create contacts and lists, and import into a list'}\n- {scope: campaigns, description: create and control campaigns}\n- {scope: numbers, description: search for and provision numbers}\n- {scope: webhooks, description: 'register and delete webhook endpoints (listing them stays under read)'}\nwebhook_signing:\n  header: X-CodaPhone-Signature\n  algorithm: HMAC-SHA256 of the raw request body using the per-webhook signing secret\n  format: sha256=<hex>\n  secret_prefix: cpwh_\n"
source_yaml_url: https://artifacts.apis.io/codaphone-app/authentication/codaphone-app-authentication.yml
summary_line: 2 schemes
tags:
- Company
- SMS
- Business Texting
- Messaging
- Shared Inbox
- SMS Campaigns
- 10DLC
- Webhook
- MCP
---
