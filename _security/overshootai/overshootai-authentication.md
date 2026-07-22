---
api_key_in: []
api_specs:
- filename: overshootai-openapi.yaml
  format: yaml
  label: Overshoot API
  slug: overshoot-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/overshootai/refs/heads/main/openapi/overshootai-openapi.yaml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Overshootai Authentication
name_suffix: Authentication
oauth_flows: []
overview: overshoot.ai secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: overshoot.ai
provider_slug: overshootai
scheme_count: 1
schemes:
- description: Bearer <api_key>
  name: API Key
  scheme: bearer
  sources:
  - openapi/overshootai-inference-openapi-original.json
  - openapi/overshootai-openapi.yaml
  type: http
slug: overshootai-authentication
source_filename: overshootai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: derived\nsource: openapi/overshootai-inference-openapi-original.json, openapi/overshootai-openapi.yaml\nsummary:\n  types:\n  - http\nschemes:\n- name: API Key\n  type: http\n  scheme: bearer\n  description: Bearer <api_key>\n  sources:\n  - openapi/overshootai-inference-openapi-original.json\n  - openapi/overshootai-openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/overshootai/refs/heads/main/authentication/overshootai-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Artificial Intelligence
- Computer Vision
- Video
- Real Time
- Streaming
- Machine Learning
- Vision Language Models
- Inference
- Developer Tools
---
