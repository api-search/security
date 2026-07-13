---
api_key_in:
- header
api_specs:
- filename: anthropic-claude-openapi.yml
  format: yaml
  label: Anthropic Claude Messages API
  slug: messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anthropic-claude/refs/heads/main/openapi/anthropic-claude-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Anthropic Claude Authentication
name_suffix: Authentication
oauth_flows: []
overview: Anthropic Claude secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Anthropic Claude
provider_slug: anthropic-claude
scheme_count: 1
schemes:
- description: Anthropic API key. Send as the `x-api-key` header on every request.
  in: header
  name: ApiKeyAuth
  parameter: x-api-key
  sources:
  - openapi/anthropic-claude-openapi.yml
  type: apiKey
slug: anthropic-claude-authentication
source_filename: anthropic-claude-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/anthropic-claude-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: Anthropic API key. Send as the `x-api-key` header on every request.\n  sources:\n  - openapi/anthropic-claude-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/anthropic-claude/refs/heads/main/authentication/anthropic-claude-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Artificial Intelligence
- Large Language Models
- LLM
- Generative AI
- Chat
- Agents
- Claude
---
