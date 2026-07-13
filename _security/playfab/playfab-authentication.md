---
api_key_in:
- header
api_specs:
- filename: playfab-openapi.yml
  format: yaml
  label: PlayFab Client API
  slug: playfab-client-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/playfab/refs/heads/main/openapi/playfab-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Playfab Authentication
name_suffix: Authentication
oauth_flows: []
overview: PlayFab secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: PlayFab
provider_slug: playfab
scheme_count: 2
schemes:
- description: 'Session ticket returned by a successful `LoginWith*` call. Required

    for all Client API operations other than login/registration.'
  in: header
  name: sessionTicket
  parameter: X-Authorization
  sources:
  - openapi/playfab-openapi.yml
  type: apiKey
- description: Entity token used for Entity-model API calls.
  in: header
  name: entityToken
  parameter: X-EntityToken
  sources:
  - openapi/playfab-openapi.yml
  type: apiKey
slug: playfab-authentication
source_filename: playfab-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/playfab-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: sessionTicket\n  type: apiKey\n  in: header\n  parameter: X-Authorization\n  description: |-\n    Session ticket returned by a successful `LoginWith*` call. Required\n    for all Client API operations other than login/registration.\n  sources:\n  - openapi/playfab-openapi.yml\n- name: entityToken\n  type: apiKey\n  in: header\n  parameter: X-EntityToken\n  description: Entity token used for Entity-model API calls.\n  sources:\n  - openapi/playfab-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/playfab/refs/heads/main/authentication/playfab-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Authentication
- Azure
- Backend
- BaaS
- CloudScript
- Economy
- Game Backend
- Game Development
- Games
- Leaderboards
- Matchmaking
- Microsoft
- Multiplayer
- PlayFab
- REST
---
