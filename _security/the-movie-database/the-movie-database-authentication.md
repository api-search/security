---
api_key_in:
- header
api_specs:
- filename: tmdb-api.json
  format: json
  label: The Movie Database API
  slug: the-movie-database
  spec_type: OpenAPI
  url: https://developer.themoviedb.org/openapi/tmdb-api.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: The Movie Database Authentication
name_suffix: Authentication
oauth_flows: []
overview: The Movie Database secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: The Movie Database
provider_slug: the-movie-database
scheme_count: 1
schemes:
- in: header
  name: sec0
  parameter: Authorization
  sources:
  - openapi/the-movie-database-openapi.json
  type: apiKey
slug: the-movie-database-authentication
source_filename: the-movie-database-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/the-movie-database-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: sec0\n  type: apiKey\n  in: header\n  parameter: Authorization\n  sources:\n  - openapi/the-movie-database-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/the-movie-database/refs/heads/main/authentication/the-movie-database-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Entertainment
- Movies
- Television
---
