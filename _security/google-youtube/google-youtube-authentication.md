---
api_key_in:
- query
api_specs:
- filename: google-youtube-activities-api-openapi.yml
  format: yaml
  label: YouTube Data Activities API
  slug: google-youtube-activities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-youtube/refs/heads/main/openapi/google-youtube-activities-api-openapi.yml
- filename: google-youtube-channels-api-openapi.yml
  format: yaml
  label: YouTube Data Channels API
  slug: google-youtube-channels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-youtube/refs/heads/main/openapi/google-youtube-channels-api-openapi.yml
- filename: google-youtube-commentthreads-api-openapi.yml
  format: yaml
  label: YouTube Data CommentThreads API
  slug: google-youtube-commentthreads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-youtube/refs/heads/main/openapi/google-youtube-commentthreads-api-openapi.yml
- filename: google-youtube-playlistitems-api-openapi.yml
  format: yaml
  label: YouTube Data PlaylistItems API
  slug: google-youtube-playlistitems-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-youtube/refs/heads/main/openapi/google-youtube-playlistitems-api-openapi.yml
- filename: google-youtube-playlists-api-openapi.yml
  format: yaml
  label: YouTube Data Playlists API
  slug: google-youtube-playlists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-youtube/refs/heads/main/openapi/google-youtube-playlists-api-openapi.yml
- filename: google-youtube-search-api-openapi.yml
  format: yaml
  label: YouTube Data Search API
  slug: google-youtube-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-youtube/refs/heads/main/openapi/google-youtube-search-api-openapi.yml
- filename: google-youtube-subscriptions-api-openapi.yml
  format: yaml
  label: YouTube Data Subscriptions API
  slug: google-youtube-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-youtube/refs/heads/main/openapi/google-youtube-subscriptions-api-openapi.yml
- filename: google-youtube-videos-api-openapi.yml
  format: yaml
  label: YouTube Data Videos API
  slug: google-youtube-videos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-youtube/refs/heads/main/openapi/google-youtube-videos-api-openapi.yml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Google Youtube Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: YouTube Data secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: YouTube Data
provider_slug: google-youtube
scheme_count: 2
schemes:
- flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/auth
    flow: authorizationCode
    scopes: 3
    tokenUrl: https://oauth2.googleapis.com/token
  name: oauth2
  sources:
  - openapi/youtube.yml
  type: oauth2
- in: query
  name: apiKey
  parameter: key
  sources:
  - openapi/youtube.yml
  type: apiKey
slug: google-youtube-authentication
source_filename: google-youtube-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/youtube.yml\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - query\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\n    scopes: 3\n  sources:\n  - openapi/youtube.yml\n- name: apiKey\n  type: apiKey\n  in: query\n  parameter: key\n  sources:\n  - openapi/youtube.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google-youtube/refs/heads/main/authentication/google-youtube-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- Channels
- Google
- Media
- Playlists
- Search
- Streaming
- Video
- YouTube
---
