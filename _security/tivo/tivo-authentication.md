---
api_key_in: []
api_specs:
- filename: tivo-video-metadata-openapi.yml
  format: yaml
  label: TiVo Video Metadata API
  slug: tivo-video-metadata
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tivo/refs/heads/main/openapi/tivo-video-metadata-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Tivo Authentication
name_suffix: Authentication
oauth_flows: []
overview: Tivo secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Tivo
provider_slug: tivo
scheme_count: 1
schemes:
- description: TiVo API authentication token
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/tivo-video-metadata-openapi.yml
  type: http
slug: tivo-authentication
source_filename: tivo-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/tivo-video-metadata-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: TiVo API authentication token\n  sources:\n  - openapi/tivo-video-metadata-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tivo/refs/heads/main/authentication/tivo-authentication.yml
summary_line: http · 1 scheme
tags:
- Entertainment
- Metadata
- Television
- Movies
- Music
- Streaming
---
