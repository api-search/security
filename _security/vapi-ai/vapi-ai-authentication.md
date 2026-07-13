---
api_key_in: []
api_specs:
- filename: vapi-assistants-api-openapi.yml
  format: yaml
  label: Vapi Assistants API
  slug: vapi-assistants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vapi-ai/refs/heads/main/openapi/vapi-assistants-api-openapi.yml
- filename: vapi-calls-api-openapi.yml
  format: yaml
  label: Vapi Calls API
  slug: vapi-calls-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vapi-ai/refs/heads/main/openapi/vapi-calls-api-openapi.yml
- filename: vapi-phone-numbers-api-openapi.yml
  format: yaml
  label: Vapi Phone Numbers API
  slug: vapi-phone-numbers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vapi-ai/refs/heads/main/openapi/vapi-phone-numbers-api-openapi.yml
- filename: vapi-squads-api-openapi.yml
  format: yaml
  label: Vapi Squads API
  slug: vapi-squads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vapi-ai/refs/heads/main/openapi/vapi-squads-api-openapi.yml
- filename: vapi-tools-api-openapi.yml
  format: yaml
  label: Vapi Tools API
  slug: vapi-tools-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vapi-ai/refs/heads/main/openapi/vapi-tools-api-openapi.yml
- filename: vapi-files-api-openapi.yml
  format: yaml
  label: Vapi Files API
  slug: vapi-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vapi-ai/refs/heads/main/openapi/vapi-files-api-openapi.yml
- filename: vapi-chats-api-openapi.yml
  format: yaml
  label: Vapi Chats API
  slug: vapi-chats-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vapi-ai/refs/heads/main/openapi/vapi-chats-api-openapi.yml
- filename: vapi-sessions-api-openapi.yml
  format: yaml
  label: Vapi Sessions API
  slug: vapi-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vapi-ai/refs/heads/main/openapi/vapi-sessions-api-openapi.yml
- filename: vapi-campaigns-api-openapi.yml
  format: yaml
  label: Vapi Campaigns API
  slug: vapi-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vapi-ai/refs/heads/main/openapi/vapi-campaigns-api-openapi.yml
- filename: vapi-analytics-api-openapi.yml
  format: yaml
  label: Vapi Analytics API
  slug: vapi-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vapi-ai/refs/heads/main/openapi/vapi-analytics-api-openapi.yml
- filename: vapi-insight-api-openapi.yml
  format: yaml
  label: Vapi Insight API
  slug: vapi-insight-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vapi-ai/refs/heads/main/openapi/vapi-insight-api-openapi.yml
- filename: vapi-observability-api-openapi.yml
  format: yaml
  label: Vapi Observability Scorecard API
  slug: vapi-observability-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vapi-ai/refs/heads/main/openapi/vapi-observability-api-openapi.yml
- filename: vapi-eval-api-openapi.yml
  format: yaml
  label: Vapi Eval API
  slug: vapi-eval-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vapi-ai/refs/heads/main/openapi/vapi-eval-api-openapi.yml
- filename: vapi-structured-outputs-api-openapi.yml
  format: yaml
  label: Vapi Structured Outputs API
  slug: vapi-structured-outputs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vapi-ai/refs/heads/main/openapi/vapi-structured-outputs-api-openapi.yml
- filename: vapi-provider-resources-api-openapi.yml
  format: yaml
  label: Vapi Provider Resources API
  slug: vapi-provider-resources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vapi-ai/refs/heads/main/openapi/vapi-provider-resources-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Vapi Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Vapi secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Vapi
provider_slug: vapi-ai
scheme_count: 1
schemes:
- bearerFormat: Bearer
  description: Retrieve your API Key from [Dashboard](dashboard.vapi.ai).
  name: bearer
  scheme: bearer
  sources:
  - openapi/vapi-analytics-api-openapi.yml
  - openapi/vapi-assistants-api-openapi.yml
  - openapi/vapi-calls-api-openapi.yml
  - openapi/vapi-campaigns-api-openapi.yml
  - openapi/vapi-chats-api-openapi.yml
  - openapi/vapi-eval-api-openapi.yml
  - openapi/vapi-files-api-openapi.yml
  - openapi/vapi-insight-api-openapi.yml
  - openapi/vapi-observability-api-openapi.yml
  - openapi/vapi-phone-numbers-api-openapi.yml
  - openapi/vapi-provider-resources-api-openapi.yml
  - openapi/vapi-sessions-api-openapi.yml
  - openapi/vapi-squads-api-openapi.yml
  - openapi/vapi-structured-outputs-api-openapi.yml
  - openapi/vapi-tools-api-openapi.yml
  type: http
slug: vapi-ai-authentication
source_filename: vapi-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/vapi-analytics-api-openapi.yml, openapi/vapi-assistants-api-openapi.yml, openapi/vapi-calls-api-openapi.yml,\n  openapi/vapi-campaigns-api-openapi.yml, openapi/vapi-chats-api-openapi.yml, openapi/vapi-eval-api-openapi.yml,\n  openapi/vapi-files-api-openapi.yml, openapi/vapi-insight-api-openapi.yml, openapi/vapi-observability-api-openapi.yml,\n  openapi/vapi-phone-numbers-api-openapi.yml, openapi/vapi-provider-resources-api-openapi.yml,\n  openapi/vapi-sessions-api-openapi.yml ...\nsummary:\n  types:\n  - http\nschemes:\n- name: bearer\n  type: http\n  scheme: bearer\n  bearerFormat: Bearer\n  description: Retrieve your API Key from [Dashboard](dashboard.vapi.ai).\n  sources:\n  - openapi/vapi-analytics-api-openapi.yml\n  - openapi/vapi-assistants-api-openapi.yml\n  - openapi/vapi-calls-api-openapi.yml\n  - openapi/vapi-campaigns-api-openapi.yml\n  - openapi/vapi-chats-api-openapi.yml\n  - openapi/vapi-eval-api-openapi.yml\n\
  \  - openapi/vapi-files-api-openapi.yml\n  - openapi/vapi-insight-api-openapi.yml\n  - openapi/vapi-observability-api-openapi.yml\n  - openapi/vapi-phone-numbers-api-openapi.yml\n  - openapi/vapi-provider-resources-api-openapi.yml\n  - openapi/vapi-sessions-api-openapi.yml\n  - openapi/vapi-squads-api-openapi.yml\n  - openapi/vapi-structured-outputs-api-openapi.yml\n  - openapi/vapi-tools-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vapi-ai/refs/heads/main/authentication/vapi-ai-authentication.yml
summary_line: http · 1 scheme
tags:
- AI
- Voice AI
- Voice Agents
- Conversational AI
- Telephony
- Real-Time
- Transcription
- Text-to-Speech
- LLM
- Agents
- MCP
---
