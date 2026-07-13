---
api_key_in:
- header
api_specs:
- filename: riot-games-league-of-legends-openapi.yml
  format: yaml
  label: League of Legends API
  slug: league-of-legends-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/riot-games/refs/heads/main/openapi/riot-games-league-of-legends-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Riot Games Authentication
name_suffix: Authentication
oauth_flows: []
overview: Riot Games secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Riot Games
provider_slug: riot-games
scheme_count: 1
schemes:
- in: header
  name: ApiKey
  parameter: X-Riot-Token
  sources:
  - openapi/riot-games-league-of-legends-openapi.yml
  type: apiKey
slug: riot-games-authentication
source_filename: riot-games-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/riot-games-league-of-legends-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKey\n  type: apiKey\n  in: header\n  parameter: X-Riot-Token\n  sources:\n  - openapi/riot-games-league-of-legends-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/riot-games/refs/heads/main/authentication/riot-games-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Esports
- Gaming
- League of Legends
- Legends of Runeterra
- Teamfight Tactics
- VALORANT
---
