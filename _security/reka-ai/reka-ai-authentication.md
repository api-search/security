---
api_key_in: []
api_specs:
- filename: reka-ai-openapi.yml
  format: yaml
  label: Reka AI Platform API
  slug: platform
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reka-ai/refs/heads/main/openapi/reka-ai-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Reka Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Reka AI secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Reka AI
provider_slug: reka-ai
scheme_count: 1
schemes:
- bearerFormat: REKA_API_KEY
  description: Bearer API key issued from the Reka Platform dashboard.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/reka-ai-openapi.yml
  type: http
slug: reka-ai-authentication
source_filename: reka-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/reka-ai-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: REKA_API_KEY\n  description: Bearer API key issued from the Reka Platform dashboard.\n  sources:\n  - openapi/reka-ai-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/reka-ai/refs/heads/main/authentication/reka-ai-authentication.yml
summary_line: http · 1 scheme
tags:
- AI
- LLM
- Inference
- Multimodal
- Foundation Models
- Vision
---
