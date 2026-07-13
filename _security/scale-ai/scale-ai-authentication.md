---
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Scale Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Scale AI secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Scale AI
provider_slug: scale-ai
scheme_count: 1
schemes:
- description: 'HTTP Basic authentication. Use your Scale API key (live or sandbox) as

    the username and leave the password blank.'
  name: BasicAuth
  scheme: basic
  sources:
  - openapi/scale-ai-openapi.yml
  type: http
slug: scale-ai-authentication
source_filename: scale-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/scale-ai-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BasicAuth\n  type: http\n  scheme: basic\n  description: |-\n    HTTP Basic authentication. Use your Scale API key (live or sandbox) as\n    the username and leave the password blank.\n  sources:\n  - openapi/scale-ai-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/scale-ai/refs/heads/main/authentication/scale-ai-authentication.yml
summary_line: http · 1 scheme
tags:
- Data Engine
- Labeling
- RLHF
- GenAI Platform
- Donovan
- Defense AI
- LiDAR
- Sensor Fusion
- REST API
---
