---
api_key_in:
- query
api_specs:
- filename: giantbomb-characters-api-openapi.yml
  format: yaml
  label: Giant Bomb Characters API
  slug: giantbomb-characters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/giantbomb/refs/heads/main/openapi/giantbomb-characters-api-openapi.yml
- filename: giantbomb-companies-api-openapi.yml
  format: yaml
  label: Giant Bomb Companies API
  slug: giantbomb-companies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/giantbomb/refs/heads/main/openapi/giantbomb-companies-api-openapi.yml
- filename: giantbomb-franchises-api-openapi.yml
  format: yaml
  label: Giant Bomb Franchises API
  slug: giantbomb-franchises-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/giantbomb/refs/heads/main/openapi/giantbomb-franchises-api-openapi.yml
- filename: giantbomb-games-api-openapi.yml
  format: yaml
  label: Giant Bomb Games API
  slug: giantbomb-games-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/giantbomb/refs/heads/main/openapi/giantbomb-games-api-openapi.yml
- filename: giantbomb-platforms-api-openapi.yml
  format: yaml
  label: Giant Bomb Platforms API
  slug: giantbomb-platforms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/giantbomb/refs/heads/main/openapi/giantbomb-platforms-api-openapi.yml
- filename: giantbomb-releases-api-openapi.yml
  format: yaml
  label: Giant Bomb Releases API
  slug: giantbomb-releases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/giantbomb/refs/heads/main/openapi/giantbomb-releases-api-openapi.yml
- filename: giantbomb-reviews-api-openapi.yml
  format: yaml
  label: Giant Bomb Reviews API
  slug: giantbomb-reviews-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/giantbomb/refs/heads/main/openapi/giantbomb-reviews-api-openapi.yml
- filename: giantbomb-search-api-openapi.yml
  format: yaml
  label: Giant Bomb Search API
  slug: giantbomb-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/giantbomb/refs/heads/main/openapi/giantbomb-search-api-openapi.yml
- filename: giantbomb-videos-api-openapi.yml
  format: yaml
  label: Giant Bomb Videos API
  slug: giantbomb-videos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/giantbomb/refs/heads/main/openapi/giantbomb-videos-api-openapi.yml
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
