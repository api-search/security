---
api_key_in:
- query
api_specs:
- filename: youtube-data-api-openapi.yml
  format: yaml
  label: Youtube Activities API
  slug: youtube-activities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/youtube/refs/heads/main/openapi/youtube-data-api-openapi.yml
- filename: youtube-data-api-openapi.yml
  format: yaml
  label: Youtube Channels API
  slug: youtube-channels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/youtube/refs/heads/main/openapi/youtube-data-api-openapi.yml
- filename: youtube-data-api-openapi.yml
  format: yaml
  label: Youtube Comments API
  slug: youtube-comments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/youtube/refs/heads/main/openapi/youtube-data-api-openapi.yml
- filename: youtube-data-api-openapi.yml
  format: yaml
  label: Youtube Comment Threads API
  slug: youtube-comment-threads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/youtube/refs/heads/main/openapi/youtube-data-api-openapi.yml
- filename: youtube-data-api-openapi.yml
  format: yaml
  label: Youtube Playlists API
  slug: youtube-playlists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/youtube/refs/heads/main/openapi/youtube-data-api-openapi.yml
- filename: youtube-data-api-openapi.yml
  format: yaml
  label: Youtube Playlist Items API
  slug: youtube-playlist-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/youtube/refs/heads/main/openapi/youtube-data-api-openapi.yml
- filename: youtube-data-api-openapi.yml
  format: yaml
  label: Youtube Search API
  slug: youtube-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/youtube/refs/heads/main/openapi/youtube-data-api-openapi.yml
- filename: youtube-data-api-openapi.yml
  format: yaml
  label: Youtube Subscriptions API
  slug: youtube-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/youtube/refs/heads/main/openapi/youtube-data-api-openapi.yml
- filename: youtube-data-api-openapi.yml
  format: yaml
  label: Youtube Videos API
  slug: youtube-videos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/youtube/refs/heads/main/openapi/youtube-data-api-openapi.yml
- filename: youtube-data-api-openapi.yml
  format: yaml
  label: Youtube Captions API
  slug: youtube-captions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/youtube/refs/heads/main/openapi/youtube-data-api-openapi.yml
- filename: youtube-data-api-openapi.yml
  format: yaml
  label: Youtube Video Categories API
  slug: youtube-video-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/youtube/refs/heads/main/openapi/youtube-data-api-openapi.yml
- filename: youtube-data-api-openapi.yml
  format: yaml
  label: Youtube I18n Languages API
  slug: youtube-i18n-languages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/youtube/refs/heads/main/openapi/youtube-data-api-openapi.yml
- filename: youtube-data-api-openapi.yml
  format: yaml
  label: Youtube I18n Regions API
  slug: youtube-i18n-regions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/youtube/refs/heads/main/openapi/youtube-data-api-openapi.yml
- filename: youtube-analytics-openapi.yml
  format: yaml
  label: YouTube Analytics API
  slug: youtube-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/youtube/refs/heads/main/openapi/youtube-analytics-openapi.yml
- filename: youtube-reporting-openapi.yml
  format: yaml
  label: YouTube Reporting API
  slug: youtube-reporting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/youtube/refs/heads/main/openapi/youtube-reporting-openapi.yml
- filename: youtube-live-streaming-openapi.yml
  format: yaml
  label: YouTube Live Streaming API
  slug: youtube-live-streaming-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/youtube/refs/heads/main/openapi/youtube-live-streaming-openapi.yml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Youtube Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Youtube secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Youtube
provider_slug: youtube
scheme_count: 2
schemes:
- description: OAuth 2.0 authentication for YouTube Analytics API
  flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/auth
    flow: authorizationCode
    scopes: 4
    tokenUrl: https://oauth2.googleapis.com/token
  name: OAuth2
  sources:
  - openapi/youtube-analytics-openapi-original.yml
  - openapi/youtube-analytics-openapi.yml
  - openapi/youtube-data-api-openapi.yml
  - openapi/youtube-data-openapi-original.yml
  - openapi/youtube-live-streaming-openapi.yml
  - openapi/youtube-reporting-openapi.yml
  type: oauth2
- in: query
  name: apiKey
  parameter: key
  sources:
  - openapi/youtube-data-api-openapi.yml
  - openapi/youtube-data-openapi-original.yml
  - openapi/youtube-live-streaming-openapi.yml
  type: apiKey
slug: youtube-authentication
source_filename: youtube-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/youtube-analytics-openapi-original.yml, openapi/youtube-analytics-openapi.yml,\n  openapi/youtube-data-api-openapi.yml, openapi/youtube-data-openapi-original.yml, openapi/youtube-live-streaming-openapi.yml,\n  openapi/youtube-reporting-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - query\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\n    scopes: 4\n  description: OAuth 2.0 authentication for YouTube Analytics API\n  sources:\n  - openapi/youtube-analytics-openapi-original.yml\n  - openapi/youtube-analytics-openapi.yml\n  - openapi/youtube-data-api-openapi.yml\n  - openapi/youtube-data-openapi-original.yml\n  - openapi/youtube-live-streaming-openapi.yml\n  - openapi/youtube-reporting-openapi.yml\n- name:\
  \ apiKey\n  type: apiKey\n  in: query\n  parameter: key\n  sources:\n  - openapi/youtube-data-api-openapi.yml\n  - openapi/youtube-data-openapi-original.yml\n  - openapi/youtube-live-streaming-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/youtube/refs/heads/main/authentication/youtube-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- Google
- Media
- Social
- Streaming
- Video
- Videos
---
