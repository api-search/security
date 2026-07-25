---
api_key_in: []
api_specs:
- filename: wakatime-commits-api-openapi.yml
  format: yaml
  label: WakaTime Commits API
  slug: wakatime-commits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wakatime/refs/heads/main/openapi/wakatime-commits-api-openapi.yml
- filename: wakatime-custom-rules-api-openapi.yml
  format: yaml
  label: WakaTime Custom Rules API
  slug: wakatime-custom-rules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wakatime/refs/heads/main/openapi/wakatime-custom-rules-api-openapi.yml
- filename: wakatime-data-dumps-api-openapi.yml
  format: yaml
  label: WakaTime Data Dumps API
  slug: wakatime-data-dumps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wakatime/refs/heads/main/openapi/wakatime-data-dumps-api-openapi.yml
- filename: wakatime-durations-api-openapi.yml
  format: yaml
  label: WakaTime Durations API
  slug: wakatime-durations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wakatime/refs/heads/main/openapi/wakatime-durations-api-openapi.yml
- filename: wakatime-editors-api-openapi.yml
  format: yaml
  label: WakaTime Editors API
  slug: wakatime-editors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wakatime/refs/heads/main/openapi/wakatime-editors-api-openapi.yml
- filename: wakatime-external-durations-api-openapi.yml
  format: yaml
  label: WakaTime External Durations API
  slug: wakatime-external-durations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wakatime/refs/heads/main/openapi/wakatime-external-durations-api-openapi.yml
- filename: wakatime-goals-api-openapi.yml
  format: yaml
  label: WakaTime Goals API
  slug: wakatime-goals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wakatime/refs/heads/main/openapi/wakatime-goals-api-openapi.yml
- filename: wakatime-heartbeats-api-openapi.yml
  format: yaml
  label: WakaTime Heartbeats API
  slug: wakatime-heartbeats-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wakatime/refs/heads/main/openapi/wakatime-heartbeats-api-openapi.yml
- filename: wakatime-insights-api-openapi.yml
  format: yaml
  label: WakaTime Insights API
  slug: wakatime-insights-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wakatime/refs/heads/main/openapi/wakatime-insights-api-openapi.yml
- filename: wakatime-languages-api-openapi.yml
  format: yaml
  label: WakaTime Languages API
  slug: wakatime-languages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wakatime/refs/heads/main/openapi/wakatime-languages-api-openapi.yml
- filename: wakatime-leaderboards-api-openapi.yml
  format: yaml
  label: WakaTime Leaderboards API
  slug: wakatime-leaderboards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wakatime/refs/heads/main/openapi/wakatime-leaderboards-api-openapi.yml
- filename: wakatime-machines-api-openapi.yml
  format: yaml
  label: WakaTime Machines API
  slug: wakatime-machines-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wakatime/refs/heads/main/openapi/wakatime-machines-api-openapi.yml
- filename: wakatime-meta-api-openapi.yml
  format: yaml
  label: WakaTime Meta API
  slug: wakatime-meta-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wakatime/refs/heads/main/openapi/wakatime-meta-api-openapi.yml
- filename: wakatime-organizations-api-openapi.yml
  format: yaml
  label: WakaTime Organizations API
  slug: wakatime-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wakatime/refs/heads/main/openapi/wakatime-organizations-api-openapi.yml
- filename: wakatime-projects-api-openapi.yml
  format: yaml
  label: WakaTime Projects API
  slug: wakatime-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wakatime/refs/heads/main/openapi/wakatime-projects-api-openapi.yml
- filename: wakatime-stats-api-openapi.yml
  format: yaml
  label: WakaTime Stats API
  slug: wakatime-stats-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wakatime/refs/heads/main/openapi/wakatime-stats-api-openapi.yml
- filename: wakatime-status-bar-api-openapi.yml
  format: yaml
  label: WakaTime Status Bar API
  slug: wakatime-status-bar-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wakatime/refs/heads/main/openapi/wakatime-status-bar-api-openapi.yml
- filename: wakatime-summaries-api-openapi.yml
  format: yaml
  label: WakaTime Summaries API
  slug: wakatime-summaries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wakatime/refs/heads/main/openapi/wakatime-summaries-api-openapi.yml
- filename: wakatime-user-agents-api-openapi.yml
  format: yaml
  label: WakaTime User Agents API
  slug: wakatime-user-agents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wakatime/refs/heads/main/openapi/wakatime-user-agents-api-openapi.yml
- filename: wakatime-users-api-openapi.yml
  format: yaml
  label: WakaTime Users API
  slug: wakatime-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wakatime/refs/heads/main/openapi/wakatime-users-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Wakatime Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- implicit
overview: WakaTime secures its APIs with http and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and implicit flow(s).
provider_name: WakaTime
provider_slug: wakatime
scheme_count: 3
schemes:
- description: OAuth 2.0 authorization code flow.
  flows:
  - authorizationUrl: https://wakatime.com/oauth/authorize
    flow: authorizationCode
    scopes: 8
    tokenUrl: https://wakatime.com/oauth/token
  - authorizationUrl: https://wakatime.com/oauth/authorize
    flow: implicit
    scopes: 8
  name: oauth2
  sources:
  - openapi/wakatime-api-v1-openapi.yml
  type: oauth2
- description: HTTP Basic with the WakaTime API key as the username. Alternatively, pass `?api_key=...` as a query parameter.
  name: apiKey
  scheme: basic
  sources:
  - openapi/wakatime-api-v1-openapi.yml
  type: http
- description: OAuth access token in the Authorization header as `Bearer [example key]`.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/wakatime-api-v1-openapi.yml
  type: http
slug: wakatime-authentication
source_filename: wakatime-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/wakatime-api-v1-openapi.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  - implicit\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://wakatime.com/oauth/authorize\n    tokenUrl: https://wakatime.com/oauth/token\n    scopes: 8\n  - flow: implicit\n    authorizationUrl: https://wakatime.com/oauth/authorize\n    scopes: 8\n  description: OAuth 2.0 authorization code flow.\n  sources:\n  - openapi/wakatime-api-v1-openapi.yml\n- name: apiKey\n  type: http\n  scheme: basic\n  description: HTTP Basic with the WakaTime API key as the username. Alternatively, pass `?api_key=...`\n    as a query parameter.\n  sources:\n  - openapi/wakatime-api-v1-openapi.yml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: OAuth access token in the Authorization header as `Bearer [example key]`.\n  sources:\n  - openapi/wakatime-api-v1-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wakatime/refs/heads/main/authentication/wakatime-authentication.yml
summary_line: http/oauth2 · 3 schemes
tags:
- Developer Productivity
- Developer Tools
- Time Tracking
- Coding Analytics
- Leaderboards
- IDE Plugins
- Open Source
- Public APIs
---
