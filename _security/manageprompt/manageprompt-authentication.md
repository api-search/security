---
anonymous_access: false
api_key_in: []
api_specs:
- filename: manageprompt-actions-api-openapi.yml
  format: yaml
  label: ManagePrompt Actions API
  slug: manageprompt-actions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/manageprompt/refs/heads/main/openapi/manageprompt-actions-api-openapi.yml
- filename: manageprompt-sessions-api-openapi.yml
  format: yaml
  label: ManagePrompt Sessions API
  slug: manageprompt-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/manageprompt/refs/heads/main/openapi/manageprompt-sessions-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Manageprompt Authentication
name_suffix: Authentication
oauth_flows: []
overview: ManagePrompt secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: ManagePrompt
provider_slug: manageprompt
scheme_count: 1
schemes:
- bearerFormat: base64(userId:secret)
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/manageprompt-sessions.yaml
  type: http
slug: manageprompt-authentication
source_filename: manageprompt-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-18'\nmethod: derived\nsource: openapi/manageprompt-sessions.yaml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: base64(userId:secret)\n  sources:\n  - openapi/manageprompt-sessions.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/manageprompt/refs/heads/main/authentication/manageprompt-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- LLM
- Debugging
- OpenSource
- DeveloperTools
---
