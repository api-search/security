---
api_key_in: []
api_specs:
- filename: rask-openapi.yml
  format: yaml
  label: Rask AI Projects & Dubbing Jobs API
  slug: projects-dubbing-jobs
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rask/refs/heads/main/openapi/rask-openapi.yml
- filename: rask-openapi.yml
  format: yaml
  label: Rask AI Translation API
  slug: translation
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rask/refs/heads/main/openapi/rask-openapi.yml
- filename: rask-openapi.yml
  format: yaml
  label: Rask AI Voices API
  slug: voices
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rask/refs/heads/main/openapi/rask-openapi.yml
- filename: rask-openapi.yml
  format: yaml
  label: Rask AI Transcription API
  slug: transcription
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rask/refs/heads/main/openapi/rask-openapi.yml
- filename: rask-openapi.yml
  format: yaml
  label: Rask AI Job Status API
  slug: job-status
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rask/refs/heads/main/openapi/rask-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Rask Authentication
name_suffix: Authentication
oauth_flows: []
overview: Rask AI secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Rask AI
provider_slug: rask
scheme_count: 1
schemes:
- description: 'OAuth2-issued Bearer token. Generate an API Client ID and API Code in the Rask app, exchange them for an OAuth2 token, and send it as `Authorization: Bearer {token}`.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/rask-openapi.yml
  type: http
slug: rask-authentication
source_filename: rask-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/rask-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'OAuth2-issued Bearer token. Generate an API Client ID and API Code in the Rask\n    app, exchange them for an OAuth2 token, and send it as `Authorization: Bearer {token}`.'\n  sources:\n  - openapi/rask-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rask/refs/heads/main/authentication/rask-authentication.yml
summary_line: http · 1 scheme
tags:
- AI
- Video Localization
- Dubbing
- Translation
- Transcription
---
