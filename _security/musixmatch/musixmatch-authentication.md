---
api_key_in:
- query
api_specs:
- filename: musixmatch-album-api-openapi.yml
  format: yaml
  label: Musixmatch Album API
  slug: musixmatch-album-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/musixmatch/refs/heads/main/openapi/musixmatch-album-api-openapi.yml
- filename: musixmatch-artist-api-openapi.yml
  format: yaml
  label: Musixmatch Artist API
  slug: musixmatch-artist-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/musixmatch/refs/heads/main/openapi/musixmatch-artist-api-openapi.yml
- filename: musixmatch-lyrics-api-openapi.yml
  format: yaml
  label: Musixmatch Lyrics API
  slug: musixmatch-lyrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/musixmatch/refs/heads/main/openapi/musixmatch-lyrics-api-openapi.yml
- filename: musixmatch-snippets-api-openapi.yml
  format: yaml
  label: Musixmatch Snippets API
  slug: musixmatch-snippets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/musixmatch/refs/heads/main/openapi/musixmatch-snippets-api-openapi.yml
- filename: musixmatch-subtitle-api-openapi.yml
  format: yaml
  label: Musixmatch Subtitle API
  slug: musixmatch-subtitle-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/musixmatch/refs/heads/main/openapi/musixmatch-subtitle-api-openapi.yml
- filename: musixmatch-track-api-openapi.yml
  format: yaml
  label: Musixmatch Track API
  slug: musixmatch-track-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/musixmatch/refs/heads/main/openapi/musixmatch-track-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Musixmatch Authentication
name_suffix: Authentication
oauth_flows: []
overview: Musixmatch secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Musixmatch
provider_slug: musixmatch
scheme_count: 1
schemes:
- in: query
  name: key
  parameter: apikey
  sources:
  - openapi/musixmatch-openapi-original.yml
  type: apiKey
slug: musixmatch-authentication
source_filename: musixmatch-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/musixmatch-openapi-original.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: key\n  type: apiKey\n  in: query\n  parameter: apikey\n  sources:\n  - openapi/musixmatch-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/musixmatch/refs/heads/main/authentication/musixmatch-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Lyrics
- Music
- Translations
---
