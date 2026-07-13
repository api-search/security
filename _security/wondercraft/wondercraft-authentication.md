---
api_key_in:
- header
api_specs:
- filename: wondercraft-openapi.yml
  format: yaml
  label: Wondercraft Audio Generation API
  slug: audio-generation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wondercraft/refs/heads/main/openapi/wondercraft-openapi.yml
- filename: wondercraft-openapi.yml
  format: yaml
  label: Wondercraft Scripted Audio API
  slug: scripted-audio-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wondercraft/refs/heads/main/openapi/wondercraft-openapi.yml
- filename: wondercraft-openapi.yml
  format: yaml
  label: Wondercraft Convo Mode API
  slug: convo-mode-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wondercraft/refs/heads/main/openapi/wondercraft-openapi.yml
- filename: wondercraft-openapi.yml
  format: yaml
  label: Wondercraft Job Status API
  slug: job-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wondercraft/refs/heads/main/openapi/wondercraft-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Wondercraft Authentication
name_suffix: Authentication
oauth_flows: []
overview: Wondercraft secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Wondercraft
provider_slug: wondercraft
scheme_count: 1
schemes:
- in: header
  name: APIKeyHeader
  parameter: X-API-KEY
  sources:
  - openapi/wondercraft-openapi.yml
  type: apiKey
slug: wondercraft-authentication
source_filename: wondercraft-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/wondercraft-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: APIKeyHeader\n  type: apiKey\n  in: header\n  parameter: X-API-KEY\n  sources:\n  - openapi/wondercraft-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wondercraft/refs/heads/main/authentication/wondercraft-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- AI
- Audio
- Podcast
- Text to Speech
- Generative Audio
---
