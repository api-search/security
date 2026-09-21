---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 0
method: probed
name: Baconhollow Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: Bot Hub declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Bot Hub
provider_slug: baconhollow-com
scheme_count: 0
schemes: []
slug: baconhollow-com-authentication
source_filename: baconhollow-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: probed\nsource: https://baconhollow.com/.well-known/agent-card.json\nderived_from: a2a/baconhollow-com-agent-card.json\ndocs: []\nsummary:\n  types: []\n  model: >-\n    No authentication is declared or required on the published surface. The agent card carries no\n    securitySchemes and no security requirement, and the JSON-RPC endpoint at https://baconhollow.com\n    accepted an anonymous message/send on 2026-09-19 and answered with agent content. There is no\n    developer portal, sign-up page, API key issuance or OAuth metadata (/.well-known/openid-configuration,\n    /oauth-authorization-server and /oauth-protected-resource all 404). The card's own text says\n    \"All access is read-only.\"\nschemes: []\nobserved:\n- surface: A2A JSON-RPC (POST https://baconhollow.com/)\n  anonymous: true\n  evidence: 'message/send with a text part returned 200 and a role \"agent\" message without any credential; tasks/get returned -32001 Task not found,\
  \ not an auth error'\n- surface: agent/getAuthenticatedExtendedCard\n  result: '-32603 \"Authenticated card not supported\"'\n  evidence: consistent with no supportsAuthenticatedExtendedCard capability in the card\ngaps:\n- >-\n  The oracle-picks skill describes \"tier-based access\" and \"sign up for a buyer account\", so an\n  authorization boundary exists inside the conversation (which picks a caller may see), but nothing\n  published describes how a buyer identifies itself on a later call. Not probed: signing up would\n  have created an account.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/baconhollow-com/refs/heads/main/authentication/baconhollow-com-authentication.yml
summary_line: 0 schemes
tags:
- AI Agents
- A2A
- Autonomous Agents
- Prediction Markets
- Kalshi
- Trading Signals
- Weather
- agent-native
---
