---
api_key_in: []
api_specs:
- filename: moonshot-ai-openapi.json
  format: json
  label: Moonshot AI Platform API
  slug: platform
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moonshot-ai/refs/heads/main/openapi/moonshot-ai-openapi.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Moonshot Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Moonshot AI secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Moonshot AI
provider_slug: moonshot-ai
scheme_count: 1
schemes:
- description: The Authorization header expects a Bearer token. Use an MOONSHOT_API_KEY as the token. This is a server-side secret key. Generate one on the [API keys page](https://platform.kimi.ai/console/api-keys) in your dashboard.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/moonshot-ai-openapi.json
  type: http
slug: moonshot-ai-authentication
source_filename: moonshot-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/moonshot-ai-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: The Authorization header expects a Bearer token. Use an MOONSHOT_API_KEY as the\n    token. This is a server-side secret key. Generate one on the [API keys page](https://platform.kimi.ai/console/api-keys)\n    in your dashboard.\n  sources:\n  - openapi/moonshot-ai-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/moonshot-ai/refs/heads/main/authentication/moonshot-ai-authentication.yml
summary_line: http · 1 scheme
tags:
- AI
- LLM
- Inference
- Long Context
- Kimi
---
