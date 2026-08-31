---
api_key_in:
- header
api_specs:
- filename: wondercraft-account-api-openapi.yml
  format: yaml
  label: Wondercraft Account API
  slug: wondercraft-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wondercraft/refs/heads/main/openapi/wondercraft-account-api-openapi.yml
- filename: wondercraft-audio-generation-api-openapi.yml
  format: yaml
  label: Wondercraft Audio Generation API
  slug: wondercraft-audio-generation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wondercraft/refs/heads/main/openapi/wondercraft-audio-generation-api-openapi.yml
- filename: wondercraft-convo-mode-api-openapi.yml
  format: yaml
  label: Wondercraft Convo Mode API
  slug: wondercraft-convo-mode-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wondercraft/refs/heads/main/openapi/wondercraft-convo-mode-api-openapi.yml
- filename: wondercraft-jobs-api-openapi.yml
  format: yaml
  label: Wondercraft Jobs API
  slug: wondercraft-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wondercraft/refs/heads/main/openapi/wondercraft-jobs-api-openapi.yml
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
- Artificial Intelligence
- Audio
- Podcast
- Text to Speech
- Generative Audio
---
