---
api_key_in:
- header
- query
api_specs:
- filename: therundown-v1-delta-api-openapi.yml
  format: yaml
  label: The Rundown V1 Delta API
  slug: therundown-v1-delta-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/therundown/refs/heads/main/openapi/therundown-v1-delta-api-openapi.yml
- filename: therundown-v1-events-api-openapi.yml
  format: yaml
  label: The Rundown V1 Events API
  slug: therundown-v1-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/therundown/refs/heads/main/openapi/therundown-v1-events-api-openapi.yml
- filename: therundown-v1-lines-api-openapi.yml
  format: yaml
  label: The Rundown V1 Lines API
  slug: therundown-v1-lines-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/therundown/refs/heads/main/openapi/therundown-v1-lines-api-openapi.yml
- filename: therundown-v1-reference-api-openapi.yml
  format: yaml
  label: The Rundown V1 Reference API
  slug: therundown-v1-reference-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/therundown/refs/heads/main/openapi/therundown-v1-reference-api-openapi.yml
- filename: therundown-v1-sports-api-openapi.yml
  format: yaml
  label: The Rundown V1 Sports API
  slug: therundown-v1-sports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/therundown/refs/heads/main/openapi/therundown-v1-sports-api-openapi.yml
- filename: therundown-v1-websocket-api-openapi.yml
  format: yaml
  label: The Rundown V1 WebSocket API
  slug: therundown-v1-websocket-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/therundown/refs/heads/main/openapi/therundown-v1-websocket-api-openapi.yml
- filename: therundown-v2-events-api-openapi.yml
  format: yaml
  label: The Rundown V2 Events API
  slug: therundown-v2-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/therundown/refs/heads/main/openapi/therundown-v2-events-api-openapi.yml
- filename: therundown-v2-markets-api-openapi.yml
  format: yaml
  label: The Rundown V2 Markets API
  slug: therundown-v2-markets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/therundown/refs/heads/main/openapi/therundown-v2-markets-api-openapi.yml
- filename: therundown-v2-players-api-openapi.yml
  format: yaml
  label: The Rundown V2 Players API
  slug: therundown-v2-players-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/therundown/refs/heads/main/openapi/therundown-v2-players-api-openapi.yml
- filename: therundown-v2-reference-api-openapi.yml
  format: yaml
  label: The Rundown V2 Reference API
  slug: therundown-v2-reference-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/therundown/refs/heads/main/openapi/therundown-v2-reference-api-openapi.yml
- filename: therundown-v2-sports-api-openapi.yml
  format: yaml
  label: The Rundown V2 Sports API
  slug: therundown-v2-sports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/therundown/refs/heads/main/openapi/therundown-v2-sports-api-openapi.yml
- filename: therundown-v2-stats-api-openapi.yml
  format: yaml
  label: The Rundown V2 Stats API
  slug: therundown-v2-stats-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/therundown/refs/heads/main/openapi/therundown-v2-stats-api-openapi.yml
- filename: therundown-v2-teams-api-openapi.yml
  format: yaml
  label: The Rundown V2 Teams API
  slug: therundown-v2-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/therundown/refs/heads/main/openapi/therundown-v2-teams-api-openapi.yml
- filename: therundown-v2-websocket-api-openapi.yml
  format: yaml
  label: The Rundown V2 WebSocket API
  slug: therundown-v2-websocket-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/therundown/refs/heads/main/openapi/therundown-v2-websocket-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Therundown Authentication
name_suffix: Authentication
oauth_flows: []
overview: The Rundown secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: The Rundown
provider_slug: therundown
scheme_count: 2
schemes:
- description: API key as query parameter
  in: query
  name: ApiKeyQuery
  parameter: key
  sources:
  - openapi/therundown-sports-odds-api-openapi.yml
  type: apiKey
- description: API key as request header
  in: header
  name: ApiKeyHeader
  parameter: X-Therundown-Key
  sources:
  - openapi/therundown-sports-odds-api-openapi.yml
  type: apiKey
slug: therundown-authentication
source_filename: therundown-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/therundown-sports-odds-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  - query\nschemes:\n- name: ApiKeyQuery\n  type: apiKey\n  in: query\n  parameter: key\n  description: API key as query parameter\n  sources:\n  - openapi/therundown-sports-odds-api-openapi.yml\n- name: ApiKeyHeader\n  type: apiKey\n  in: header\n  parameter: X-Therundown-Key\n  description: API key as request header\n  sources:\n  - openapi/therundown-sports-odds-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/therundown/refs/heads/main/authentication/therundown-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Sports
- Betting
- Odds
- NFL
- NBA
- MLB
- NHL
- Soccer
- Real-Time
- Sports Data
- Sportsbook
---
