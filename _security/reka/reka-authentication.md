---
api_key_in: []
api_specs:
- filename: openapi.json
  format: json
  label: Reka API
  slug: reka-api
  spec_type: OpenAPI
  url: https://api.reka.ai/openapi.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Reka Authentication
name_suffix: Authentication
oauth_flows: []
overview: Reka secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Reka
provider_slug: reka
scheme_count: 1
schemes:
- bearerFormat: REKA_API_KEY
  description: 'Bearer token issued from the Reka Platform dashboard. Pass as

    `Authorization: Bearer [example key]`.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/reka-openapi.yml
  type: http
slug: reka-authentication
source_filename: reka-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/reka-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: REKA_API_KEY\n  description: |-\n    Bearer token issued from the Reka Platform dashboard. Pass as\n    `Authorization: Bearer [example key]`.\n  sources:\n  - openapi/reka-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/reka/refs/heads/main/authentication/reka-authentication.yml
summary_line: http · 1 scheme
tags:
- AI
- Multimodal
- Large Language Models
- Vision
- Speech
- Foundation Models
- OpenAI Compatible
- SDK
- Enterprise
- On-Premises
---
