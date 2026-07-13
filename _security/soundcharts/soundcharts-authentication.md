---
api_key_in:
- header
api_specs:
- filename: soundcharts-openapi.yml
  format: yaml
  label: Soundcharts Artists API
  slug: artists
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/soundcharts/refs/heads/main/openapi/soundcharts-openapi.yml
- filename: soundcharts-openapi.yml
  format: yaml
  label: Soundcharts Songs API
  slug: songs
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/soundcharts/refs/heads/main/openapi/soundcharts-openapi.yml
- filename: soundcharts-openapi.yml
  format: yaml
  label: Soundcharts Albums API
  slug: albums
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/soundcharts/refs/heads/main/openapi/soundcharts-openapi.yml
- filename: soundcharts-openapi.yml
  format: yaml
  label: Soundcharts Playlists API
  slug: playlists
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/soundcharts/refs/heads/main/openapi/soundcharts-openapi.yml
- filename: soundcharts-openapi.yml
  format: yaml
  label: Soundcharts Charts API
  slug: charts
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/soundcharts/refs/heads/main/openapi/soundcharts-openapi.yml
- filename: soundcharts-openapi.yml
  format: yaml
  label: Soundcharts Streaming and Social Metrics API
  slug: streaming-social-metrics
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/soundcharts/refs/heads/main/openapi/soundcharts-openapi.yml
- filename: soundcharts-openapi.yml
  format: yaml
  label: Soundcharts Radio API
  slug: radio
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/soundcharts/refs/heads/main/openapi/soundcharts-openapi.yml
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
