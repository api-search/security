---
api_key_in:
- query
api_specs:
- filename: tribune-media-celebrities-api-openapi.yml
  format: yaml
  label: Tribune Media Celebrities API
  slug: tribune-media-celebrities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tribune-media/refs/heads/main/openapi/tribune-media-celebrities-api-openapi.yml
- filename: tribune-media-lineups-api-openapi.yml
  format: yaml
  label: Tribune Media Lineups API
  slug: tribune-media-lineups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tribune-media/refs/heads/main/openapi/tribune-media-lineups-api-openapi.yml
- filename: tribune-media-movies-api-openapi.yml
  format: yaml
  label: Tribune Media Movies API
  slug: tribune-media-movies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tribune-media/refs/heads/main/openapi/tribune-media-movies-api-openapi.yml
- filename: tribune-media-online-video-api-openapi.yml
  format: yaml
  label: Tribune Media Online Video API
  slug: tribune-media-online-video-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tribune-media/refs/heads/main/openapi/tribune-media-online-video-api-openapi.yml
- filename: tribune-media-programs-api-openapi.yml
  format: yaml
  label: Tribune Media Programs API
  slug: tribune-media-programs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tribune-media/refs/heads/main/openapi/tribune-media-programs-api-openapi.yml
- filename: tribune-media-series-api-openapi.yml
  format: yaml
  label: Tribune Media Series API
  slug: tribune-media-series-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tribune-media/refs/heads/main/openapi/tribune-media-series-api-openapi.yml
- filename: tribune-media-social-api-openapi.yml
  format: yaml
  label: Tribune Media Social API
  slug: tribune-media-social-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tribune-media/refs/heads/main/openapi/tribune-media-social-api-openapi.yml
- filename: tribune-media-sports-api-openapi.yml
  format: yaml
  label: Tribune Media Sports API
  slug: tribune-media-sports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tribune-media/refs/heads/main/openapi/tribune-media-sports-api-openapi.yml
- filename: tribune-media-stations-api-openapi.yml
  format: yaml
  label: Tribune Media Stations API
  slug: tribune-media-stations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tribune-media/refs/heads/main/openapi/tribune-media-stations-api-openapi.yml
- filename: tribune-media-theatres-api-openapi.yml
  format: yaml
  label: Tribune Media Theatres API
  slug: tribune-media-theatres-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tribune-media/refs/heads/main/openapi/tribune-media-theatres-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Tribune Media Authentication
name_suffix: Authentication
oauth_flows: []
overview: Tribune Media secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Tribune Media
provider_slug: tribune-media
scheme_count: 1
schemes:
- in: query
  name: apiKey
  parameter: api_key
  sources:
  - openapi/tms-onconnect-openapi.yml
  type: apiKey
slug: tribune-media-authentication
source_filename: tribune-media-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/tms-onconnect-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: apiKey\n  type: apiKey\n  in: query\n  parameter: api_key\n  sources:\n  - openapi/tms-onconnect-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tribune-media/refs/heads/main/authentication/tribune-media-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Media
- Entertainment
- Broadcasting
- Television
- Movies
- Sports
- Celebrity
- Fortune 1000
---
