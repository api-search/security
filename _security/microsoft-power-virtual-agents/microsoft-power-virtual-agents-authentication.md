---
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Microsoft Power Virtual Agents Authentication
name_suffix: Authentication
oauth_flows: []
overview: Microsoft Power Virtual Agents secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Microsoft Power Virtual Agents
provider_slug: microsoft-power-virtual-agents
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: Direct Line authentication uses either a long-lived secret or a short-lived token. Supply the value in the Authorization header as `Bearer {secret-or-token}`.
  name: bearer
  scheme: bearer
  sources:
  - openapi/microsoft-power-virtual-agents-openapi.yml
  type: http
slug: microsoft-power-virtual-agents-authentication
source_filename: microsoft-power-virtual-agents-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/microsoft-power-virtual-agents-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearer\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: Direct Line authentication uses either a long-lived secret or a short-lived token.\n    Supply the value in the Authorization header as `Bearer {secret-or-token}`.\n  sources:\n  - openapi/microsoft-power-virtual-agents-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microsoft-power-virtual-agents/refs/heads/main/authentication/microsoft-power-virtual-agents-authentication.yml
summary_line: http · 1 scheme
tags:
- Chatbots
- Conversational AI
- Copilot Studio
- Microsoft
---
