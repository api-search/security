---
api_key_in: []
api_specs:
- filename: spotify-albums-api-openapi.yml
  format: yaml
  label: Spotify Albums API
  slug: spotify-albums-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spotify/refs/heads/main/openapi/spotify-albums-api-openapi.yml
- filename: spotify-artists-api-openapi.yml
  format: yaml
  label: Spotify Artists API
  slug: spotify-artists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spotify/refs/heads/main/openapi/spotify-artists-api-openapi.yml
- filename: spotify-audiobooks-api-openapi.yml
  format: yaml
  label: Spotify Audiobooks API
  slug: spotify-audiobooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spotify/refs/heads/main/openapi/spotify-audiobooks-api-openapi.yml
- filename: spotify-categories-api-openapi.yml
  format: yaml
  label: Spotify Categories API
  slug: spotify-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spotify/refs/heads/main/openapi/spotify-categories-api-openapi.yml
- filename: spotify-chapters-api-openapi.yml
  format: yaml
  label: Spotify Chapters API
  slug: spotify-chapters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spotify/refs/heads/main/openapi/spotify-chapters-api-openapi.yml
- filename: spotify-episodes-api-openapi.yml
  format: yaml
  label: Spotify Episodes API
  slug: spotify-episodes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spotify/refs/heads/main/openapi/spotify-episodes-api-openapi.yml
- filename: spotify-genres-api-openapi.yml
  format: yaml
  label: Spotify Genres API
  slug: spotify-genres-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spotify/refs/heads/main/openapi/spotify-genres-api-openapi.yml
- filename: spotify-library-api-openapi.yml
  format: yaml
  label: Spotify Library API
  slug: spotify-library-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spotify/refs/heads/main/openapi/spotify-library-api-openapi.yml
- filename: spotify-markets-api-openapi.yml
  format: yaml
  label: Spotify Markets API
  slug: spotify-markets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spotify/refs/heads/main/openapi/spotify-markets-api-openapi.yml
- filename: spotify-player-api-openapi.yml
  format: yaml
  label: Spotify Player API
  slug: spotify-player-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spotify/refs/heads/main/openapi/spotify-player-api-openapi.yml
- filename: spotify-playlists-api-openapi.yml
  format: yaml
  label: Spotify Playlists API
  slug: spotify-playlists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spotify/refs/heads/main/openapi/spotify-playlists-api-openapi.yml
- filename: spotify-search-api-openapi.yml
  format: yaml
  label: Spotify Search API
  slug: spotify-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spotify/refs/heads/main/openapi/spotify-search-api-openapi.yml
- filename: spotify-shows-api-openapi.yml
  format: yaml
  label: Spotify Shows API
  slug: spotify-shows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spotify/refs/heads/main/openapi/spotify-shows-api-openapi.yml
- filename: spotify-tracks-api-openapi.yml
  format: yaml
  label: Spotify Tracks API
  slug: spotify-tracks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spotify/refs/heads/main/openapi/spotify-tracks-api-openapi.yml
- filename: spotify-users-api-openapi.yml
  format: yaml
  label: Spotify Users API
  slug: spotify-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spotify/refs/heads/main/openapi/spotify-users-api-openapi.yml
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
