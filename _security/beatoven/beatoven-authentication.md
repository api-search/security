---
api_key_in: []
api_specs:
- filename: beatoven-composition-api-openapi.yml
  format: yaml
  label: Beatoven Composition API
  slug: beatoven-composition-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beatoven/refs/heads/main/openapi/beatoven-composition-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Beatoven Authentication
name_suffix: Authentication
oauth_flows: []
overview: Beatoven.ai secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Beatoven.ai
provider_slug: beatoven
scheme_count: 1
schemes:
- description: Beatoven API token, issued by hello@beatoven.ai or from the API dashboard.
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/beatoven-composition-api-openapi.yml
  type: http
slug: beatoven-authentication
source_filename: beatoven-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/beatoven-composition-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: Beatoven API token, issued by hello@beatoven.ai or from the API dashboard.\n  sources:\n  - openapi/beatoven-composition-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/beatoven/refs/heads/main/authentication/beatoven-authentication.yml
summary_line: http · 1 scheme
tags:
- AI
- Artificial Intelligence
- Music
- Music Generation
- Generative Audio
- Text To Music
- Text To SFX
- Royalty-Free Music
- Background Music
- Video Creators
- Podcasts
- Stems
- Fairly Trained
- India
---
