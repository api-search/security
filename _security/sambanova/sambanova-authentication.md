---
api_key_in: []
api_specs:
- filename: sambanova-openapi.yml
  format: yaml
  label: SambaCloud API
  slug: sambacloud-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sambanova/refs/heads/main/openapi/sambanova-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Sambanova Authentication
name_suffix: Authentication
oauth_flows: []
overview: SambaNova secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: SambaNova
provider_slug: sambanova
scheme_count: 1
schemes:
- description: 'SambaCloud API key issued from the /apis dashboard on

    cloud.sambanova.ai, sent as `Authorization: Bearer <key>`.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/sambanova-openapi.yml
  type: http
slug: sambanova-authentication
source_filename: sambanova-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/sambanova-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: |-\n    SambaCloud API key issued from the /apis dashboard on\n    cloud.sambanova.ai, sent as `Authorization: Bearer <key>`.\n  sources:\n  - openapi/sambanova-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sambanova/refs/heads/main/authentication/sambanova-authentication.yml
summary_line: http · 1 scheme
tags:
- AI Inference
- Large Language Models
- Dataflow
- Hardware
- Cloud
- OpenAI Compatible
- Sovereign AI
- SDK
- Accelerator
- Open Source
---
