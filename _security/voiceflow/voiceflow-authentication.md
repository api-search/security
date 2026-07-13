---
api_key_in:
- header
api_specs:
- filename: voiceflow-openapi.yml
  format: yaml
  label: Voiceflow Conversations API
  slug: conversations
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/voiceflow/refs/heads/main/openapi/voiceflow-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Voiceflow Authentication
name_suffix: Authentication
oauth_flows: []
overview: Voiceflow secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Voiceflow
provider_slug: voiceflow
scheme_count: 1
schemes:
- description: 'Voiceflow Dialog Manager API key (format `VF.DM.*`) sent in the

    `Authorization` header.'
  in: header
  name: apiKey
  parameter: Authorization
  sources:
  - openapi/voiceflow-openapi.yml
  type: apiKey
slug: voiceflow-authentication
source_filename: voiceflow-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/voiceflow-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: |-\n    Voiceflow Dialog Manager API key (format `VF.DM.*`) sent in the\n    `Authorization` header.\n  sources:\n  - openapi/voiceflow-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/voiceflow/refs/heads/main/authentication/voiceflow-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- AI
- Conversational
- Chat
- Voice
- Agent Builder
- Dialog Manager
---
