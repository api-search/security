---
api_key_in:
- header
api_specs:
- filename: soundcharts-album-api-openapi.yml
  format: yaml
  label: Soundcharts Album API
  slug: soundcharts-album-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/soundcharts/refs/heads/main/openapi/soundcharts-album-api-openapi.yml
- filename: soundcharts-artist-api-openapi.yml
  format: yaml
  label: Soundcharts Artist API
  slug: soundcharts-artist-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/soundcharts/refs/heads/main/openapi/soundcharts-artist-api-openapi.yml
- filename: soundcharts-chart-api-openapi.yml
  format: yaml
  label: Soundcharts Chart API
  slug: soundcharts-chart-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/soundcharts/refs/heads/main/openapi/soundcharts-chart-api-openapi.yml
- filename: soundcharts-metrics-api-openapi.yml
  format: yaml
  label: Soundcharts Metrics API
  slug: soundcharts-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/soundcharts/refs/heads/main/openapi/soundcharts-metrics-api-openapi.yml
- filename: soundcharts-playlist-api-openapi.yml
  format: yaml
  label: Soundcharts Playlist API
  slug: soundcharts-playlist-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/soundcharts/refs/heads/main/openapi/soundcharts-playlist-api-openapi.yml
- filename: soundcharts-radio-api-openapi.yml
  format: yaml
  label: Soundcharts Radio API
  slug: soundcharts-radio-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/soundcharts/refs/heads/main/openapi/soundcharts-radio-api-openapi.yml
- filename: soundcharts-referential-api-openapi.yml
  format: yaml
  label: Soundcharts Referential API
  slug: soundcharts-referential-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/soundcharts/refs/heads/main/openapi/soundcharts-referential-api-openapi.yml
- filename: soundcharts-search-api-openapi.yml
  format: yaml
  label: Soundcharts Search API
  slug: soundcharts-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/soundcharts/refs/heads/main/openapi/soundcharts-search-api-openapi.yml
- filename: soundcharts-song-api-openapi.yml
  format: yaml
  label: Soundcharts Song API
  slug: soundcharts-song-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/soundcharts/refs/heads/main/openapi/soundcharts-song-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Soundcharts Authentication
name_suffix: Authentication
oauth_flows: []
overview: Soundcharts secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Soundcharts
provider_slug: soundcharts
scheme_count: 2
schemes:
- description: Soundcharts application identifier.
  in: header
  name: AppId
  parameter: x-app-id
  sources:
  - openapi/soundcharts-openapi.yml
  type: apiKey
- description: Soundcharts API key.
  in: header
  name: ApiKey
  parameter: x-api-key
  sources:
  - openapi/soundcharts-openapi.yml
  type: apiKey
slug: soundcharts-authentication
source_filename: soundcharts-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/soundcharts-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: AppId\n  type: apiKey\n  in: header\n  parameter: x-app-id\n  description: Soundcharts application identifier.\n  sources:\n  - openapi/soundcharts-openapi.yml\n- name: ApiKey\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: Soundcharts API key.\n  sources:\n  - openapi/soundcharts-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/soundcharts/refs/heads/main/authentication/soundcharts-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Music
- Analytics
- Market Intelligence
- Metadata
- Streaming
- Charts
---
