---
api_key_in: []
api_specs:
- filename: audiomack-artist-api-openapi.yml
  format: yaml
  label: Audiomack Artist API
  slug: audiomack-artist-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/audiomack/refs/heads/main/openapi/audiomack-artist-api-openapi.yml
- filename: audiomack-chart-api-openapi.yml
  format: yaml
  label: Audiomack Chart API
  slug: audiomack-chart-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/audiomack/refs/heads/main/openapi/audiomack-chart-api-openapi.yml
- filename: audiomack-music-api-openapi.yml
  format: yaml
  label: Audiomack Music API
  slug: audiomack-music-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/audiomack/refs/heads/main/openapi/audiomack-music-api-openapi.yml
- filename: audiomack-oauth-api-openapi.yml
  format: yaml
  label: Audiomack OAuth API
  slug: audiomack-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/audiomack/refs/heads/main/openapi/audiomack-oauth-api-openapi.yml
- filename: audiomack-playlist-api-openapi.yml
  format: yaml
  label: Audiomack Playlist API
  slug: audiomack-playlist-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/audiomack/refs/heads/main/openapi/audiomack-playlist-api-openapi.yml
- filename: audiomack-search-api-openapi.yml
  format: yaml
  label: Audiomack Search API
  slug: audiomack-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/audiomack/refs/heads/main/openapi/audiomack-search-api-openapi.yml
- filename: audiomack-stats-api-openapi.yml
  format: yaml
  label: Audiomack Stats API
  slug: audiomack-stats-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/audiomack/refs/heads/main/openapi/audiomack-stats-api-openapi.yml
- filename: audiomack-user-api-openapi.yml
  format: yaml
  label: Audiomack User API
  slug: audiomack-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/audiomack/refs/heads/main/openapi/audiomack-user-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Audiomack Authentication
name_suffix: Authentication
oauth_flows: []
overview: Audiomack secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Audiomack
provider_slug: audiomack
scheme_count: 1
schemes:
- description: OAuth 1.0a signed request. Obtain a request token via `POST /v1/request_token`, redirect the user to `https://audiomack.com/oauth/authenticate?oauth_token=...`, then exchange for an access token via `POST /v1/access_token`. Access tokens are valid for one year.
  name: oauth1
  scheme: OAuth
  sources:
  - openapi/audiomack-data-api-openapi.yml
  type: http
slug: audiomack-authentication
source_filename: audiomack-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/audiomack-data-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: oauth1\n  type: http\n  scheme: OAuth\n  description: OAuth 1.0a signed request. Obtain a request token via `POST /v1/request_token`,\n    redirect the user to `https://audiomack.com/oauth/authenticate?oauth_token=...`, then exchange\n    for an access token via `POST /v1/access_token`. Access tokens are valid for one year.\n  sources:\n  - openapi/audiomack-data-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/audiomack/refs/heads/main/authentication/audiomack-authentication.yml
summary_line: http · 1 scheme
tags:
- Music
- Music Streaming
- Audio
- Podcasts
- Hip-Hop
- Rap
- Afrobeats
- Reggae
- Dancehall
- R&B
- Electronic
- Charts
- Playlists
- Discovery
- Creator Economy
- Independent Artists
---
