---
api_key_in: []
api_specs:
- filename: vercel-webhooks-asyncapi.yml
  format: yaml
  label: Vercel Webhooks
  slug: vercel-webhooks
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/vercel/refs/heads/main/asyncapi/vercel-webhooks-asyncapi.yml
- filename: vercel-chat-api-openapi.yml
  format: yaml
  label: Vercel Chat API
  slug: vercel-chat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vercel/refs/heads/main/openapi/vercel-chat-api-openapi.yml
- filename: vercel-chats-api-openapi.yml
  format: yaml
  label: Vercel Chats API
  slug: vercel-chats-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vercel/refs/heads/main/openapi/vercel-chats-api-openapi.yml
- filename: vercel-embeddings-api-openapi.yml
  format: yaml
  label: Vercel Embeddings API
  slug: vercel-embeddings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vercel/refs/heads/main/openapi/vercel-embeddings-api-openapi.yml
- filename: vercel-models-api-openapi.yml
  format: yaml
  label: Vercel Models API
  slug: vercel-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vercel/refs/heads/main/openapi/vercel-models-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Vercel Authentication
name_suffix: Authentication
oauth_flows: []
overview: Vercel secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Vercel
provider_slug: vercel
scheme_count: 1
schemes:
- description: Vercel AI Gateway API key (AI_GATEWAY_API_KEY)
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/vercel-ai-gateway-openapi.yml
  - openapi/vercel-v0-platform-openapi.yml
  type: http
slug: vercel-authentication
source_filename: vercel-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/vercel-ai-gateway-openapi.yml, openapi/vercel-v0-platform-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: Vercel AI Gateway API key (AI_GATEWAY_API_KEY)\n  sources:\n  - openapi/vercel-ai-gateway-openapi.yml\n  - openapi/vercel-v0-platform-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vercel/refs/heads/main/authentication/vercel-authentication.yml
summary_line: http · 1 scheme
tags:
- AI Gateways
- Gateways
- Observability
- Webhook
---
