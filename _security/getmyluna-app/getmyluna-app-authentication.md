---
anonymous_access: false
api_key_in:
- cookie
api_specs:
- filename: getmyluna-app-account-api-openapi.yml
  format: yaml
  label: Luna Account API
  slug: getmyluna-app-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getmyluna-app/openapi/getmyluna-app-account-api-openapi.yml
- filename: getmyluna-app-analytics-api-openapi.yml
  format: yaml
  label: Luna Analytics API
  slug: getmyluna-app-analytics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getmyluna-app/openapi/getmyluna-app-analytics-api-openapi.yml
- filename: getmyluna-app-ask-luna-api-openapi.yml
  format: yaml
  label: Luna Ask Luna API
  slug: getmyluna-app-ask-luna-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getmyluna-app/openapi/getmyluna-app-ask-luna-api-openapi.yml
- filename: getmyluna-app-discovery-api-openapi.yml
  format: yaml
  label: Luna Discovery API
  slug: getmyluna-app-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getmyluna-app/openapi/getmyluna-app-discovery-api-openapi.yml
- filename: getmyluna-app-insights-api-openapi.yml
  format: yaml
  label: Luna Insights API
  slug: getmyluna-app-insights-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getmyluna-app/openapi/getmyluna-app-insights-api-openapi.yml
- filename: getmyluna-app-profile-api-openapi.yml
  format: yaml
  label: Luna Profile API
  slug: getmyluna-app-profile-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getmyluna-app/openapi/getmyluna-app-profile-api-openapi.yml
- filename: getmyluna-app-tokens-api-openapi.yml
  format: yaml
  label: Luna Tokens API
  slug: getmyluna-app-tokens-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getmyluna-app/openapi/getmyluna-app-tokens-api-openapi.yml
- filename: getmyluna-app-tracker-api-openapi.yml
  format: yaml
  label: Luna Tracker API
  slug: getmyluna-app-tracker-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getmyluna-app/openapi/getmyluna-app-tracker-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Luna Authentication
name_suffix: Authentication
oauth_flows: []
overview: Luna secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Luna
provider_slug: getmyluna-app
scheme_count: 2
schemes:
- bearerFormat: opaque
  description: 'Token from Settings → Connect an assistant or `POST /api/vega/token`. Scopes: `read`, `write`. A `read` token gets `403 insufficient_scope` on any operation whose `x-required-scope` is `write`.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/getmyluna-app-openapi.json
  type: http
- description: Browser session set by `POST /login` or `POST /api/vega/onboard`.
  in: cookie
  name: sessionCookie
  parameter: luna_session
  sources:
  - openapi/getmyluna-app-openapi.json
  type: apiKey
slug: getmyluna-app-authentication
source_filename: getmyluna-app-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-10'\nmethod: derived\nsource: openapi/getmyluna-app-openapi.json\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - cookie\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: opaque\n  description: 'Token from Settings → Connect an assistant or `POST /api/vega/token`. Scopes:\n    `read`, `write`. A `read` token gets `403 insufficient_scope` on any operation whose `x-required-scope`\n    is `write`.'\n  sources:\n  - openapi/getmyluna-app-openapi.json\n- name: sessionCookie\n  type: apiKey\n  in: cookie\n  parameter: luna_session\n  description: Browser session set by `POST /login` or `POST /api/vega/onboard`.\n  sources:\n  - openapi/getmyluna-app-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/getmyluna-app/authentication/getmyluna-app-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Baby Tracker
- Shared Log
- Health Tracking
- Family Care
---
