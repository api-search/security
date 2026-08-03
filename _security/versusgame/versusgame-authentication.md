---
api_key_in:
- header
api_specs:
- filename: versusgame-openapi-original.json
  format: json
  label: Versusgame API
  slug: versusgame-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/versusgame/refs/heads/main/openapi/versusgame-openapi-original.json
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Versusgame Authentication
name_suffix: Authentication
oauth_flows: []
overview: VersusGame secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: VersusGame
provider_slug: versusgame
scheme_count: 2
schemes:
- bearerFormat: JWT
  description: Enter the bearer token below (do not include 'Bearer')
  name: access-token
  scheme: bearer
  sources:
  - openapi/versusgame-openapi-original.json
  type: http
- description: API Key For External calls
  in: header
  name: x-api-key
  parameter: x-api-key
  sources:
  - openapi/versusgame-openapi-original.json
  type: apiKey
slug: versusgame-authentication
source_filename: versusgame-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: derived\nsource: openapi/versusgame-openapi-original.json\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: access-token\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: Enter the bearer token below (do not include 'Bearer')\n  sources:\n  - openapi/versusgame-openapi-original.json\n- name: x-api-key\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: API Key For External calls\n  sources:\n  - openapi/versusgame-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/versusgame/refs/heads/main/authentication/versusgame-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Company
- gaming
- prediction-games
- audience-engagement
- gamification
- media-and-entertainment
- publishing
- widgets
- leaderboards
- creator-economy
- ai-content-generation
- payments
---
