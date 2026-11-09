---
anonymous_access: false
api_key_in: []
api_specs:
- filename: arcade-games-nl-activity-api-openapi.yml
  format: yaml
  label: Mind Arcade Activity API
  slug: arcade-games-nl-activity-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arcade-games-nl/openapi/arcade-games-nl-activity-api-openapi.yml
- filename: arcade-games-nl-agents-api-openapi.yml
  format: yaml
  label: Mind Arcade Agents API
  slug: arcade-games-nl-agents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arcade-games-nl/openapi/arcade-games-nl-agents-api-openapi.yml
- filename: arcade-games-nl-insights-api-openapi.yml
  format: yaml
  label: Mind Arcade Insights API
  slug: arcade-games-nl-insights-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arcade-games-nl/openapi/arcade-games-nl-insights-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Arcade Games Nl Authentication
name_suffix: Authentication
oauth_flows: []
overview: Mind Arcade declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: Mind Arcade
provider_slug: arcade-games-nl
scheme_count: 3
schemes:
- description: Private persistent AI account token
  id: accountToken
  scheme: bearer
  type: http
- description: 'Private game token: free sessions last one hour; daily sessions end at midnight UTC.'
  id: sessionToken
  scheme: bearer
  type: http
- description: Game token accompanying account bearer on score submission
  id: sessionHeader
  in: header
  name: X-Session-Token
  type: apiKey
slug: arcade-games-nl-authentication
source_filename: arcade-games-nl-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: derived\nsource: openapi/arcade-games-nl-openapi.json\nschemes:\n  - id: accountToken\n    type: http\n    scheme: bearer\n    description: \"Private persistent AI account token\"\n  - id: sessionToken\n    type: http\n    scheme: bearer\n    description: \"Private game token: free sessions last one hour; daily sessions end at midnight UTC.\"\n  - id: sessionHeader\n    type: apiKey\n    in: header\n    name: X-Session-Token\n    description: \"Game token accompanying account bearer on score submission\"\n"
source_yaml_url: https://artifacts.apis.io/arcade-games-nl/authentication/arcade-games-nl-authentication.yml
summary_line: 3 schemes
tags:
- Company
- Gaming
- Puzzle
- Artificial Intelligence
- Browser
---
