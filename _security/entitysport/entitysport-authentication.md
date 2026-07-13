---
api_key_in:
- query
api_specs:
- filename: entitysport-openapi.yml
  format: yaml
  label: Entity Sport Competitions API
  slug: competitions
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/entitysport/refs/heads/main/openapi/entitysport-openapi.yml
- filename: entitysport-openapi.yml
  format: yaml
  label: Entity Sport Matches & Live Scoring API
  slug: matches-live-scoring
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/entitysport/refs/heads/main/openapi/entitysport-openapi.yml
- filename: entitysport-openapi.yml
  format: yaml
  label: Entity Sport Scorecards API
  slug: scorecards
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/entitysport/refs/heads/main/openapi/entitysport-openapi.yml
- filename: entitysport-openapi.yml
  format: yaml
  label: Entity Sport Fantasy Points API
  slug: fantasy-points
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/entitysport/refs/heads/main/openapi/entitysport-openapi.yml
- filename: entitysport-openapi.yml
  format: yaml
  label: Entity Sport Players & Teams API
  slug: players-teams
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/entitysport/refs/heads/main/openapi/entitysport-openapi.yml
- filename: entitysport-openapi.yml
  format: yaml
  label: Entity Sport Odds API
  slug: odds
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/entitysport/refs/heads/main/openapi/entitysport-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Entitysport Authentication
name_suffix: Authentication
oauth_flows: []
overview: Entity Sport secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Entity Sport
provider_slug: entitysport
scheme_count: 1
schemes:
- description: Short-lived access token obtained from POST /auth, passed as the `token` query parameter on every request.
  in: query
  name: accessToken
  parameter: token
  sources:
  - openapi/entitysport-openapi.yml
  type: apiKey
slug: entitysport-authentication
source_filename: entitysport-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/entitysport-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: accessToken\n  type: apiKey\n  in: query\n  parameter: token\n  description: Short-lived access token obtained from POST /auth, passed as the `token` query\n    parameter on every request.\n  sources:\n  - openapi/entitysport-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/entitysport/refs/heads/main/authentication/entitysport-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Sports Data
- Cricket
- Live Scores
- Fantasy
- Odds
---
