---
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Botpress Authentication
name_suffix: Authentication
oauth_flows: []
overview: Botpress secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Botpress
provider_slug: botpress
scheme_count: 1
schemes:
- description: Personal access token or workspace API key passed as a Bearer token.
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/botpress-openapi.yml
  type: http
slug: botpress-authentication
source_filename: botpress-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/botpress-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: Personal access token or workspace API key passed as a Bearer token.\n  sources:\n  - openapi/botpress-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/botpress/refs/heads/main/authentication/botpress-authentication.yml
summary_line: http · 1 scheme
tags:
- AI
- Conversational
- Chat
- Open Source
- Bot Builder
- LLM
---
