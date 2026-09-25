---
anonymous_access: false
api_key_in: []
api_specs:
- filename: hookpulse-apis-json-api-openapi.yml
  format: yaml
  label: HookPulse Apis.json API
  slug: hookpulse-apis-json-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hookpulse/refs/heads/main/openapi/hookpulse-apis-json-api-openapi.yml
- filename: hookpulse-auth-api-openapi.yml
  format: yaml
  label: HookPulse Auth API
  slug: hookpulse-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hookpulse/refs/heads/main/openapi/hookpulse-auth-api-openapi.yml
- filename: hookpulse-billing-api-openapi.yml
  format: yaml
  label: HookPulse Billing API
  slug: hookpulse-billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hookpulse/refs/heads/main/openapi/hookpulse-billing-api-openapi.yml
- filename: hookpulse-contact-api-openapi.yml
  format: yaml
  label: HookPulse Contact API
  slug: hookpulse-contact-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hookpulse/refs/heads/main/openapi/hookpulse-contact-api-openapi.yml
- filename: hookpulse-credito-api-openapi.yml
  format: yaml
  label: HookPulse Credito API
  slug: hookpulse-credito-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hookpulse/refs/heads/main/openapi/hookpulse-credito-api-openapi.yml
- filename: hookpulse-endpoints-api-openapi.yml
  format: yaml
  label: HookPulse Endpoints API
  slug: hookpulse-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hookpulse/refs/heads/main/openapi/hookpulse-endpoints-api-openapi.yml
- filename: hookpulse-guest-api-openapi.yml
  format: yaml
  label: HookPulse Guest API
  slug: hookpulse-guest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hookpulse/refs/heads/main/openapi/hookpulse-guest-api-openapi.yml
- filename: hookpulse-health-api-openapi.yml
  format: yaml
  label: HookPulse Health API
  slug: hookpulse-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hookpulse/refs/heads/main/openapi/hookpulse-health-api-openapi.yml
- filename: hookpulse-hookpulse-api-openapi.yml
  format: yaml
  label: HookPulse Hook Pulse API
  slug: hookpulse-hookpulse-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hookpulse/refs/heads/main/openapi/hookpulse-hookpulse-api-openapi.yml
- filename: hookpulse-in-api-openapi.yml
  format: yaml
  label: HookPulse In API
  slug: hookpulse-in-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hookpulse/refs/heads/main/openapi/hookpulse-in-api-openapi.yml
- filename: hookpulse-mcp-api-openapi.yml
  format: yaml
  label: HookPulse MCP API
  slug: hookpulse-mcp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hookpulse/refs/heads/main/openapi/hookpulse-mcp-api-openapi.yml
- filename: hookpulse-me-api-openapi.yml
  format: yaml
  label: HookPulse Me API
  slug: hookpulse-me-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hookpulse/refs/heads/main/openapi/hookpulse-me-api-openapi.yml
- filename: hookpulse-metrics-api-openapi.yml
  format: yaml
  label: HookPulse Metrics API
  slug: hookpulse-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hookpulse/refs/heads/main/openapi/hookpulse-metrics-api-openapi.yml
- filename: hookpulse-okf-api-openapi.yml
  format: yaml
  label: HookPulse Okf API
  slug: hookpulse-okf-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hookpulse/refs/heads/main/openapi/hookpulse-okf-api-openapi.yml
- filename: hookpulse-s-api-openapi.yml
  format: yaml
  label: HookPulse S API
  slug: hookpulse-s-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hookpulse/refs/heads/main/openapi/hookpulse-s-api-openapi.yml
- filename: hookpulse-status-feed-api-openapi.yml
  format: yaml
  label: HookPulse Status Feed API
  slug: hookpulse-status-feed-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hookpulse/refs/heads/main/openapi/hookpulse-status-feed-api-openapi.yml
- filename: hookpulse-templates-api-openapi.yml
  format: yaml
  label: HookPulse Templates API
  slug: hookpulse-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hookpulse/refs/heads/main/openapi/hookpulse-templates-api-openapi.yml
- filename: hookpulse-visit-api-openapi.yml
  format: yaml
  label: HookPulse Visit API
  slug: hookpulse-visit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hookpulse/refs/heads/main/openapi/hookpulse-visit-api-openapi.yml
- filename: hookpulse-well-known-api-openapi.yml
  format: yaml
  label: HookPulse .well Known API
  slug: hookpulse-well-known-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hookpulse/refs/heads/main/openapi/hookpulse-well-known-api-openapi.yml
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
- Webhook
- Heartbeat
- Dead-mans-switch
- Alerting
- Status Pages
- Agent-Native
- MCP
- x402
- Micropayments
---
