---
api_key_in: []
api_specs:
- filename: pandascore-changes-api-openapi.yml
  format: yaml
  label: PandaScore Changes API
  slug: pandascore-changes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pandascore/refs/heads/main/openapi/pandascore-changes-api-openapi.yml
- filename: pandascore-game-cs-go-api-openapi.yml
  format: yaml
  label: PandaScore Game - CS:GO API
  slug: pandascore-game-cs-go-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pandascore/refs/heads/main/openapi/pandascore-game-cs-go-api-openapi.yml
- filename: pandascore-game-dota-2-api-openapi.yml
  format: yaml
  label: PandaScore Game - Dota 2 API
  slug: pandascore-game-dota-2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pandascore/refs/heads/main/openapi/pandascore-game-dota-2-api-openapi.yml
- filename: pandascore-game-league-of-legends-api-openapi.yml
  format: yaml
  label: PandaScore Game - League of Legends API
  slug: pandascore-game-league-of-legends-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pandascore/refs/heads/main/openapi/pandascore-game-league-of-legends-api-openapi.yml
- filename: pandascore-game-valorant-api-openapi.yml
  format: yaml
  label: PandaScore Game - Valorant API
  slug: pandascore-game-valorant-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pandascore/refs/heads/main/openapi/pandascore-game-valorant-api-openapi.yml
- filename: pandascore-leagues-api-openapi.yml
  format: yaml
  label: PandaScore Leagues API
  slug: pandascore-leagues-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pandascore/refs/heads/main/openapi/pandascore-leagues-api-openapi.yml
- filename: pandascore-matches-api-openapi.yml
  format: yaml
  label: PandaScore Matches API
  slug: pandascore-matches-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pandascore/refs/heads/main/openapi/pandascore-matches-api-openapi.yml
- filename: pandascore-players-api-openapi.yml
  format: yaml
  label: PandaScore Players API
  slug: pandascore-players-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pandascore/refs/heads/main/openapi/pandascore-players-api-openapi.yml
- filename: pandascore-series-api-openapi.yml
  format: yaml
  label: PandaScore Series API
  slug: pandascore-series-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pandascore/refs/heads/main/openapi/pandascore-series-api-openapi.yml
- filename: pandascore-teams-api-openapi.yml
  format: yaml
  label: PandaScore Teams API
  slug: pandascore-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pandascore/refs/heads/main/openapi/pandascore-teams-api-openapi.yml
- filename: pandascore-tournaments-api-openapi.yml
  format: yaml
  label: PandaScore Tournaments API
  slug: pandascore-tournaments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pandascore/refs/heads/main/openapi/pandascore-tournaments-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Pandascore Authentication
name_suffix: Authentication
oauth_flows: []
overview: PandaScore secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: PandaScore
provider_slug: pandascore
scheme_count: 1
schemes:
- description: Bearer token authentication using a PandaScore API token
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/pandascore-openapi.yml
  type: http
slug: pandascore-authentication
source_filename: pandascore-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/pandascore-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Bearer token authentication using a PandaScore API token\n  sources:\n  - openapi/pandascore-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pandascore/refs/heads/main/authentication/pandascore-authentication.yml
summary_line: http · 1 scheme
tags:
- Esports
- Odds
- Betting
- Live Data
- Stats
- Fantasy
- WebSocket
- REST
---
