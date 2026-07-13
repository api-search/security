---
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Livepeer Authentication
name_suffix: Authentication
oauth_flows: []
overview: Livepeer secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Livepeer
provider_slug: livepeer
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: apiKey
  scheme: bearer
  sources:
  - openapi/livepeer-openapi.yml
  type: http
slug: livepeer-authentication
source_filename: livepeer-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/livepeer-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: apiKey\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/livepeer-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/livepeer/refs/heads/main/authentication/livepeer-authentication.yml
summary_line: http · 1 scheme
tags:
- Video
- Streaming
- Transcoding
- Decentralized
- Web3
- Live Video
- AI Video
---
