---
api_key_in: []
api_specs:
- filename: resemble-ai-openapi.yml
  format: yaml
  label: Resemble AI Platform API
  slug: platform
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/resemble-ai/refs/heads/main/openapi/resemble-ai-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Resemble Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Resemble AI secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Resemble AI
provider_slug: resemble-ai
scheme_count: 1
schemes:
- description: API token from https://app.resemble.ai/account/api
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/resemble-ai-openapi.yml
  type: http
slug: resemble-ai-authentication
source_filename: resemble-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/resemble-ai-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: API token from https://app.resemble.ai/account/api\n  sources:\n  - openapi/resemble-ai-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/resemble-ai/refs/heads/main/authentication/resemble-ai-authentication.yml
summary_line: http · 1 scheme
tags:
- AI
- Voice
- TTS
- Voice Cloning
- Voice Conversion
- Audio
- Detection
---
