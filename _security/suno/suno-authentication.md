---
api_key_in: []
api_specs:
- filename: suno-lyrics-api-openapi.yml
  format: yaml
  label: Suno Lyrics API
  slug: suno-lyrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/suno/refs/heads/main/openapi/suno-lyrics-api-openapi.yml
- filename: suno-music-api-openapi.yml
  format: yaml
  label: Suno Music API
  slug: suno-music-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/suno/refs/heads/main/openapi/suno-music-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Suno Authentication
name_suffix: Authentication
oauth_flows: []
overview: Suno secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Suno
provider_slug: suno
scheme_count: 1
schemes:
- bearerFormat: API Key
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/suno-openapi.yml
  type: http
slug: suno-authentication
source_filename: suno-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/suno-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: API Key\n  sources:\n  - openapi/suno-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/suno/refs/heads/main/authentication/suno-authentication.yml
summary_line: http · 1 scheme
tags:
- Artificial Intelligence
- Music Generation
- Audio
- Generative
- TTS
---
