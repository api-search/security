---
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Autocontent Api Authentication
name_suffix: Authentication
oauth_flows: []
overview: AutoContent API secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: AutoContent API
provider_slug: autocontent-api
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: AutoContent API key as a Bearer token in the Authorization header.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/autocontent-api-openapi.yml
  type: http
slug: autocontent-api-authentication
source_filename: autocontent-api-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/autocontent-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: AutoContent API key as a Bearer token in the Authorization header.\n  sources:\n  - openapi/autocontent-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/autocontent-api/refs/heads/main/authentication/autocontent-api-authentication.yml
summary_line: http · 1 scheme
tags:
- AI
- Audio
- Content Generation
- Podcasts
- Video
- Generative AI
- Text to Speech
- Automation
---
