---
api_key_in:
- header
api_specs:
- filename: moondream-openapi.yml
  format: yaml
  label: Moondream Cloud API
  slug: moondream-cloud-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moondream/refs/heads/main/openapi/moondream-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: searched
name: Moondream Authentication
name_suffix: Authentication
oauth_flows: []
overview: Moondream secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Moondream
provider_slug: moondream
scheme_count: 2
schemes:
- in: header
  name: MoondreamAuth
  parameter_name: X-Moondream-Auth
  sources:
  - openapi/moondream-openapi.yml
  type: apiKey
- name: BearerAuth
  scheme: bearer
  sources:
  - openapi/moondream-openapi.yml
  type: http
  used_by:
  - /chat/completions
slug: moondream-authentication
source_filename: moondream-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: openapi/moondream-openapi.yml\ndocs: https://docs.moondream.ai/api\nsummary:\n  types: [apiKey, http]\n  api_key_in: [header]\n  http_schemes: [bearer]\n  oauth2_flows: []\nnotes: >-\n  Moondream Cloud authenticates every request with an API key issued from the\n  Moondream Cloud Console (https://moondream.ai/c/cloud/api-keys). Native Skill\n  endpoints (/query, /caption, /detect, /point, /segment) pass the key in the\n  X-Moondream-Auth header. The OpenAI-compatible /chat/completions endpoint takes\n  the same key as an HTTP bearer token (Authorization: Bearer). There is no OAuth\n  or scope surface.\nschemes:\n  - name: MoondreamAuth\n    type: apiKey\n    in: header\n    parameter_name: X-Moondream-Auth\n    sources: [openapi/moondream-openapi.yml]\n  - name: BearerAuth\n    type: http\n    scheme: bearer\n    used_by: [/chat/completions]\n    sources: [openapi/moondream-openapi.yml]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/moondream/refs/heads/main/authentication/moondream-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Company
- Artificial Intelligence
- Machine Learning
- Computer Vision
- Vision Language Model
- Object Detection
- Image Captioning
- OCR
- Developer Tools
---
