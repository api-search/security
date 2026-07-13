---
api_key_in: []
api_specs:
- filename: sonix-openapi.yml
  format: yaml
  label: Sonix Media & Transcription API
  slug: sonix-media-transcription-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sonix/refs/heads/main/openapi/sonix-openapi.yml
- filename: sonix-openapi.yml
  format: yaml
  label: Sonix Transcripts API
  slug: sonix-transcripts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sonix/refs/heads/main/openapi/sonix-openapi.yml
- filename: sonix-openapi.yml
  format: yaml
  label: Sonix Translations API
  slug: sonix-translations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sonix/refs/heads/main/openapi/sonix-openapi.yml
- filename: sonix-openapi.yml
  format: yaml
  label: Sonix Exports & Subtitles API
  slug: sonix-exports-subtitles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sonix/refs/heads/main/openapi/sonix-openapi.yml
- filename: sonix-openapi.yml
  format: yaml
  label: Sonix AI Analysis API
  slug: sonix-ai-analysis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sonix/refs/heads/main/openapi/sonix-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Sonix Authentication
name_suffix: Authentication
oauth_flows: []
overview: Sonix secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Sonix
provider_slug: sonix
scheme_count: 1
schemes:
- description: 'Sonix API key passed as `Authorization: Bearer <API Key>`. Subscribers retrieve their key at https://my.sonix.ai/api; trial accounts request one from Sonix support. The current API version is v1 at https://api.sonix.ai/v1.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/sonix-openapi.yml
  - https://sonix.ai/docs/api
  type: http
slug: sonix-authentication
source_filename: sonix-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/sonix-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: >-\n    Sonix API key passed as `Authorization: Bearer <API Key>`. Subscribers\n    retrieve their key at https://my.sonix.ai/api; trial accounts request one\n    from Sonix support. The current API version is v1 at https://api.sonix.ai/v1.\n  sources:\n  - openapi/sonix-openapi.yml\n  - https://sonix.ai/docs/api\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sonix/refs/heads/main/authentication/sonix-authentication.yml
summary_line: http · 1 scheme
tags:
- Audio Transcription
- Transcription
- Speech-to-Text
- Subtitles
- Captions
- Translation
- AI
- Media
---
