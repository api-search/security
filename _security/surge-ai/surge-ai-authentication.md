---
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Surge Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Surge AI secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Surge AI
provider_slug: surge-ai
scheme_count: 1
schemes:
- description: HTTP Basic auth with the API key as username (set via SURGE_API_KEY).
  name: basicAuth
  scheme: basic
  sources:
  - openapi/surge-ai-openapi.yml
  type: http
slug: surge-ai-authentication
source_filename: surge-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/surge-ai-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic auth with the API key as username (set via SURGE_API_KEY).\n  sources:\n  - openapi/surge-ai-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/surge-ai/refs/heads/main/authentication/surge-ai-authentication.yml
summary_line: http · 1 scheme
tags:
- Human Data
- RLHF
- SFT
- Rubrics
- Verifiers
- RL Environments
- Multimodal
- Internationalization
- Labeling
---
