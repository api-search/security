---
api_key_in: []
api_specs:
- filename: descript-openapi.yml
  format: yaml
  label: Descript Platform API
  slug: descript-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/descript/refs/heads/main/openapi/descript-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Descript Authentication
name_suffix: Authentication
oauth_flows: []
overview: Descript secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Descript
provider_slug: descript
scheme_count: 1
schemes:
- description: Personal API token created in Descript Settings → API Tokens. See the Authentication section for details.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/descript-openapi.yml
  type: http
slug: descript-authentication
source_filename: descript-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/descript-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Personal API token created in Descript Settings → API Tokens. See the Authentication\n    section for details.\n  sources:\n  - openapi/descript-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/descript/refs/heads/main/authentication/descript-authentication.yml
summary_line: http · 1 scheme
tags:
- AI
- Audio Editing
- Captions
- Media
- Podcasting
- Transcription
- Video Editing
---
