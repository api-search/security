---
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Inworld Authentication
name_suffix: Authentication
oauth_flows: []
overview: Inworld AI secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Inworld AI
provider_slug: inworld
scheme_count: 1
schemes:
- description: 'Authentication uses HTTP Basic with the API key as the username

    (password empty), encoded as: `Authorization: Basic base64(apiKey:)`.

    Get an API key at https://platform.inworld.ai.'
  name: basicAuth
  scheme: basic
  sources:
  - openapi/inworld-openapi.yml
  type: http
slug: inworld-authentication
source_filename: inworld-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/inworld-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: |-\n    Authentication uses HTTP Basic with the API key as the username\n    (password empty), encoded as: `Authorization: Basic base64(apiKey:)`.\n    Get an API key at https://platform.inworld.ai.\n  sources:\n  - openapi/inworld-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/inworld/refs/heads/main/authentication/inworld-authentication.yml
summary_line: http · 1 scheme
tags:
- AI
- Voice
- Characters
- Games
- Conversational
---
