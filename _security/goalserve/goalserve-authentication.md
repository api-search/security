---
api_key_in:
- path
api_specs:
- filename: goalserve-commentaries-api-openapi.yml
  format: yaml
  label: GoalServe Commentaries API
  slug: goalserve-commentaries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goalserve/refs/heads/main/openapi/goalserve-commentaries-api-openapi.yml
- filename: goalserve-fixtures-api-openapi.yml
  format: yaml
  label: GoalServe Fixtures API
  slug: goalserve-fixtures-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goalserve/refs/heads/main/openapi/goalserve-fixtures-api-openapi.yml
- filename: goalserve-live-scores-api-openapi.yml
  format: yaml
  label: GoalServe Live Scores API
  slug: goalserve-live-scores-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goalserve/refs/heads/main/openapi/goalserve-live-scores-api-openapi.yml
- filename: goalserve-player-data-api-openapi.yml
  format: yaml
  label: GoalServe Player Data API
  slug: goalserve-player-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goalserve/refs/heads/main/openapi/goalserve-player-data-api-openapi.yml
- filename: goalserve-standings-api-openapi.yml
  format: yaml
  label: GoalServe Standings API
  slug: goalserve-standings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goalserve/refs/heads/main/openapi/goalserve-standings-api-openapi.yml
- filename: goalserve-team-data-api-openapi.yml
  format: yaml
  label: GoalServe Team Data API
  slug: goalserve-team-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goalserve/refs/heads/main/openapi/goalserve-team-data-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Goalserve Authentication
name_suffix: Authentication
oauth_flows: []
overview: GoalServe secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: GoalServe
provider_slug: goalserve
scheme_count: 1
schemes:
- description: Unique GoalServe API access key supplied as the first path segment after `/getfeed/`. Issued on registration; in-play feeds also require the caller's IP address to be whitelisted.
  in: path
  name: ApiKeyInPath
  parameter: key
  sources:
  - openapi/goalserve-openapi.yml
  type: apiKey
slug: goalserve-authentication
source_filename: goalserve-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/goalserve-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - path\nschemes:\n- name: ApiKeyInPath\n  type: apiKey\n  in: path\n  parameter: key\n  description: Unique GoalServe API access key supplied as the first path segment after `/getfeed/`.\n    Issued on registration; in-play feeds also require the caller's IP address to be whitelisted.\n  sources:\n  - openapi/goalserve-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/goalserve/refs/heads/main/authentication/goalserve-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Sports Data
- Live Scores
- Odds
- Fixtures
- Soccer
---
