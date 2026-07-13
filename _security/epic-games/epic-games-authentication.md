---
api_key_in: []
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Epic Games Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Epic Games secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Epic Games
provider_slug: epic-games
scheme_count: 2
schemes:
- flows:
  - flow: clientCredentials
    scopes: 1
    tokenUrl: https://api.epicgames.dev/auth/v1/oauth/token
  name: oauthClientCredentials
  sources:
  - openapi/epic-games-openapi.yml
  type: oauth2
- bearerFormat: JWT
  description: EOS bearer access token issued by the OAuth token endpoint.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/epic-games-openapi.yml
  type: http
slug: epic-games-authentication
source_filename: epic-games-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/epic-games-openapi.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: oauthClientCredentials\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.epicgames.dev/auth/v1/oauth/token\n    scopes: 1\n  sources:\n  - openapi/epic-games-openapi.yml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: EOS bearer access token issued by the OAuth token endpoint.\n  sources:\n  - openapi/epic-games-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/epic-games/refs/heads/main/authentication/epic-games-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Achievements
- Anti-Cheat
- Cross-Platform
- EOS
- Epic Online Services
- Game Backend
- Game Development
- Games
- Identity
- Lobby
- Matchmaking
- Multiplayer
- Sessions
- Unreal Engine
- Voice
---
