---
api_key_in: []
api_specs:
- filename: groq-openapi.yml
  format: yaml
  label: Groq Chat Completions API
  slug: groq-chat-completions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/groq/refs/heads/main/openapi/groq-openapi.yml
- filename: groq-openapi.yml
  format: yaml
  label: Groq Reasoning API
  slug: groq-reasoning-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/groq/refs/heads/main/openapi/groq-openapi.yml
- filename: groq-openapi.yml
  format: yaml
  label: Groq Vision API
  slug: groq-vision-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/groq/refs/heads/main/openapi/groq-openapi.yml
- filename: groq-openapi.yml
  format: yaml
  label: Groq Speech-to-Text API
  slug: groq-speech-to-text-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/groq/refs/heads/main/openapi/groq-openapi.yml
- filename: groq-openapi.yml
  format: yaml
  label: Groq Text-to-Speech API
  slug: groq-text-to-speech-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/groq/refs/heads/main/openapi/groq-openapi.yml
- filename: groq-openapi.yml
  format: yaml
  label: Groq Content Moderation API
  slug: groq-content-moderation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/groq/refs/heads/main/openapi/groq-openapi.yml
- filename: groq-openapi.yml
  format: yaml
  label: Groq Batch API
  slug: groq-batch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/groq/refs/heads/main/openapi/groq-openapi.yml
- filename: groq-openapi.yml
  format: yaml
  label: Groq Flex Processing API
  slug: groq-flex-processing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/groq/refs/heads/main/openapi/groq-openapi.yml
- filename: groq-openapi.yml
  format: yaml
  label: Groq Files API
  slug: groq-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/groq/refs/heads/main/openapi/groq-openapi.yml
- filename: groq-openapi.yml
  format: yaml
  label: Groq Models API
  slug: groq-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/groq/refs/heads/main/openapi/groq-openapi.yml
- filename: groq-openapi.yml
  format: yaml
  label: Groq Tools API
  slug: groq-tools-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/groq/refs/heads/main/openapi/groq-openapi.yml
- filename: groq-openapi.yml
  format: yaml
  label: Groq LoRA Inference API
  slug: groq-lora-inference-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/groq/refs/heads/main/openapi/groq-openapi.yml
- filename: groq-openapi.yml
  format: yaml
  label: Groq Prompt Caching
  slug: groq-prompt-caching-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/groq/refs/heads/main/openapi/groq-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Groq Authentication
name_suffix: Authentication
oauth_flows: []
overview: Groq secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Groq
provider_slug: groq
scheme_count: 1
schemes:
- bearerFormat: apiKey
  name: api_key
  scheme: bearer
  sources:
  - openapi/groq-openapi.yml
  type: http
slug: groq-authentication
source_filename: groq-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/groq-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: api_key\n  type: http\n  scheme: bearer\n  bearerFormat: apiKey\n  sources:\n  - openapi/groq-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/groq/refs/heads/main/authentication/groq-authentication.yml
summary_line: http · 1 scheme
tags:
- AI
- LLM
- Inference
- LPU
- Low Latency
---
