---
api_key_in:
- query
api_specs:
- filename: the-open-movie-database-openapi.yml
  format: yaml
  label: The Open Movie Database API
  slug: the-open-movie-database
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/the-open-movie-database/refs/heads/main/openapi/the-open-movie-database-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: The Open Movie Database Authentication
name_suffix: Authentication
oauth_flows: []
overview: The Open Movie Database secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: The Open Movie Database
provider_slug: the-open-movie-database
scheme_count: 1
schemes:
- in: query
  name: apiKey
  parameter: apikey
  sources:
  - openapi/the-open-movie-database-openapi.yml
  type: apiKey
slug: the-open-movie-database-authentication
source_filename: the-open-movie-database-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/the-open-movie-database-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: apiKey\n  type: apiKey\n  in: query\n  parameter: apikey\n  sources:\n  - openapi/the-open-movie-database-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/the-open-movie-database/refs/heads/main/authentication/the-open-movie-database-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Entertainment
- Movies
- Television
- IMDb
- Metadata
---
