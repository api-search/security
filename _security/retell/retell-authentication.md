---
api_key_in: []
api_specs:
- filename: retell-agent-api-openapi.yml
  format: yaml
  label: Retell AI Agent API
  slug: retell-agent-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/retell/refs/heads/main/openapi/retell-agent-api-openapi.yml
- filename: retell-batch-call-api-openapi.yml
  format: yaml
  label: Retell AI Batch Call API
  slug: retell-batch-call-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/retell/refs/heads/main/openapi/retell-batch-call-api-openapi.yml
- filename: retell-call-api-openapi.yml
  format: yaml
  label: Retell AI Call API
  slug: retell-call-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/retell/refs/heads/main/openapi/retell-call-api-openapi.yml
- filename: retell-concurrency-api-openapi.yml
  format: yaml
  label: Retell AI Concurrency API
  slug: retell-concurrency-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/retell/refs/heads/main/openapi/retell-concurrency-api-openapi.yml
- filename: retell-conversation-flow-api-openapi.yml
  format: yaml
  label: Retell AI Conversation Flow API
  slug: retell-conversation-flow-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/retell/refs/heads/main/openapi/retell-conversation-flow-api-openapi.yml
- filename: retell-knowledge-base-api-openapi.yml
  format: yaml
  label: Retell AI Knowledge Base API
  slug: retell-knowledge-base-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/retell/refs/heads/main/openapi/retell-knowledge-base-api-openapi.yml
- filename: retell-phone-call-api-openapi.yml
  format: yaml
  label: Retell AI Phone Call API
  slug: retell-phone-call-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/retell/refs/heads/main/openapi/retell-phone-call-api-openapi.yml
- filename: retell-phone-number-api-openapi.yml
  format: yaml
  label: Retell AI Phone Number API
  slug: retell-phone-number-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/retell/refs/heads/main/openapi/retell-phone-number-api-openapi.yml
- filename: retell-retell-llm-api-openapi.yml
  format: yaml
  label: Retell AI Retell LLM API
  slug: retell-retell-llm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/retell/refs/heads/main/openapi/retell-retell-llm-api-openapi.yml
- filename: retell-voice-api-openapi.yml
  format: yaml
  label: Retell AI Voice API
  slug: retell-voice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/retell/refs/heads/main/openapi/retell-voice-api-openapi.yml
- filename: retell-web-call-api-openapi.yml
  format: yaml
  label: Retell AI Web Call API
  slug: retell-web-call-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/retell/refs/heads/main/openapi/retell-web-call-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Retell Authentication
name_suffix: Authentication
oauth_flows: []
overview: Retell AI secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Retell AI
provider_slug: retell
scheme_count: 1
schemes:
- bearerFormat: apiKey
  description: 'Retell API key, sent as: Authorization: Bearer <RETELL_API_KEY>'
  name: api_key
  scheme: bearer
  sources:
  - openapi/retell-openapi.yml
  type: http
slug: retell-authentication
source_filename: retell-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/retell-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: api_key\n  type: http\n  scheme: bearer\n  bearerFormat: apiKey\n  description: 'Retell API key, sent as: Authorization: Bearer <RETELL_API_KEY>'\n  sources:\n  - openapi/retell-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/retell/refs/heads/main/authentication/retell-authentication.yml
summary_line: http · 1 scheme
tags:
- AI
- Voice
- Voice Agents
- Conversational AI
- Telephony
---
