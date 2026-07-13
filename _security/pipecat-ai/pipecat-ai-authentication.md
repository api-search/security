---
api_key_in: []
api_specs:
- filename: pipecat-ai-openapi.yml
  format: yaml
  label: Pipecat Cloud (Agents/Sessions API)
  slug: pipecat-cloud-agents-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pipecat-ai/refs/heads/main/openapi/pipecat-ai-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Pipecat Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Pipecat secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Pipecat
provider_slug: pipecat-ai
scheme_count: 1
schemes:
- description: Private API key from the Pipecat Cloud dashboard, sent as a Bearer token.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/pipecat-ai-openapi.yml
  type: http
slug: pipecat-ai-authentication
source_filename: pipecat-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/pipecat-ai-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Private API key from the Pipecat Cloud dashboard, sent as a Bearer token.\n  sources:\n  - openapi/pipecat-ai-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pipecat-ai/refs/heads/main/authentication/pipecat-ai-authentication.yml
summary_line: http · 1 scheme
tags:
- AI
- Voice
- Multimodal
- Agents
- Realtime
- Framework
---
