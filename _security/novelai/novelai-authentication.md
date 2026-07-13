---
api_key_in: []
api_specs:
- filename: novelai-openapi.yml
  format: yaml
  label: NovelAI API
  slug: novelai
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/novelai/refs/heads/main/openapi/novelai-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Novelai Authentication
name_suffix: Authentication
oauth_flows: []
overview: NovelAI secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: NovelAI
provider_slug: novelai
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: bearer
  scheme: bearer
  sources:
  - openapi/novelai-openapi.yml
  type: http
slug: novelai-authentication
source_filename: novelai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/novelai-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearer\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/novelai-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/novelai/refs/heads/main/authentication/novelai-authentication.yml
summary_line: http · 1 scheme
tags:
- AI
- Image Generation
- LLM
- Storytelling
---
