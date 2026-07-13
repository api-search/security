---
api_key_in: []
api_specs:
- filename: retell-openapi.yml
  format: yaml
  label: Agents
  slug: agents
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/retell/refs/heads/main/openapi/retell-openapi.yml
- filename: retell-openapi.yml
  format: yaml
  label: Retell LLM
  slug: retell-llm
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/retell/refs/heads/main/openapi/retell-openapi.yml
- filename: retell-openapi.yml
  format: yaml
  label: Conversation Flow
  slug: conversation-flow
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/retell/refs/heads/main/openapi/retell-openapi.yml
- filename: retell-openapi.yml
  format: yaml
  label: Phone Calls
  slug: phone-calls
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/retell/refs/heads/main/openapi/retell-openapi.yml
- filename: retell-openapi.yml
  format: yaml
  label: Web Calls
  slug: web-calls
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/retell/refs/heads/main/openapi/retell-openapi.yml
- filename: retell-openapi.yml
  format: yaml
  label: Phone Numbers
  slug: phone-numbers
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/retell/refs/heads/main/openapi/retell-openapi.yml
- filename: retell-openapi.yml
  format: yaml
  label: Voices
  slug: voices
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/retell/refs/heads/main/openapi/retell-openapi.yml
- filename: retell-openapi.yml
  format: yaml
  label: Knowledge Bases
  slug: knowledge-bases
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/retell/refs/heads/main/openapi/retell-openapi.yml
- filename: retell-openapi.yml
  format: yaml
  label: Batch Call
  slug: batch-call
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/retell/refs/heads/main/openapi/retell-openapi.yml
- filename: retell-openapi.yml
  format: yaml
  label: Concurrency
  slug: concurrency
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/retell/refs/heads/main/openapi/retell-openapi.yml
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
