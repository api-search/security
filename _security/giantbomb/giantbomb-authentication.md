---
api_key_in:
- query
api_specs:
- filename: openapi.json
  format: json
  label: Giant Bomb API
  slug: giantbomb-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/giantbomb/refs/heads/main/openapi/openapi.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Giantbomb Authentication
name_suffix: Authentication
oauth_flows: []
overview: Giant Bomb secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Giant Bomb
provider_slug: giantbomb
scheme_count: 1
schemes:
- description: API key for authentication. Register at https://www.giantbomb.com/api/
  in: query
  name: apiKeyQuery
  parameter: api_key
  sources:
  - openapi/openapi.json
  type: apiKey
slug: giantbomb-authentication
source_filename: giantbomb-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: apiKeyQuery\n  type: apiKey\n  in: query\n  parameter: api_key\n  description: API key for authentication. Register at https://www.giantbomb.com/api/\n  sources:\n  - openapi/openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/giantbomb/refs/heads/main/authentication/giantbomb-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Entertainment
- Video Games
- Game Database
- Gaming
- Media
---
