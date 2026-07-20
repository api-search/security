---
api_key_in: []
api_specs:
- filename: arcee-ai-afm-openapi.json
  format: json
  label: Arcee Platform API (AFM API)
  slug: arcee-platform-api-afm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arcee-ai/refs/heads/main/openapi/arcee-ai-afm-openapi.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Arcee Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Arcee AI secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Arcee AI
provider_slug: arcee-ai
scheme_count: 1
schemes:
- name: HTTPBearer
  scheme: bearer
  sources:
  - openapi/arcee-ai-afm-openapi.json
  type: http
slug: arcee-ai-authentication
source_filename: arcee-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: openapi/arcee-ai-afm-openapi.json\ndocs: https://docs.arcee.ai/api-reference/your-first-api-call\nsummary:\n  types:\n  - http\n  http_schemes:\n  - bearer\n  api_key_delivery: Authorization header, \"Bearer [example key]\"\n  key_management: https://docs.arcee.ai/other/platform-walkthrough/api-key-management\nnotes: >-\n  The Arcee Platform API uses bearer API keys. A key is created in the Arcee Platform dashboard\n  (API Keys management page) and passed on every request as an Authorization: Bearer header. The\n  inference surface is OpenAI-compatible, so the standard OpenAI client libraries authenticate by\n  setting this key. Interactive/platform login also supports GitHub and Google OAuth and a device\n  authorization flow (see /app/v1/oauth/* and /app/v1/device/* operations), but programmatic API\n  access is bearer-key only. No OAuth2 scope surface is documented.\nschemes:\n- name: HTTPBearer\n  type: http\n  scheme:\
  \ bearer\n  sources:\n  - openapi/arcee-ai-afm-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/arcee-ai/refs/heads/main/authentication/arcee-ai-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Ai
- Artificial Intelligence
- Machine Learning
- Large Language Models
- Small Language Models
- Inference
- Model Context Protocol
- Open Source
- Developer Platform
---
