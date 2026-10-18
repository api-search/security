---
anonymous_access: false
api_key_in:
- header
- query
api_specs:
- filename: aihubmix-aihubmix-unified-api-api-openapi.yml
  format: yaml
  label: AIHubMix AIHubMix Unified API
  slug: aihubmix-aihubmix-unified-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aihubmix/refs/heads/main/openapi/aihubmix-aihubmix-unified-api-api-openapi.yml
- filename: aihubmix-anthropic-compatible-api-openapi.yml
  format: yaml
  label: AIHubMix Anthropic Compatible API
  slug: aihubmix-anthropic-compatible-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aihubmix/refs/heads/main/openapi/aihubmix-anthropic-compatible-api-openapi.yml
- filename: aihubmix-google-vertex-ai-compatible-api-openapi.yml
  format: yaml
  label: AIHubMix Google Vertex AI Compatible API
  slug: aihubmix-google-vertex-ai-compatible-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aihubmix/refs/heads/main/openapi/aihubmix-google-vertex-ai-compatible-api-openapi.yml
- filename: aihubmix-openai-compatible-api-openapi.yml
  format: yaml
  label: AIHubMix OpenAI Compatible API
  slug: aihubmix-openai-compatible-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aihubmix/refs/heads/main/openapi/aihubmix-openai-compatible-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 4
method: derived
name: Aihubmix Authentication
name_suffix: Authentication
oauth_flows: []
overview: AIHubMix secures its APIs with apiKey and http across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: AIHubMix
provider_slug: aihubmix
scheme_count: 4
schemes:
- bearerFormat: API Key
  description: 'Gateway-issued API key, formatted as `sk-gateway-xxxxxxxx`.

    Used by OpenAI-shaped endpoints (/v1/chat/completions, etc.).'
  name: gatewayBearer
  scheme: bearer
  sources:
  - openapi/aihubmix-openapi.yml
  type: http
- description: 'Used by Anthropic-shaped endpoints (/v1/messages). The value is

    the gateway API key, shared with OpenAI-shaped endpoints. Clients

    identifying as anthropic-sdk-* will use this header.'
  in: header
  name: gatewayAnthropicKey
  parameter: x-api-key
  sources:
  - openapi/aihubmix-openapi.yml
  type: apiKey
- description: 'Used by Gemini-shaped endpoints (/v1beta/...). The value is the

    gateway API key, shared with other endpoint shapes. The google-genai

    SDK uses this header by default.'
  in: header
  name: gatewayGeminiKey
  parameter: x-goog-api-key
  sources:
  - openapi/aihubmix-openapi.yml
  type: apiKey
- description: 'Query-parameter fallback for Gemini-shaped endpoints. Some SDKs

    and tools only support the `?key=` form. Value is the same as

    `gatewayGeminiKey`.'
  in: query
  name: gatewayGeminiQuery
  parameter: key
  sources:
  - openapi/aihubmix-openapi.yml
  type: apiKey
slug: aihubmix-authentication
source_filename: aihubmix-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-13'\nmethod: derived\nsource: openapi/aihubmix-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\n  - query\nschemes:\n- name: gatewayBearer\n  type: http\n  scheme: bearer\n  bearerFormat: API Key\n  description: |-\n    Gateway-issued API key, formatted as `sk-gateway-xxxxxxxx`.\n    Used by OpenAI-shaped endpoints (/v1/chat/completions, etc.).\n  sources:\n  - openapi/aihubmix-openapi.yml\n- name: gatewayAnthropicKey\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: |-\n    Used by Anthropic-shaped endpoints (/v1/messages). The value is\n    the gateway API key, shared with OpenAI-shaped endpoints. Clients\n    identifying as anthropic-sdk-* will use this header.\n  sources:\n  - openapi/aihubmix-openapi.yml\n- name: gatewayGeminiKey\n  type: apiKey\n  in: header\n  parameter: x-goog-api-key\n  description: |-\n    Used by Gemini-shaped endpoints (/v1beta/...). The value is the\n    gateway API key, shared\
  \ with other endpoint shapes. The google-genai\n    SDK uses this header by default.\n  sources:\n  - openapi/aihubmix-openapi.yml\n- name: gatewayGeminiQuery\n  type: apiKey\n  in: query\n  parameter: key\n  description: |-\n    Query-parameter fallback for Gemini-shaped endpoints. Some SDKs\n    and tools only support the `?key=` form. Value is the same as\n    `gatewayGeminiKey`.\n  sources:\n  - openapi/aihubmix-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aihubmix/refs/heads/main/authentication/aihubmix-authentication.yml
summary_line: apiKey/http · 4 schemes
tags:
- Company
- Artificial Intelligence
- LLM
- Model Routing
- AI Gateway
- Generative AI
- MCP
---
