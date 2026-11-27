---
anonymous_access: false
api_key_in:
- cookie
api_specs:
- filename: meet-bot-api-v1-api-openapi.yml
  format: yaml
  label: Meet.bot API v1 API
  slug: meet-bot-api-v1-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/meet-bot/openapi/meet-bot-api-v1-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Meet.bot Authentication
name_suffix: Authentication
oauth_flows: []
overview: Meet.bot secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Meet.bot
provider_slug: meet-bot
scheme_count: 2
schemes:
- bearerFormat: opaque
  name: UserTokenAuthentication
  scheme: bearer
  sources:
  - openapi/meet-bot-openapi.yml
  type: http
- in: cookie
  name: cookieAuth
  parameter: sessionid
  sources:
  - openapi/meet-bot-openapi.yml
  type: apiKey
slug: meet-bot-authentication
source_filename: meet-bot-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: derived\nsource: openapi/meet-bot-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - cookie\nschemes:\n- name: UserTokenAuthentication\n  type: http\n  scheme: bearer\n  bearerFormat: opaque\n  sources:\n  - openapi/meet-bot-openapi.yml\n- name: cookieAuth\n  type: apiKey\n  in: cookie\n  parameter: sessionid\n  sources:\n  - openapi/meet-bot-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/meet-bot/authentication/meet-bot-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Scheduling
- AI Agents
- Integration
- Meetings
- Automation
---
