---
api_key_in:
- header
api_specs:
- filename: listennotes-directory-api-api-openapi.yml
  format: yaml
  label: Listen Notes Directory API API
  slug: listennotes-directory-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/listennotes/refs/heads/main/openapi/listennotes-directory-api-api-openapi.yml
- filename: listennotes-insights-api-api-openapi.yml
  format: yaml
  label: Listen Notes Insights API API
  slug: listennotes-insights-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/listennotes/refs/heads/main/openapi/listennotes-insights-api-api-openapi.yml
- filename: listennotes-playlist-api-api-openapi.yml
  format: yaml
  label: Listen Notes Playlist API API
  slug: listennotes-playlist-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/listennotes/refs/heads/main/openapi/listennotes-playlist-api-api-openapi.yml
- filename: listennotes-podcaster-api-api-openapi.yml
  format: yaml
  label: Listen Notes Podcaster API API
  slug: listennotes-podcaster-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/listennotes/refs/heads/main/openapi/listennotes-podcaster-api-api-openapi.yml
- filename: listennotes-search-api-api-openapi.yml
  format: yaml
  label: Listen Notes Search API API
  slug: listennotes-search-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/listennotes/refs/heads/main/openapi/listennotes-search-api-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Listennotes Authentication
name_suffix: Authentication
oauth_flows: []
overview: Listen Notes secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Listen Notes
provider_slug: listennotes
scheme_count: 1
schemes:
- description: Your Listen API key, sent in the X-ListenAPI-Key request header.
  in: header
  name: apiKeyHeader
  parameter: X-ListenAPI-Key
  sources:
  - openapi/listennotes-openapi.yml
  type: apiKey
slug: listennotes-authentication
source_filename: listennotes-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/listennotes-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKeyHeader\n  type: apiKey\n  in: header\n  parameter: X-ListenAPI-Key\n  description: Your Listen API key, sent in the X-ListenAPI-Key request header.\n  sources:\n  - openapi/listennotes-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/listennotes/refs/heads/main/authentication/listennotes-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Podcasts
- Podcast Search
- Podcast Directory
- Search
- Audio
- Media
- Podcast Insights
---
