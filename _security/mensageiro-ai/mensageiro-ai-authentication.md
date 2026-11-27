---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: mensageiro-ai-audio-api-openapi.yml
  format: yaml
  label: Mensageiro Audio API
  slug: mensageiro-ai-audio-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mensageiro-ai/openapi/mensageiro-ai-audio-api-openapi.yml
- filename: mensageiro-ai-balance-api-openapi.yml
  format: yaml
  label: Mensageiro Balance API
  slug: mensageiro-ai-balance-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mensageiro-ai/openapi/mensageiro-ai-balance-api-openapi.yml
- filename: mensageiro-ai-batch-api-openapi.yml
  format: yaml
  label: Mensageiro Batch API
  slug: mensageiro-ai-batch-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mensageiro-ai/openapi/mensageiro-ai-batch-api-openapi.yml
- filename: mensageiro-ai-chat-api-openapi.yml
  format: yaml
  label: Mensageiro Chat API
  slug: mensageiro-ai-chat-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mensageiro-ai/openapi/mensageiro-ai-chat-api-openapi.yml
- filename: mensageiro-ai-exports-api-openapi.yml
  format: yaml
  label: Mensageiro Exports API
  slug: mensageiro-ai-exports-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mensageiro-ai/openapi/mensageiro-ai-exports-api-openapi.yml
- filename: mensageiro-ai-guardrails-api-openapi.yml
  format: yaml
  label: Mensageiro Guardrails API
  slug: mensageiro-ai-guardrails-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mensageiro-ai/openapi/mensageiro-ai-guardrails-api-openapi.yml
- filename: mensageiro-ai-invoices-api-openapi.yml
  format: yaml
  label: Mensageiro Invoices API
  slug: mensageiro-ai-invoices-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mensageiro-ai/openapi/mensageiro-ai-invoices-api-openapi.yml
- filename: mensageiro-ai-keys-api-openapi.yml
  format: yaml
  label: Mensageiro Keys API
  slug: mensageiro-ai-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mensageiro-ai/openapi/mensageiro-ai-keys-api-openapi.yml
- filename: mensageiro-ai-mcp-api-openapi.yml
  format: yaml
  label: Mensageiro MCP API
  slug: mensageiro-ai-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mensageiro-ai/openapi/mensageiro-ai-mcp-api-openapi.yml
- filename: mensageiro-ai-media-api-openapi.yml
  format: yaml
  label: Mensageiro Media API
  slug: mensageiro-ai-media-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mensageiro-ai/openapi/mensageiro-ai-media-api-openapi.yml
- filename: mensageiro-ai-meta-api-openapi.yml
  format: yaml
  label: Mensageiro Meta API
  slug: mensageiro-ai-meta-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mensageiro-ai/openapi/mensageiro-ai-meta-api-openapi.yml
- filename: mensageiro-ai-models-api-openapi.yml
  format: yaml
  label: Mensageiro Models API
  slug: mensageiro-ai-models-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mensageiro-ai/openapi/mensageiro-ai-models-api-openapi.yml
- filename: mensageiro-ai-presets-api-openapi.yml
  format: yaml
  label: Mensageiro Presets API
  slug: mensageiro-ai-presets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mensageiro-ai/openapi/mensageiro-ai-presets-api-openapi.yml
- filename: mensageiro-ai-pricing-api-openapi.yml
  format: yaml
  label: Mensageiro Pricing API
  slug: mensageiro-ai-pricing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mensageiro-ai/openapi/mensageiro-ai-pricing-api-openapi.yml
- filename: mensageiro-ai-receipts-api-openapi.yml
  format: yaml
  label: Mensageiro Receipts API
  slug: mensageiro-ai-receipts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mensageiro-ai/openapi/mensageiro-ai-receipts-api-openapi.yml
- filename: mensageiro-ai-search-api-openapi.yml
  format: yaml
  label: Mensageiro Search API
  slug: mensageiro-ai-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mensageiro-ai/openapi/mensageiro-ai-search-api-openapi.yml
- filename: mensageiro-ai-sessions-api-openapi.yml
  format: yaml
  label: Mensageiro Sessions API
  slug: mensageiro-ai-sessions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mensageiro-ai/openapi/mensageiro-ai-sessions-api-openapi.yml
- filename: mensageiro-ai-sign-in-api-openapi.yml
  format: yaml
  label: Mensageiro Sign In API
  slug: mensageiro-ai-sign-in-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mensageiro-ai/openapi/mensageiro-ai-sign-in-api-openapi.yml
- filename: mensageiro-ai-status-api-openapi.yml
  format: yaml
  label: Mensageiro Status API
  slug: mensageiro-ai-status-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mensageiro-ai/openapi/mensageiro-ai-status-api-openapi.yml
- filename: mensageiro-ai-webhooks-api-openapi.yml
  format: yaml
  label: Mensageiro Webhooks API
  slug: mensageiro-ai-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mensageiro-ai/openapi/mensageiro-ai-webhooks-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: derived
name: Mensageiro Authentication
name_suffix: Authentication
oauth_flows: []
overview: Mensageiro secures its APIs with apiKey and http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Mensageiro
provider_slug: mensageiro-ai
scheme_count: 3
schemes:
- description: '`Authorization: Bearer sk-msg-live-...`. The OpenAI SDK sends this.'
  name: bearer
  scheme: bearer
  sources:
  - openapi/mensageiro-ai-openapi.json
  type: http
- description: The same key in `x-api-key`, as the Anthropic SDK sends it. On GET /v1/models it selects Anthropic's list shape.
  in: header
  name: apiKey
  parameter: x-api-key
  sources:
  - openapi/mensageiro-ai-openapi.json
  type: apiKey
- description: The same key in `x-goog-api-key`, as the Gemini SDK sends it. On GET /v1/models it selects Google's list shape.
  in: header
  name: googleApiKey
  parameter: x-goog-api-key
  sources:
  - openapi/mensageiro-ai-openapi.json
  type: apiKey
slug: mensageiro-ai-authentication
source_filename: mensageiro-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-16'\nmethod: derived\nsource: openapi/mensageiro-ai-openapi.json\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: bearer\n  type: http\n  scheme: bearer\n  description: '`Authorization: Bearer sk-msg-live-...`. The OpenAI SDK sends this.'\n  sources:\n  - openapi/mensageiro-ai-openapi.json\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: The same key in `x-api-key`, as the Anthropic SDK sends it. On GET /v1/models\n    it selects Anthropic's list shape.\n  sources:\n  - openapi/mensageiro-ai-openapi.json\n- name: googleApiKey\n  type: apiKey\n  in: header\n  parameter: x-goog-api-key\n  description: The same key in `x-goog-api-key`, as the Gemini SDK sends it. On GET /v1/models\n    it selects Google's list shape.\n  sources:\n  - openapi/mensageiro-ai-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/mensageiro-ai/authentication/mensageiro-ai-authentication.yml
summary_line: apiKey/http · 3 schemes
tags:
- WhatsApp
- AI Chatbot
---
