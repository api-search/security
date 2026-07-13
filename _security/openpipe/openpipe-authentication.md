---
api_key_in: []
api_specs:
- filename: openpipe-openapi.json
  format: json
  label: OpenPipe Platform API
  slug: platform
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openpipe/refs/heads/main/openapi/openpipe-openapi.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Openpipe Authentication
name_suffix: Authentication
oauth_flows: []
overview: OpenPipe secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: OpenPipe
provider_slug: openpipe
scheme_count: 1
schemes:
- name: Authorization
  scheme: bearer
  sources:
  - openapi/openpipe-openapi.json
  type: http
slug: openpipe-authentication
source_filename: openpipe-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/openpipe-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: Authorization\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/openpipe-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/openpipe/refs/heads/main/authentication/openpipe-authentication.yml
summary_line: http · 1 scheme
tags:
- AI
- LLM
- Fine-Tuning
- Distillation
- Inference
- OpenAI Compatible
- Anthropic Compatible
- Caching
---
