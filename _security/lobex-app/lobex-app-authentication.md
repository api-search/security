---
anonymous_access: false
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Lobex Authentication
name_suffix: Authentication
oauth_flows: []
overview: Lobex secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Lobex
provider_slug: lobex-app
scheme_count: 1
schemes:
- bearerFormat: rk_live
  description: Module API key from POST /api/agent/register (rk_live_...)
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/lobex-app-openapi.json
  type: http
slug: lobex-app-authentication
source_filename: lobex-app-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-17'\nmethod: derived\nsource: openapi/lobex-app-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: rk_live\n  description: Module API key from POST /api/agent/register (rk_live_...)\n  sources:\n  - openapi/lobex-app-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/lobex-app/authentication/lobex-app-authentication.yml
summary_line: http · 1 scheme
tags:
- Artificial Intelligence
- Marketplace
- Agents
- Monetization
- Platform
---
