---
api_key_in:
- header
api_specs:
- filename: dacast-openapi.yml
  format: yaml
  label: Dacast VOD API
  slug: dacast-vod-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dacast/refs/heads/main/openapi/dacast-openapi.yml
- filename: dacast-openapi.yml
  format: yaml
  label: Dacast Live Channels API
  slug: dacast-live-channels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dacast/refs/heads/main/openapi/dacast-openapi.yml
- filename: dacast-openapi.yml
  format: yaml
  label: Dacast Playlists API
  slug: dacast-playlists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dacast/refs/heads/main/openapi/dacast-openapi.yml
- filename: dacast-openapi.yml
  format: yaml
  label: Dacast Analytics API
  slug: dacast-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dacast/refs/heads/main/openapi/dacast-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Dacast Authentication
name_suffix: Authentication
oauth_flows: []
overview: Dacast secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Dacast
provider_slug: dacast
scheme_count: 1
schemes:
- in: header
  name: ApiKeyAuth
  parameter: X-Api-Key
  sources:
  - openapi/dacast-openapi.yml
  type: apiKey
slug: dacast-authentication
source_filename: dacast-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/dacast-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-Api-Key\n  sources:\n  - openapi/dacast-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dacast/refs/heads/main/authentication/dacast-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Live Streaming
- Video
- VOD
- OTT
- Video Hosting
- Media
- Analytics
---
