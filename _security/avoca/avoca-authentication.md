---
api_key_in: []
api_specs:
- filename: avoca-analytics-v1-api-openapi.yml
  format: yaml
  label: Avoca Analytics (v1) API
  slug: avoca-analytics-v1-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/avoca/refs/heads/main/openapi/avoca-analytics-v1-api-openapi.yml
- filename: avoca-calls-api-openapi.yml
  format: yaml
  label: Avoca Calls API
  slug: avoca-calls-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/avoca/refs/heads/main/openapi/avoca-calls-api-openapi.yml
- filename: avoca-coach-api-openapi.yml
  format: yaml
  label: Avoca Coach API
  slug: avoca-coach-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/avoca/refs/heads/main/openapi/avoca-coach-api-openapi.yml
- filename: avoca-leads-api-openapi.yml
  format: yaml
  label: Avoca Leads API
  slug: avoca-leads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/avoca/refs/heads/main/openapi/avoca-leads-api-openapi.yml
- filename: avoca-outbound-texting-api-openapi.yml
  format: yaml
  label: Avoca Outbound Texting API
  slug: avoca-outbound-texting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/avoca/refs/heads/main/openapi/avoca-outbound-texting-api-openapi.yml
- filename: avoca-scheduler-analytics-v0-api-openapi.yml
  format: yaml
  label: Avoca Scheduler Analytics (v0) API
  slug: avoca-scheduler-analytics-v0-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/avoca/refs/heads/main/openapi/avoca-scheduler-analytics-v0-api-openapi.yml
- filename: avoca-sessions-bookings-api-openapi.yml
  format: yaml
  label: Avoca Sessions & Bookings API
  slug: avoca-sessions-bookings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/avoca/refs/heads/main/openapi/avoca-sessions-bookings-api-openapi.yml
- filename: avoca-teams-api-openapi.yml
  format: yaml
  label: Avoca Teams API
  slug: avoca-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/avoca/refs/heads/main/openapi/avoca-teams-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Avoca Authentication
name_suffix: Authentication
oauth_flows: []
overview: Avoca secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Avoca
provider_slug: avoca
scheme_count: 1
schemes:
- description: 'API key in the format `avoca_<64 hex characters>`, presented as `Authorization: Bearer <API_KEY>` on every Enterprise API request.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/avoca-openapi-original.json
  type: http
slug: avoca-authentication
source_filename: avoca-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: openapi/avoca-openapi-original.json\ndocs: https://docs.avoca.ai/api-reference/authentication\nsummary:\n  types:\n  - http\n  scheme: bearer\n  api_key_format: avoca_<64 hex characters>\n  header: 'Authorization: Bearer <API_KEY>'\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: >-\n    API key in the format `avoca_<64 hex characters>`, presented as\n    `Authorization: Bearer <API_KEY>` on every Enterprise API request.\n  sources:\n  - openapi/avoca-openapi-original.json\n# Key types govern which teams/enterprises a key can reach (from the docs auth page).\nkey_types:\n- name: enterprise\n  scope: Single team; no additional headers required.\n- name: enterprise_all_teams\n  scope: >-\n    All teams within one enterprise. Requires the `x-team-id` header on v0\n    endpoints, or the team id in the URL path on v1 endpoints.\n- name: portfolio_all_teams\n  scope: >-\n    Multiple teams across potentially\
  \ different enterprises; same scoping rules\n    as enterprise_all_teams but excludes enterprise-specific routes.\n# Per-key permission scopes documented on the auth page. Missing scope => 403.\npermission_scopes:\n- scope: read:calls\n  description: Call records, metadata, and pre-call transfers.\n- scope: read:transcripts\n  description: Call transcripts.\n- scope: read:leads\n  description: Unified leads (v0) and the canonical leads feed (v1).\n- scope: read:teams\n  description: Listing accessible teams (multi-team keys only).\n- scope: read:coach\n  description: Coach evaluations, scores, and rubrics.\n- scope: read:scheduler_analytics\n  description: Scheduler analytics, sessions, bookings, and scheduler configs.\n- scope: read:outbound\n  description: Outbound texting feeds (campaign texts and customer events).\nteam_scoping:\n  header: x-team-id\n  note: >-\n    v0 endpoints resolve the team from the `x-team-id` header (or an optional\n    `team_id` query parameter); v1 endpoints\
  \ carry the team id in the URL path\n    (`/api/v1/teams/{teamId}/...`).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/avoca/refs/heads/main/authentication/avoca-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Artificial Intelligence
- Voice AI
- Conversational AI
- Customer Service
- Contact Center
- Home Services
- Field Service
- Scheduling
- Analytics
- Webhook
- Enterprise API
---
