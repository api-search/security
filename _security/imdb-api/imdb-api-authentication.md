---
api_key_in:
- query
api_specs:
- filename: imdb-api-openapi.yml
  format: yaml
  label: IMDb-API
  slug: imdb-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/imdb-api/refs/heads/main/openapi/imdb-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Imdb Api Authentication
name_suffix: Authentication
oauth_flows: []
overview: IMDb-API secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: IMDb-API
provider_slug: imdb-api
scheme_count: 1
schemes:
- description: API key issued at https://tv-api.com after sign-up. Embedded directly in the request path for most endpoints.
  in: query
  name: ApiKeyInPath
  parameter: apiKey
  sources:
  - openapi/imdb-api-openapi.yml
  type: apiKey
slug: imdb-api-authentication
source_filename: imdb-api-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/imdb-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: ApiKeyInPath\n  type: apiKey\n  in: query\n  parameter: apiKey\n  description: API key issued at https://tv-api.com after sign-up. Embedded directly in the\n    request path for most endpoints.\n  sources:\n  - openapi/imdb-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/imdb-api/refs/heads/main/authentication/imdb-api-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Video
- Movies
- TV
- Entertainment
- Metadata
- Ratings
- Public APIs
---
