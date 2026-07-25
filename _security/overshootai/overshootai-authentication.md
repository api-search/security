---
api_key_in: []
api_specs:
- filename: overshootai-billing-api-openapi.yml
  format: yaml
  label: overshoot.ai Billing API
  slug: overshootai-billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/overshootai/refs/heads/main/openapi/overshootai-billing-api-openapi.yml
- filename: overshootai-chat-api-openapi.yml
  format: yaml
  label: overshoot.ai Chat API
  slug: overshootai-chat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/overshootai/refs/heads/main/openapi/overshootai-chat-api-openapi.yml
- filename: overshootai-healthz-api-openapi.yml
  format: yaml
  label: overshoot.ai Healthz API
  slug: overshootai-healthz-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/overshootai/refs/heads/main/openapi/overshootai-healthz-api-openapi.yml
- filename: overshootai-metrics-api-openapi.yml
  format: yaml
  label: overshoot.ai Metrics API
  slug: overshootai-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/overshootai/refs/heads/main/openapi/overshootai-metrics-api-openapi.yml
- filename: overshootai-models-api-openapi.yml
  format: yaml
  label: overshoot.ai Models API
  slug: overshootai-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/overshootai/refs/heads/main/openapi/overshootai-models-api-openapi.yml
- filename: overshootai-readyz-api-openapi.yml
  format: yaml
  label: overshoot.ai Readyz API
  slug: overshootai-readyz-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/overshootai/refs/heads/main/openapi/overshootai-readyz-api-openapi.yml
- filename: overshootai-streams-api-openapi.yml
  format: yaml
  label: overshoot.ai Streams API
  slug: overshootai-streams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/overshootai/refs/heads/main/openapi/overshootai-streams-api-openapi.yml
- filename: overshootai-v1beta-api-openapi.yml
  format: yaml
  label: overshoot.ai V1beta API
  slug: overshootai-v1beta-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/overshootai/refs/heads/main/openapi/overshootai-v1beta-api-openapi.yml
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
