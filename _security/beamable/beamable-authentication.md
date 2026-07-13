---
api_key_in:
- header
api_specs:
- filename: beamable-player-accounts-openapi.yml
  format: yaml
  label: Beamable Player Accounts API
  slug: player-accounts
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beamable/refs/heads/main/openapi/beamable-player-accounts-openapi.yml
- filename: beamable-leaderboards-openapi.yml
  format: yaml
  label: Beamable Leaderboards API
  slug: leaderboards
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beamable/refs/heads/main/openapi/beamable-leaderboards-openapi.yml
- filename: beamable-live-events-openapi.yml
  format: yaml
  label: Beamable Live Events API
  slug: live-events
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beamable/refs/heads/main/openapi/beamable-live-events-openapi.yml
- filename: beamable-microservices-openapi.yml
  format: yaml
  label: Beamable Microservices API
  slug: microservices
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beamable/refs/heads/main/openapi/beamable-microservices-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Beamable Authentication
name_suffix: Authentication
oauth_flows: []
overview: Beamable secures its APIs with apiKey and http across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Beamable
provider_slug: beamable
scheme_count: 4
schemes:
- description: Signed Request authentication using project secret key.
  in: header
  name: server
  parameter: X-DE-SIGNATURE
  sources:
  - openapi/beamable-leaderboards-openapi.yml
  - openapi/beamable-live-events-openapi.yml
  - openapi/beamable-microservices-openapi.yml
  - openapi/beamable-player-accounts-openapi.yml
  type: apiKey
- bearerFormat: Bearer <Access Token>
  description: Bearer authentication with a player access token in the Authorization header.
  name: user
  scheme: bearer
  sources:
  - openapi/beamable-leaderboards-openapi.yml
  - openapi/beamable-live-events-openapi.yml
  - openapi/beamable-microservices-openapi.yml
  - openapi/beamable-player-accounts-openapi.yml
  type: http
- description: Gamer Tag of the player.
  in: header
  name: userRequired
  parameter: X-DE-GAMERTAG
  sources:
  - openapi/beamable-live-events-openapi.yml
  type: apiKey
- description: Customer and project scope. This should contain the '<customer-id>.<project-id>'.
  in: header
  name: scope
  parameter: X-DE-SCOPE
  sources:
  - openapi/beamable-live-events-openapi.yml
  type: apiKey
slug: beamable-authentication
source_filename: beamable-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/beamable-leaderboards-openapi.yml, openapi/beamable-live-events-openapi.yml,\n  openapi/beamable-microservices-openapi.yml, openapi/beamable-player-accounts-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: server\n  type: apiKey\n  in: header\n  parameter: X-DE-SIGNATURE\n  description: Signed Request authentication using project secret key.\n  sources:\n  - openapi/beamable-leaderboards-openapi.yml\n  - openapi/beamable-live-events-openapi.yml\n  - openapi/beamable-microservices-openapi.yml\n  - openapi/beamable-player-accounts-openapi.yml\n- name: user\n  type: http\n  scheme: bearer\n  bearerFormat: Bearer <Access Token>\n  description: Bearer authentication with a player access token in the Authorization header.\n  sources:\n  - openapi/beamable-leaderboards-openapi.yml\n  - openapi/beamable-live-events-openapi.yml\n  - openapi/beamable-microservices-openapi.yml\n\
  \  - openapi/beamable-player-accounts-openapi.yml\n- name: userRequired\n  type: apiKey\n  in: header\n  parameter: X-DE-GAMERTAG\n  description: Gamer Tag of the player.\n  sources:\n  - openapi/beamable-live-events-openapi.yml\n- name: scope\n  type: apiKey\n  in: header\n  parameter: X-DE-SCOPE\n  description: Customer and project scope. This should contain the '<customer-id>.<project-id>'.\n  sources:\n  - openapi/beamable-live-events-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/beamable/refs/heads/main/authentication/beamable-authentication.yml
summary_line: apiKey/http · 4 schemes
tags:
- Game Backend
- LiveOps
- Player Accounts
- Virtual Currency
- Inventory
- Leaderboards
- Matchmaking
- Microservices
- Unity
- Unreal
- Game Economy
- Analytics
---
