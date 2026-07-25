---
api_key_in:
- query
api_specs:
- filename: entitysport-authentication-api-openapi.yml
  format: yaml
  label: Entity Sport Authentication API
  slug: entitysport-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/entitysport/refs/heads/main/openapi/entitysport-authentication-api-openapi.yml
- filename: entitysport-competitions-api-openapi.yml
  format: yaml
  label: Entity Sport Competitions API
  slug: entitysport-competitions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/entitysport/refs/heads/main/openapi/entitysport-competitions-api-openapi.yml
- filename: entitysport-fantasy-api-openapi.yml
  format: yaml
  label: Entity Sport Fantasy API
  slug: entitysport-fantasy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/entitysport/refs/heads/main/openapi/entitysport-fantasy-api-openapi.yml
- filename: entitysport-matches-api-openapi.yml
  format: yaml
  label: Entity Sport Matches API
  slug: entitysport-matches-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/entitysport/refs/heads/main/openapi/entitysport-matches-api-openapi.yml
- filename: entitysport-odds-api-openapi.yml
  format: yaml
  label: Entity Sport Odds API
  slug: entitysport-odds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/entitysport/refs/heads/main/openapi/entitysport-odds-api-openapi.yml
- filename: entitysport-players-api-openapi.yml
  format: yaml
  label: Entity Sport Players API
  slug: entitysport-players-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/entitysport/refs/heads/main/openapi/entitysport-players-api-openapi.yml
- filename: entitysport-scorecards-api-openapi.yml
  format: yaml
  label: Entity Sport Scorecards API
  slug: entitysport-scorecards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/entitysport/refs/heads/main/openapi/entitysport-scorecards-api-openapi.yml
- filename: entitysport-teams-api-openapi.yml
  format: yaml
  label: Entity Sport Teams API
  slug: entitysport-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/entitysport/refs/heads/main/openapi/entitysport-teams-api-openapi.yml
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
