---
api_key_in: []
api_specs:
- filename: wakatime-api-v1-openapi.yml
  format: yaml
  label: WakaTime API v1
  slug: wakatime-api-v1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wakatime/refs/heads/main/openapi/wakatime-api-v1-openapi.yml
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
