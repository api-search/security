---
api_key_in: []
api_specs:
- filename: spotify-openapi-original.yml
  format: yaml
  label: Spotify Web API
  slug: spotify-web-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spotify/refs/heads/main/openapi/spotify-openapi-original.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Spotify Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Spotify secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Spotify
provider_slug: spotify
scheme_count: 1
schemes:
- description: Spotify supports OAuth 2.0 for authenticating all API requests.
  flows:
  - authorizationUrl: https://accounts.spotify.com/authorize
    flow: authorizationCode
    scopes: 19
    tokenUrl: https://accounts.spotify.com/api/token
  name: oauth_2_0
  sources:
  - openapi/spotify-openapi-original.yml
  type: oauth2
slug: spotify-authentication
source_filename: spotify-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/spotify-openapi-original.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: oauth_2_0\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.spotify.com/authorize\n    tokenUrl: https://accounts.spotify.com/api/token\n    scopes: 19\n  description: Spotify supports OAuth 2.0 for authenticating all API requests.\n  sources:\n  - openapi/spotify-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/spotify/refs/heads/main/authentication/spotify-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Music
- Audio
- Streaming
- Podcasts
- Playlists
---
