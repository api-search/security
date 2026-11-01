---
anonymous_access: false
api_key_in: []
api_specs:
- filename: jarvisclaw-ai-a2a-api-openapi.yml
  format: yaml
  label: jarvisclaw-ai A2a API
  slug: jarvisclaw-ai-a2a-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jarvisclaw-ai/openapi/jarvisclaw-ai-a2a-api-openapi.yml
- filename: jarvisclaw-ai-audio-api-openapi.yml
  format: yaml
  label: jarvisclaw-ai Audio API
  slug: jarvisclaw-ai-audio-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jarvisclaw-ai/openapi/jarvisclaw-ai-audio-api-openapi.yml
- filename: jarvisclaw-ai-completions-api-openapi.yml
  format: yaml
  label: jarvisclaw-ai Completions API
  slug: jarvisclaw-ai-completions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jarvisclaw-ai/openapi/jarvisclaw-ai-completions-api-openapi.yml
- filename: jarvisclaw-ai-edits-api-openapi.yml
  format: yaml
  label: jarvisclaw-ai Edits API
  slug: jarvisclaw-ai-edits-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jarvisclaw-ai/openapi/jarvisclaw-ai-edits-api-openapi.yml
- filename: jarvisclaw-ai-embeddings-api-openapi.yml
  format: yaml
  label: jarvisclaw-ai Embeddings API
  slug: jarvisclaw-ai-embeddings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jarvisclaw-ai/openapi/jarvisclaw-ai-embeddings-api-openapi.yml
- filename: jarvisclaw-ai-images-api-openapi.yml
  format: yaml
  label: jarvisclaw-ai Images API
  slug: jarvisclaw-ai-images-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jarvisclaw-ai/openapi/jarvisclaw-ai-images-api-openapi.yml
- filename: jarvisclaw-ai-intent-api-openapi.yml
  format: yaml
  label: jarvisclaw-ai Intent API
  slug: jarvisclaw-ai-intent-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jarvisclaw-ai/openapi/jarvisclaw-ai-intent-api-openapi.yml
- filename: jarvisclaw-ai-marketplace-api-openapi.yml
  format: yaml
  label: jarvisclaw-ai Marketplace API
  slug: jarvisclaw-ai-marketplace-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jarvisclaw-ai/openapi/jarvisclaw-ai-marketplace-api-openapi.yml
- filename: jarvisclaw-ai-messages-api-openapi.yml
  format: yaml
  label: jarvisclaw-ai Messages API
  slug: jarvisclaw-ai-messages-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jarvisclaw-ai/openapi/jarvisclaw-ai-messages-api-openapi.yml
- filename: jarvisclaw-ai-moderations-api-openapi.yml
  format: yaml
  label: jarvisclaw-ai Moderations API
  slug: jarvisclaw-ai-moderations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jarvisclaw-ai/openapi/jarvisclaw-ai-moderations-api-openapi.yml
- filename: jarvisclaw-ai-prompt-coach-api-openapi.yml
  format: yaml
  label: jarvisclaw-ai Prompt Coach API
  slug: jarvisclaw-ai-prompt-coach-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jarvisclaw-ai/openapi/jarvisclaw-ai-prompt-coach-api-openapi.yml
- filename: jarvisclaw-ai-realtime-api-openapi.yml
  format: yaml
  label: jarvisclaw-ai Realtime API
  slug: jarvisclaw-ai-realtime-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jarvisclaw-ai/openapi/jarvisclaw-ai-realtime-api-openapi.yml
- filename: jarvisclaw-ai-rerank-api-openapi.yml
  format: yaml
  label: jarvisclaw-ai Rerank API
  slug: jarvisclaw-ai-rerank-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jarvisclaw-ai/openapi/jarvisclaw-ai-rerank-api-openapi.yml
- filename: jarvisclaw-ai-responses-api-openapi.yml
  format: yaml
  label: jarvisclaw-ai Responses API
  slug: jarvisclaw-ai-responses-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jarvisclaw-ai/openapi/jarvisclaw-ai-responses-api-openapi.yml
- filename: jarvisclaw-ai-search-api-openapi.yml
  format: yaml
  label: jarvisclaw-ai Search API
  slug: jarvisclaw-ai-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jarvisclaw-ai/openapi/jarvisclaw-ai-search-api-openapi.yml
- filename: jarvisclaw-ai-videos-api-openapi.yml
  format: yaml
  label: jarvisclaw-ai Videos API
  slug: jarvisclaw-ai-videos-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jarvisclaw-ai/openapi/jarvisclaw-ai-videos-api-openapi.yml
- filename: jarvisclaw-ai-chat-completions-api-openapi.yml
  format: yaml
  label: jarvisclaw-ai Chat Completions API
  slug: jarvisclaw-ai-chat-completions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jarvisclaw-ai/openapi/jarvisclaw-ai-chat-completions-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Jarvisclaw Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: jarvisclaw-ai declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: jarvisclaw-ai
provider_slug: jarvisclaw-ai
scheme_count: 2
schemes:
- description: 'JarvisClaw API key: Authorization: Bearer sk-...

    '
  scheme: bearer
  type: http
- description: 'x402 USDC payment via PAYMENT-SIGNATURE header

    '
  scheme: x402
  type: http
slug: jarvisclaw-ai-authentication
source_filename: jarvisclaw-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: derived\nsource:\n  - https://api.jarvisclaw.ai/openapi.json\nschemes:\n  - type: http\n    scheme: bearer\n    description: |\n      JarvisClaw API key: Authorization: Bearer sk-...\n  - type: http\n    scheme: x402\n    description: |\n      x402 USDC payment via PAYMENT-SIGNATURE header\n"
source_yaml_url: https://artifacts.apis.io/jarvisclaw-ai/authentication/jarvisclaw-ai-authentication.yml
summary_line: 2 schemes
tags:
- Company
- AI
- Payments
- Infrastructure
- Marketplace
---
