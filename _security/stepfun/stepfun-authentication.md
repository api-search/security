---
api_key_in:
- header
api_specs:
- filename: stepfun-realtime-asyncapi.yml
  format: yaml
  label: StepFun Realtime API
  slug: realtime-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/stepfun/refs/heads/main/asyncapi/stepfun-realtime-asyncapi.yml
auth_types:
- http-bearer-api-key
description: ''
kind: authentication
layout: security
method: searched
name: Stepfun Authentication
name_suffix: Authentication
oauth_flows: []
overview: StepFun secures its APIs with http-bearer-api-key across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: StepFun
provider_slug: stepfun
scheme_count: 1
schemes:
- description: 'Platform API key sent as "Authorization: Bearer <STEP_API_KEY>" on every request (REST and WebSocket). Keys are issued in the platform console under 接口密钥 (interface keys). The same key authorizes the StepSearch hosted MCP server. OpenAI/Anthropic SDKs pass it as their api_key with base_url pointed at https://api.stepfun.com.'
  key_console: https://platform.stepfun.com/interface-key
  name: bearerAuth
  scheme: bearer
  type: http
slug: stepfun-authentication
source_filename: stepfun-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\ndocs: https://platform.stepfun.com/docs/zh/quickstart/overview\nsource: >-\n  StepFun open-platform quickstart and API reference. No OpenAPI is published\n  (the docs' openapi.json is the Mintlify placeholder), so this profile is\n  captured from the documentation rather than derived from a spec.\nsummary:\n  types: [http-bearer-api-key]\n  api_key_in: [header]\n  oauth2_flows: []\nschemes:\n  - name: bearerAuth\n    type: http\n    scheme: bearer\n    description: >-\n      Platform API key sent as \"Authorization: Bearer <STEP_API_KEY>\" on every\n      request (REST and WebSocket). Keys are issued in the platform console\n      under 接口密钥 (interface keys). The same key authorizes the StepSearch\n      hosted MCP server. OpenAI/Anthropic SDKs pass it as their api_key with\n      base_url pointed at https://api.stepfun.com.\n    key_console: https://platform.stepfun.com/interface-key\nnotes:\n  - No OAuth 2.0, OIDC, or scoped-permission\
  \ surface is documented; access is all-or-nothing per API key.\n  - Step Plan subscription traffic authenticates the same way against the /step_plan/v1 prefix.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/stepfun/refs/heads/main/authentication/stepfun-authentication.yml
summary_line: http-bearer-api-key · 1 scheme
tags:
- AI
- Artificial Intelligence
- LLM
- Multimodal
- Chat Completion
- Audio
- Speech
- Text to Speech
- Speech Recognition
- Images
- Realtime
- Vector Stores
- China
---
