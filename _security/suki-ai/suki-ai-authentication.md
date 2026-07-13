---
api_key_in: []
api_specs:
- filename: suki-ai-openapi.yml
  format: yaml
  label: Suki Platform REST API
  slug: suki-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/suki-ai/refs/heads/main/openapi/suki-ai-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Suki Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Suki AI secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Suki AI
provider_slug: suki-ai
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: 'JWT access token issued by Suki after partner registration and login.

    Partner credentials are provisioned by Suki (no self-service signup).'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/suki-ai-openapi.yml
  type: http
slug: suki-ai-authentication
source_filename: suki-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/suki-ai-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: |-\n    JWT access token issued by Suki after partner registration and login.\n    Partner credentials are provisioned by Suki (no self-service signup).\n  sources:\n  - openapi/suki-ai-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/suki-ai/refs/heads/main/authentication/suki-ai-authentication.yml
summary_line: http · 1 scheme
tags:
- Healthcare
- Ambient AI
- Clinical Documentation
- Voice AI
- Speech Recognition
- EHR Integration
- SDK
- Dictation
---
