---
api_key_in: []
api_specs:
- filename: lm-studio-server-openapi.yml
  format: yaml
  label: LM Studio Local Server API
  slug: lm-studio-local-server-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lm-studio/refs/heads/main/openapi/lm-studio-server-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Lm Studio Authentication
name_suffix: Authentication
oauth_flows: []
overview: LM Studio secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: LM Studio
provider_slug: lm-studio
scheme_count: 1
schemes:
- applies_to:
  - /api/v1
  name: ApiToken
  required: false
  scheme: bearer
  sources:
  - openapi/lm-studio-server-openapi.yml
  type: http
slug: lm-studio-authentication
source_filename: lm-studio-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://lmstudio.ai/docs/app/api/endpoints/rest\ndocs: https://lmstudio.ai/docs/app/api/endpoints/rest\nsummary:\n  types: [http]\n  http_schemes: [bearer]\n  default_posture: none\n  note: >-\n    The LM Studio local server runs on the developer's own machine (default\n    http://localhost:1234). By default it accepts unauthenticated requests over the\n    loopback interface. The native /api/v1 API adds OPTIONAL API-token authentication\n    that can be configured to require a bearer token — useful when the server is bound\n    to a non-loopback interface or exposed over LM Link. The OpenAI- and\n    Anthropic-compatible surfaces reuse the standard Authorization: Bearer header,\n    which existing OpenAI/Anthropic clients send but LM Studio does not require by\n    default.\nschemes:\n  - name: ApiToken\n    type: http\n    scheme: bearer\n    required: false\n    applies_to: [/api/v1]\n    sources: [openapi/lm-studio-server-openapi.yml]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lm-studio/refs/heads/main/authentication/lm-studio-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Ai
- Local LLM
- Machine Learning
- Inference
- Developer Tools
- LLM
- MCP
- SDK
- Desktop Application
---
