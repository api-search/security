---
api_key_in: []
api_specs:
- filename: blizzard-entertainment-achievements-api-openapi.yml
  format: yaml
  label: Blizzard Entertainment Achievements API
  slug: blizzard-entertainment-achievements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blizzard-entertainment/refs/heads/main/openapi/blizzard-entertainment-achievements-api-openapi.yml
- filename: blizzard-entertainment-acts-api-openapi.yml
  format: yaml
  label: Blizzard Entertainment Acts API
  slug: blizzard-entertainment-acts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blizzard-entertainment/refs/heads/main/openapi/blizzard-entertainment-acts-api-openapi.yml
- filename: blizzard-entertainment-artisans-api-openapi.yml
  format: yaml
  label: Blizzard Entertainment Artisans API
  slug: blizzard-entertainment-artisans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blizzard-entertainment/refs/heads/main/openapi/blizzard-entertainment-artisans-api-openapi.yml
- filename: blizzard-entertainment-auctions-api-openapi.yml
  format: yaml
  label: Blizzard Entertainment Auctions API
  slug: blizzard-entertainment-auctions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blizzard-entertainment/refs/heads/main/openapi/blizzard-entertainment-auctions-api-openapi.yml
- filename: blizzard-entertainment-authorization-api-openapi.yml
  format: yaml
  label: Blizzard Entertainment Authorization API
  slug: blizzard-entertainment-authorization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blizzard-entertainment/refs/heads/main/openapi/blizzard-entertainment-authorization-api-openapi.yml
- filename: blizzard-entertainment-card-backs-api-openapi.yml
  format: yaml
  label: Blizzard Entertainment Card Backs API
  slug: blizzard-entertainment-card-backs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blizzard-entertainment/refs/heads/main/openapi/blizzard-entertainment-card-backs-api-openapi.yml
- filename: blizzard-entertainment-cards-api-openapi.yml
  format: yaml
  label: Blizzard Entertainment Cards API
  slug: blizzard-entertainment-cards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blizzard-entertainment/refs/heads/main/openapi/blizzard-entertainment-cards-api-openapi.yml
- filename: blizzard-entertainment-characters-api-openapi.yml
  format: yaml
  label: Blizzard Entertainment Characters API
  slug: blizzard-entertainment-characters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blizzard-entertainment/refs/heads/main/openapi/blizzard-entertainment-characters-api-openapi.yml
- filename: blizzard-entertainment-decks-api-openapi.yml
  format: yaml
  label: Blizzard Entertainment Decks API
  slug: blizzard-entertainment-decks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blizzard-entertainment/refs/heads/main/openapi/blizzard-entertainment-decks-api-openapi.yml
- filename: blizzard-entertainment-guilds-api-openapi.yml
  format: yaml
  label: Blizzard Entertainment Guilds API
  slug: blizzard-entertainment-guilds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blizzard-entertainment/refs/heads/main/openapi/blizzard-entertainment-guilds-api-openapi.yml
- filename: blizzard-entertainment-items-api-openapi.yml
  format: yaml
  label: Blizzard Entertainment Items API
  slug: blizzard-entertainment-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blizzard-entertainment/refs/heads/main/openapi/blizzard-entertainment-items-api-openapi.yml
- filename: blizzard-entertainment-ladders-api-openapi.yml
  format: yaml
  label: Blizzard Entertainment Ladders API
  slug: blizzard-entertainment-ladders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blizzard-entertainment/refs/heads/main/openapi/blizzard-entertainment-ladders-api-openapi.yml
- filename: blizzard-entertainment-metadata-api-openapi.yml
  format: yaml
  label: Blizzard Entertainment Metadata API
  slug: blizzard-entertainment-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blizzard-entertainment/refs/heads/main/openapi/blizzard-entertainment-metadata-api-openapi.yml
- filename: blizzard-entertainment-mounts-api-openapi.yml
  format: yaml
  label: Blizzard Entertainment Mounts API
  slug: blizzard-entertainment-mounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blizzard-entertainment/refs/heads/main/openapi/blizzard-entertainment-mounts-api-openapi.yml
- filename: blizzard-entertainment-profiles-api-openapi.yml
  format: yaml
  label: Blizzard Entertainment Profiles API
  slug: blizzard-entertainment-profiles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blizzard-entertainment/refs/heads/main/openapi/blizzard-entertainment-profiles-api-openapi.yml
- filename: blizzard-entertainment-realms-api-openapi.yml
  format: yaml
  label: Blizzard Entertainment Realms API
  slug: blizzard-entertainment-realms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blizzard-entertainment/refs/heads/main/openapi/blizzard-entertainment-realms-api-openapi.yml
- filename: blizzard-entertainment-token-api-openapi.yml
  format: yaml
  label: Blizzard Entertainment Token API
  slug: blizzard-entertainment-token-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blizzard-entertainment/refs/heads/main/openapi/blizzard-entertainment-token-api-openapi.yml
- filename: blizzard-entertainment-userinfo-api-openapi.yml
  format: yaml
  label: Blizzard Entertainment UserInfo API
  slug: blizzard-entertainment-userinfo-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blizzard-entertainment/refs/heads/main/openapi/blizzard-entertainment-userinfo-api-openapi.yml
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
