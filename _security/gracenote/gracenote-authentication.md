---
api_key_in:
- query
api_specs:
- filename: gracenote-celebrities-api-openapi.yml
  format: yaml
  label: Gracenote Celebrities API
  slug: gracenote-celebrities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gracenote/refs/heads/main/openapi/gracenote-celebrities-api-openapi.yml
- filename: gracenote-lineups-api-openapi.yml
  format: yaml
  label: Gracenote Lineups API
  slug: gracenote-lineups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gracenote/refs/heads/main/openapi/gracenote-lineups-api-openapi.yml
- filename: gracenote-movies-api-openapi.yml
  format: yaml
  label: Gracenote Movies API
  slug: gracenote-movies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gracenote/refs/heads/main/openapi/gracenote-movies-api-openapi.yml
- filename: gracenote-programs-api-openapi.yml
  format: yaml
  label: Gracenote Programs API
  slug: gracenote-programs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gracenote/refs/heads/main/openapi/gracenote-programs-api-openapi.yml
- filename: gracenote-series-api-openapi.yml
  format: yaml
  label: Gracenote Series API
  slug: gracenote-series-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gracenote/refs/heads/main/openapi/gracenote-series-api-openapi.yml
- filename: gracenote-sports-api-openapi.yml
  format: yaml
  label: Gracenote Sports API
  slug: gracenote-sports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gracenote/refs/heads/main/openapi/gracenote-sports-api-openapi.yml
- filename: gracenote-stations-api-openapi.yml
  format: yaml
  label: Gracenote Stations API
  slug: gracenote-stations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gracenote/refs/heads/main/openapi/gracenote-stations-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Gracenote Authentication
name_suffix: Authentication
oauth_flows: []
overview: Gracenote secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Gracenote
provider_slug: gracenote
scheme_count: 1
schemes:
- in: query
  name: apiKey
  parameter: api_key
  sources:
  - openapi/gracenote-openapi.yml
  type: apiKey
slug: gracenote-authentication
source_filename: gracenote-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/gracenote-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: apiKey\n  type: apiKey\n  in: query\n  parameter: api_key\n  sources:\n  - openapi/gracenote-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gracenote/refs/heads/main/authentication/gracenote-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Automotive
- Content Metadata
- Entertainment
- Music
- Nielsen
- Sports
- Streaming
- Television
- Video
---
