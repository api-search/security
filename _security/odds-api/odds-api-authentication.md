---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: odds-api-openapi.json
  format: json
  label: Odds API REST
  slug: odds-api-rest
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/odds-api/refs/heads/main/openapi/odds-api-openapi.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Odds Api Authentication
name_suffix: Authentication
oauth_flows: []
overview: Odds API secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Odds API
provider_slug: odds-api
scheme_count: 1
schemes:
- description: Send your API key in this header on every request.
  in: header
  name: ApiKeyAuth
  parameter: X-API-Key
  sources:
  - openapi/odds-api-openapi.json
  type: apiKey
slug: odds-api-authentication
source_filename: odds-api-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-17'\nmethod: derived\nsource: openapi/odds-api-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: Send your API key in this header on every request.\n  sources:\n  - openapi/odds-api-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/odds-api/refs/heads/main/authentication/odds-api-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Sports
- Sports Betting
- betting-odds
- bookmaker-odds
- live-odds
- Sportsbook
- Racing
- REST
- Server-Sent Events
- WebSocket
- OpenAPI
- MCP
- agent-native
- llms-txt
- SDK
- Postman
---
