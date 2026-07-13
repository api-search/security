---
api_key_in: []
api_specs:
- filename: battle-net-hearthstone-game-data.yaml
  format: yaml
  label: Hearthstone Game Data API
  slug: hearthstone-game-data
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/battle-net/refs/heads/main/openapi/battle-net-hearthstone-game-data.yaml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Battle Net Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Battle.net secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Battle.net
provider_slug: battle-net
scheme_count: 1
schemes:
- description: Battle.net OAuth 2.0 authentication. Use client credentials flow for game data APIs.
  flows:
  - flow: clientCredentials
    scopes: 0
    tokenUrl: https://oauth.battle.net/token
  name: oauth2
  sources:
  - openapi/battle-net-hearthstone-game-data.yaml
  type: oauth2
slug: battle-net-authentication
source_filename: battle-net-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/battle-net-hearthstone-game-data.yaml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://oauth.battle.net/token\n    scopes: 0\n  description: Battle.net OAuth 2.0 authentication. Use client credentials flow for game data\n    APIs.\n  sources:\n  - openapi/battle-net-hearthstone-game-data.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/battle-net/refs/heads/main/authentication/battle-net-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Games
- Gaming
- Blizzard
- World Of Warcraft
- Diablo
- Hearthstone
- Starcraft
---
