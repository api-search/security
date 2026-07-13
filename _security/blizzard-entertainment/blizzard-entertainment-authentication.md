---
api_key_in: []
api_specs:
- filename: blizzard-world-of-warcraft-openapi.yml
  format: yaml
  label: World of Warcraft Game Data API
  slug: world-of-warcraft-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blizzard-entertainment/refs/heads/main/openapi/blizzard-world-of-warcraft-openapi.yml
- filename: blizzard-diablo-iii-openapi.yml
  format: yaml
  label: Diablo III Community API
  slug: diablo-iii-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blizzard-entertainment/refs/heads/main/openapi/blizzard-diablo-iii-openapi.yml
- filename: blizzard-starcraft-ii-openapi.yml
  format: yaml
  label: StarCraft II Community API
  slug: starcraft-ii-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blizzard-entertainment/refs/heads/main/openapi/blizzard-starcraft-ii-openapi.yml
- filename: blizzard-hearthstone-openapi.yml
  format: yaml
  label: Hearthstone Game Data API
  slug: hearthstone-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blizzard-entertainment/refs/heads/main/openapi/blizzard-hearthstone-openapi.yml
- filename: blizzard-oauth-openapi.yml
  format: yaml
  label: Battle.net OAuth API
  slug: oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blizzard-entertainment/refs/heads/main/openapi/blizzard-oauth-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Blizzard Entertainment Authentication
name_suffix: Authentication
oauth_flows: []
overview: Blizzard Entertainment secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Blizzard Entertainment
provider_slug: blizzard-entertainment
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/blizzard-diablo-iii-openapi.yml
  - openapi/blizzard-hearthstone-openapi.yml
  - openapi/blizzard-oauth-openapi.yml
  - openapi/blizzard-starcraft-ii-openapi.yml
  - openapi/blizzard-world-of-warcraft-openapi.yml
  type: http
slug: blizzard-entertainment-authentication
source_filename: blizzard-entertainment-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/blizzard-diablo-iii-openapi.yml, openapi/blizzard-hearthstone-openapi.yml, openapi/blizzard-oauth-openapi.yml,\n  openapi/blizzard-starcraft-ii-openapi.yml, openapi/blizzard-world-of-warcraft-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/blizzard-diablo-iii-openapi.yml\n  - openapi/blizzard-hearthstone-openapi.yml\n  - openapi/blizzard-oauth-openapi.yml\n  - openapi/blizzard-starcraft-ii-openapi.yml\n  - openapi/blizzard-world-of-warcraft-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/blizzard-entertainment/refs/heads/main/authentication/blizzard-entertainment-authentication.yml
summary_line: http · 1 scheme
tags:
- Games
- Entertainment
- Video Games
- Game Data
- Battle.net
---
