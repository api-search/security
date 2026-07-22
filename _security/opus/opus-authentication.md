---
api_key_in: []
api_specs:
- filename: opus-openapi-original.json
  format: json
  label: OpusClip API
  slug: opusclip-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opus/refs/heads/main/openapi/opus-openapi-original.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Opus Authentication
name_suffix: Authentication
oauth_flows: []
overview: Opus secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Opus
provider_slug: opus
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: bearer
  scheme: bearer
  sources:
  - openapi/opus-openapi-original.json
  type: http
slug: opus-authentication
source_filename: opus-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: derived\nsource: openapi/opus-openapi-original.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearer\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/opus-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/opus/refs/heads/main/authentication/opus-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Frontier Tech
- Video
- AI
- Video Editing
- Short-Form Video
- Content Creation
- Social Media
- Media
- Agents
---
