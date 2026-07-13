---
api_key_in:
- header
api_specs:
- filename: baseten-llm-openapi.json
  format: json
  label: Baseten LLM Inference API
  slug: llm-inference
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/baseten/refs/heads/main/openapi/baseten-llm-openapi.json
- filename: baseten-messages-openapi.json
  format: json
  label: Baseten Anthropic-Compatible Messages API
  slug: messages
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/baseten/refs/heads/main/openapi/baseten-messages-openapi.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Baseten Authentication
name_suffix: Authentication
oauth_flows: []
overview: Baseten secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Baseten
provider_slug: baseten
scheme_count: 1
schemes:
- description: 'Use `Api-Key` as the scheme in the Authorization header: `Authorization: Api-Key YOUR_API_KEY`.'
  in: header
  name: ApiKeyAuth
  parameter: Authorization
  sources:
  - openapi/baseten-llm-openapi.json
  - openapi/baseten-messages-openapi.json
  type: apiKey
slug: baseten-authentication
source_filename: baseten-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/baseten-llm-openapi.json, openapi/baseten-messages-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: 'Use `Api-Key` as the scheme in the Authorization header: `Authorization: Api-Key\n    YOUR_API_KEY`.'\n  sources:\n  - openapi/baseten-llm-openapi.json\n  - openapi/baseten-messages-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/baseten/refs/heads/main/authentication/baseten-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- AI
- ML
- Inference
- Deployment
- MLOps
- OpenAI Compatible
- Anthropic Compatible
- Truss
---
