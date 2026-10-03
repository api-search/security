---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: odds-api-account-api-openapi.yml
  format: yaml
  label: Odds API Account API
  slug: odds-api-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/odds-api/refs/heads/main/openapi/odds-api-account-api-openapi.yml
- filename: odds-api-betting-opportunities-api-openapi.yml
  format: yaml
  label: Odds API Betting opportunities API
  slug: odds-api-betting-opportunities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/odds-api/refs/heads/main/openapi/odds-api-betting-opportunities-api-openapi.yml
- filename: odds-api-catalog-api-openapi.yml
  format: yaml
  label: Odds API Catalog API
  slug: odds-api-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/odds-api/refs/heads/main/openapi/odds-api-catalog-api-openapi.yml
- filename: odds-api-prediction-markets-api-openapi.yml
  format: yaml
  label: Odds API Prediction markets API
  slug: odds-api-prediction-markets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/odds-api/refs/heads/main/openapi/odds-api-prediction-markets-api-openapi.yml
- filename: odds-api-racing-events-api-openapi.yml
  format: yaml
  label: Odds API Racing events API
  slug: odds-api-racing-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/odds-api/refs/heads/main/openapi/odds-api-racing-events-api-openapi.yml
- filename: odds-api-racing-odds-api-openapi.yml
  format: yaml
  label: Odds API Racing odds API
  slug: odds-api-racing-odds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/odds-api/refs/heads/main/openapi/odds-api-racing-odds-api-openapi.yml
- filename: odds-api-results-api-openapi.yml
  format: yaml
  label: Odds API Results API
  slug: odds-api-results-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/odds-api/refs/heads/main/openapi/odds-api-results-api-openapi.yml
- filename: odds-api-sports-events-api-openapi.yml
  format: yaml
  label: Odds API Sports events API
  slug: odds-api-sports-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/odds-api/refs/heads/main/openapi/odds-api-sports-events-api-openapi.yml
- filename: odds-api-sports-exchange-api-openapi.yml
  format: yaml
  label: Odds API Sports exchange API
  slug: odds-api-sports-exchange-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/odds-api/refs/heads/main/openapi/odds-api-sports-exchange-api-openapi.yml
- filename: odds-api-sports-odds-api-openapi.yml
  format: yaml
  label: Odds API Sports odds API
  slug: odds-api-sports-odds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/odds-api/refs/heads/main/openapi/odds-api-sports-odds-api-openapi.yml
- filename: odds-api-start-here-api-openapi.yml
  format: yaml
  label: Odds API Start here API
  slug: odds-api-start-here-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/odds-api/refs/heads/main/openapi/odds-api-start-here-api-openapi.yml
- filename: odds-api-status-api-openapi.yml
  format: yaml
  label: Odds API Status API
  slug: odds-api-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/odds-api/refs/heads/main/openapi/odds-api-status-api-openapi.yml
- filename: odds-api-widgets-api-openapi.yml
  format: yaml
  label: Odds API Widgets API
  slug: odds-api-widgets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/odds-api/refs/heads/main/openapi/odds-api-widgets-api-openapi.yml
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
- Agent-Native
- llms-txt
- SDK
- Postman
---
