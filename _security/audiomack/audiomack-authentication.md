---
api_key_in: []
api_specs:
- filename: audiomack-data-api-openapi.yml
  format: yaml
  label: Audiomack Data API
  slug: audiomack-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/audiomack/refs/heads/main/openapi/audiomack-data-api-openapi.yml
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
