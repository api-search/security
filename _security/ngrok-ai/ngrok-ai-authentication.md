---
api_key_in:
- header
api_specs:
- filename: ngrok-ai-openapi.yml
  format: yaml
  label: ngrok AI Gateway
  slug: ai-gateway
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ngrok-ai/refs/heads/main/openapi/ngrok-ai-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Ngrok Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: ngrok AI Gateway secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: ngrok AI Gateway
provider_slug: ngrok-ai
scheme_count: 2
schemes:
- description: 'OpenAI-style authentication. Send the AI Gateway API key

    (format `ng-xxxxx-g1-xxxxx`) as `Authorization: Bearer <key>`.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/ngrok-ai-openapi.yml
  type: http
- description: 'Anthropic-style authentication. Send the AI Gateway API key

    (format `ng-xxxxx-g1-xxxxx`) in the `x-api-key` header.'
  in: header
  name: apiKeyAuth
  parameter: x-api-key
  sources:
  - openapi/ngrok-ai-openapi.yml
  type: apiKey
slug: ngrok-ai-authentication
source_filename: ngrok-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/ngrok-ai-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: |-\n    OpenAI-style authentication. Send the AI Gateway API key\n    (format `ng-xxxxx-g1-xxxxx`) as `Authorization: Bearer <key>`.\n  sources:\n  - openapi/ngrok-ai-openapi.yml\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: |-\n    Anthropic-style authentication. Send the AI Gateway API key\n    (format `ng-xxxxx-g1-xxxxx`) in the `x-api-key` header.\n  sources:\n  - openapi/ngrok-ai-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ngrok-ai/refs/heads/main/authentication/ngrok-ai-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- AI
- AI Gateway
- API Gateway
- LLM
- OpenAI Compatible
- Routing
- Security
- Traffic Management
---
