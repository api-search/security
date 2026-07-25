---
api_key_in: []
api_specs:
- filename: livepeer-accesscontrol-api-openapi.yml
  format: yaml
  label: Livepeer accessControl API
  slug: livepeer-accesscontrol-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/livepeer/refs/heads/main/openapi/livepeer-accesscontrol-api-openapi.yml
- filename: livepeer-asset-api-openapi.yml
  format: yaml
  label: Livepeer asset API
  slug: livepeer-asset-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/livepeer/refs/heads/main/openapi/livepeer-asset-api-openapi.yml
- filename: livepeer-generate-api-openapi.yml
  format: yaml
  label: Livepeer generate API
  slug: livepeer-generate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/livepeer/refs/heads/main/openapi/livepeer-generate-api-openapi.yml
- filename: livepeer-metrics-api-openapi.yml
  format: yaml
  label: Livepeer metrics API
  slug: livepeer-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/livepeer/refs/heads/main/openapi/livepeer-metrics-api-openapi.yml
- filename: livepeer-multistream-api-openapi.yml
  format: yaml
  label: Livepeer multistream API
  slug: livepeer-multistream-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/livepeer/refs/heads/main/openapi/livepeer-multistream-api-openapi.yml
- filename: livepeer-playback-api-openapi.yml
  format: yaml
  label: Livepeer playback API
  slug: livepeer-playback-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/livepeer/refs/heads/main/openapi/livepeer-playback-api-openapi.yml
- filename: livepeer-room-api-openapi.yml
  format: yaml
  label: Livepeer room API
  slug: livepeer-room-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/livepeer/refs/heads/main/openapi/livepeer-room-api-openapi.yml
- filename: livepeer-session-api-openapi.yml
  format: yaml
  label: Livepeer session API
  slug: livepeer-session-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/livepeer/refs/heads/main/openapi/livepeer-session-api-openapi.yml
- filename: livepeer-stream-api-openapi.yml
  format: yaml
  label: Livepeer stream API
  slug: livepeer-stream-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/livepeer/refs/heads/main/openapi/livepeer-stream-api-openapi.yml
- filename: livepeer-task-api-openapi.yml
  format: yaml
  label: Livepeer task API
  slug: livepeer-task-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/livepeer/refs/heads/main/openapi/livepeer-task-api-openapi.yml
- filename: livepeer-transcode-api-openapi.yml
  format: yaml
  label: Livepeer transcode API
  slug: livepeer-transcode-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/livepeer/refs/heads/main/openapi/livepeer-transcode-api-openapi.yml
- filename: livepeer-webhook-api-openapi.yml
  format: yaml
  label: Livepeer webhook API
  slug: livepeer-webhook-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/livepeer/refs/heads/main/openapi/livepeer-webhook-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Livepeer Authentication
name_suffix: Authentication
oauth_flows: []
overview: Livepeer secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Livepeer
provider_slug: livepeer
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: apiKey
  scheme: bearer
  sources:
  - openapi/livepeer-openapi.yml
  type: http
slug: livepeer-authentication
source_filename: livepeer-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/livepeer-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: apiKey\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/livepeer-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/livepeer/refs/heads/main/authentication/livepeer-authentication.yml
summary_line: http · 1 scheme
tags:
- Video
- Streaming
- Transcoding
- Decentralized
- Web3
- Live Video
- AI Video
---
