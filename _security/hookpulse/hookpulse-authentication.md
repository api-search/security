---
anonymous_access: false
api_key_in: []
api_specs:
- filename: openapi.json
  format: json
  label: HookPulse API
  slug: hookpulse-api
  spec_type: OpenAPI
  url: https://hookpulse.net/openapi.json
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Hookpulse Authentication
name_suffix: Authentication
oauth_flows: []
overview: HookPulse secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: HookPulse
provider_slug: hookpulse
scheme_count: 1
schemes:
- description: 'Guest token (`POST /api/guest`) in `X-Guest-Token: hp_…` or `Authorization: Bearer hp_…`. A `sess_…` session also works.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/hookpulse-openapi.json
  type: http
slug: hookpulse-authentication
source_filename: hookpulse-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: searched\nsource: openapi/hookpulse-openapi.json\ndocs: https://hookpulse.net/api/\nsummary:\n  types:\n  - http\n  api_key_in: []\n  oauth2_flows: []\n  note: >-\n    The OpenAPI declares one bearer scheme, but the /api/ index documents six auth modes the routes\n    actually use — all bearer-token flavors plus anonymous; no OAuth2, no OIDC, no API-key\n    self-service portal. Tokens are minted by the API itself (guest) or by e-mail OTP (session).\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'Guest token (`POST /api/guest`) in `X-Guest-Token: hp_…` or `Authorization:\n    Bearer hp_…`. A `sess_…` session also works.'\n  sources:\n  - openapi/hookpulse-openapi.json\nmodes:\n- mode: none\n  description: Public, no credential — discovery documents, ingest (/in/:id), billing, templates, metrics, public status dashboards.\n- mode: guest\n  description: >-\n    Guest token from POST /api/guest, sent as X-Guest-Token:\
  \ hp_… or Authorization: Bearer hp_…;\n    the anonymous owner of monitors. A sess_… session also works on guest routes.\n- mode: session\n  description: 'Authorization: Bearer sess_… from the e-mail OTP flow (POST /api/auth/start → POST /api/auth/verify). Confirming the e-mail grants the 90-day trial.'\n- mode: hook\n  description: >-\n    The monitor's own token in ?token= or X-Hook-Token. Read-only (state and pings) — lets a\n    third-party dashboard watch a monitor without the owner credential.\n- mode: credito\n  description: 'Prepaid credit bearer in Authorization: Bearer cred_… (or X-Credito). A bearer of balance, not an account.'\n- mode: token\n  description: Operator token (METRICS_TOKEN) as Bearer or ?key= — enriches /api/metrics with payment data; operator-only.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hookpulse/refs/heads/main/authentication/hookpulse-authentication.yml
summary_line: http · 1 scheme
tags:
- Monitoring
- Observability
- Cron
- Webhooks
- Heartbeat
- Dead-mans-switch
- Alerting
- Status pages
- Agent-native
- MCP
- x402
- Micropayments
---
