---
api_key_in:
- header
api_specs:
- filename: apple-music-openapi.yml
  format: yaml
  label: Apple Music API
  slug: catalog-library
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apple-music/refs/heads/main/openapi/apple-music-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Apple Music Authentication
name_suffix: Authentication
oauth_flows: []
overview: Apple Music secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Apple Music
provider_slug: apple-music
scheme_count: 2
schemes:
- bearerFormat: JWT
  description: 'Apple Music developer token (JWT) generated from a Music Key in the

    Apple Developer account.'
  name: DeveloperToken
  scheme: bearer
  sources:
  - openapi/apple-music-openapi.yml
  type: http
- description: 'Music User Token obtained via MusicKit on a signed-in device. Required

    for user-library endpoints.'
  in: header
  name: MusicUserToken
  parameter: Music-User-Token
  sources:
  - openapi/apple-music-openapi.yml
  type: apiKey
slug: apple-music-authentication
source_filename: apple-music-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/apple-music-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: DeveloperToken\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: |-\n    Apple Music developer token (JWT) generated from a Music Key in the\n    Apple Developer account.\n  sources:\n  - openapi/apple-music-openapi.yml\n- name: MusicUserToken\n  type: apiKey\n  in: header\n  parameter: Music-User-Token\n  description: |-\n    Music User Token obtained via MusicKit on a signed-in device. Required\n    for user-library endpoints.\n  sources:\n  - openapi/apple-music-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apple-music/refs/heads/main/authentication/apple-music-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Music
- Streaming
- Apple
- MusicKit
- Catalog
- Library
---
