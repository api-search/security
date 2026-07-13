---
api_key_in:
- header
api_specs:
- filename: bland-ai-openapi.yml
  format: yaml
  label: Bland AI Platform API
  slug: platform
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bland-ai/refs/heads/main/openapi/bland-ai-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Bland Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Bland AI secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Bland AI
provider_slug: bland-ai
scheme_count: 1
schemes:
- description: Bland API key supplied as the raw value of the `authorization` header.
  in: header
  name: apiKey
  parameter: authorization
  sources:
  - openapi/bland-ai-openapi.yml
  type: apiKey
slug: bland-ai-authentication
source_filename: bland-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/bland-ai-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: authorization\n  description: Bland API key supplied as the raw value of the `authorization` header.\n  sources:\n  - openapi/bland-ai-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bland-ai/refs/heads/main/authentication/bland-ai-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- AI
- Voice
- Agents
- Phone
- Realtime
---
