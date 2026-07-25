---
api_key_in: []
api_specs:
- filename: overshoot-billing-api-openapi.yml
  format: yaml
  label: Overshoot Billing API
  slug: overshoot-billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/overshoot/refs/heads/main/openapi/overshoot-billing-api-openapi.yml
- filename: overshoot-chat-api-openapi.yml
  format: yaml
  label: Overshoot Chat API
  slug: overshoot-chat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/overshoot/refs/heads/main/openapi/overshoot-chat-api-openapi.yml
- filename: overshoot-healthz-api-openapi.yml
  format: yaml
  label: Overshoot Healthz API
  slug: overshoot-healthz-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/overshoot/refs/heads/main/openapi/overshoot-healthz-api-openapi.yml
- filename: overshoot-metrics-api-openapi.yml
  format: yaml
  label: Overshoot Metrics API
  slug: overshoot-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/overshoot/refs/heads/main/openapi/overshoot-metrics-api-openapi.yml
- filename: overshoot-models-api-openapi.yml
  format: yaml
  label: Overshoot Models API
  slug: overshoot-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/overshoot/refs/heads/main/openapi/overshoot-models-api-openapi.yml
- filename: overshoot-readyz-api-openapi.yml
  format: yaml
  label: Overshoot Readyz API
  slug: overshoot-readyz-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/overshoot/refs/heads/main/openapi/overshoot-readyz-api-openapi.yml
- filename: overshoot-streams-api-openapi.yml
  format: yaml
  label: Overshoot Streams API
  slug: overshoot-streams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/overshoot/refs/heads/main/openapi/overshoot-streams-api-openapi.yml
- filename: overshoot-v1beta-api-openapi.yml
  format: yaml
  label: Overshoot V1beta API
  slug: overshoot-v1beta-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/overshoot/refs/heads/main/openapi/overshoot-v1beta-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Overshoot Authentication
name_suffix: Authentication
oauth_flows: []
overview: Overshoot secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Overshoot
provider_slug: overshoot
scheme_count: 1
schemes:
- bearer_format: API key (e.g. ovs_...)
  description: Every public HTTP request requires an Authorization Bearer header carrying an Overshoot API key (prefix ovs_), issued from the developer dashboard at platform.overshoot.ai/api-keys.
  header: 'Authorization: Bearer <api_key>'
  name: API Key
  scheme: bearer
  sources:
  - openapi/overshoot-openapi.yaml
  - openapi/overshoot-inference-service.json
  type: http
slug: overshoot-authentication
source_filename: overshoot-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: openapi/overshoot-openapi.yaml\ndocs: https://docs.overshoot.ai/api-reference/authentication\nsummary:\n  types:\n  - http\n  style: Bearer API key\n  token_prefix: ovs_\n  key_issuance: https://platform.overshoot.ai/api-keys\nschemes:\n- name: API Key\n  type: http\n  scheme: bearer\n  bearer_format: 'API key (e.g. ovs_...)'\n  header: 'Authorization: Bearer <api_key>'\n  description: >-\n    Every public HTTP request requires an Authorization Bearer header carrying an\n    Overshoot API key (prefix ovs_), issued from the developer dashboard at\n    platform.overshoot.ai/api-keys.\n  sources:\n  - openapi/overshoot-openapi.yaml\n  - openapi/overshoot-inference-service.json\nunauthenticated_endpoints:\n- GET /models\n- GET /billing/pricing\n- GET /billing/pricing/{model}\nnotes:\n- '401 means the key is missing, unknown, or revoked.'\n- '403 means the key is valid but cannot access the requested resource.'\n- >-\n  The publish\
  \ token returned by POST /streams is only for publishing media to\n  LiveKit over WebRTC. It does not replace the API key for HTTP calls.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/overshoot/refs/heads/main/authentication/overshoot-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Artificial Intelligence
- Computer Vision
- Video
- Video Understanding
- Vision Language Models
- Real Time
- Streaming
- WebRTC
- Inference
- Multimodal
- Machine Learning
---
