---
api_key_in:
- header
api_specs:
- filename: claude-messages-api.yml
  format: yaml
  label: Claude Messages API
  slug: claude-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/claude/refs/heads/main/openapi/claude-messages-api.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Claude Authentication
name_suffix: Authentication
oauth_flows: []
overview: Claude secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Claude
provider_slug: claude
scheme_count: 1
schemes:
- description: API key for authenticating requests. Obtain from the Anthropic Console at https://console.anthropic.com
  in: header
  name: ApiKeyAuth
  parameter: x-api-key
  sources:
  - openapi/claude-messages-api.yml
  type: apiKey
slug: claude-authentication
source_filename: claude-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/claude-messages-api.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: API key for authenticating requests. Obtain from the Anthropic Console at https://console.anthropic.com\n  sources:\n  - openapi/claude-messages-api.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/claude/refs/heads/main/authentication/claude-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Artificial Intelligence
- Chatbot
- Conversational AI
- Generative AI
- Large Language Models
- Machine Learning
- Natural Language Processing
---
