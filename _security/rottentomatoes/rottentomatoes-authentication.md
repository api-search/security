---
api_key_in:
- query
api_specs:
- filename: rottentomatoes-detailed-info-api-openapi.yml
  format: yaml
  label: Rotten Tomatoes Detailed Info API
  slug: rottentomatoes-detailed-info-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rottentomatoes/refs/heads/main/openapi/rottentomatoes-detailed-info-api-openapi.yml
- filename: rottentomatoes-dvd-lists-api-openapi.yml
  format: yaml
  label: Rotten Tomatoes DVD Lists API
  slug: rottentomatoes-dvd-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rottentomatoes/refs/heads/main/openapi/rottentomatoes-dvd-lists-api-openapi.yml
- filename: rottentomatoes-movie-lists-api-openapi.yml
  format: yaml
  label: Rotten Tomatoes Movie Lists API
  slug: rottentomatoes-movie-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rottentomatoes/refs/heads/main/openapi/rottentomatoes-movie-lists-api-openapi.yml
- filename: rottentomatoes-search-api-openapi.yml
  format: yaml
  label: Rotten Tomatoes Search API
  slug: rottentomatoes-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rottentomatoes/refs/heads/main/openapi/rottentomatoes-search-api-openapi.yml
- filename: rottentomatoes-top-level-lists-api-openapi.yml
  format: yaml
  label: Rotten Tomatoes Top Level Lists API
  slug: rottentomatoes-top-level-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rottentomatoes/refs/heads/main/openapi/rottentomatoes-top-level-lists-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Rottentomatoes Authentication
name_suffix: Authentication
oauth_flows: []
overview: Rotten Tomatoes secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Rotten Tomatoes
provider_slug: rottentomatoes
scheme_count: 1
schemes:
- in: query
  name: key
  parameter: apikey
  sources:
  - openapi/openapi.json
  type: apiKey
slug: rottentomatoes-authentication
source_filename: rottentomatoes-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: key\n  type: apiKey\n  in: query\n  parameter: apikey\n  sources:\n  - openapi/openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rottentomatoes/refs/heads/main/authentication/rottentomatoes-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Movies
- Television
- Reviews
- Ratings
- Tomatometer
- Audience Score
- Entertainment
- Media
---
