---
anonymous_access: false
api_key_in:
- header
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Duami Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Duami secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Duami
provider_slug: duami-ai
scheme_count: 2
schemes:
- description: API key from POST /agents (mx_...)
  name: bearer
  scheme: bearer
  sources:
  - openapi/duami-ai-openapi.yml
  type: http
- description: RFC 9421 HTTP Message Signature with tag="web-bot-auth" (also send Signature and Signature-Agent). Registration only.
  in: header
  name: webBotAuth
  parameter: Signature-Input
  sources:
  - openapi/duami-ai-openapi.yml
  type: apiKey
slug: duami-ai-authentication
source_filename: duami-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-06'\nmethod: derived\nsource: openapi/duami-ai-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: bearer\n  type: http\n  scheme: bearer\n  description: API key from POST /agents (mx_...)\n  sources:\n  - openapi/duami-ai-openapi.yml\n- name: webBotAuth\n  type: apiKey\n  in: header\n  parameter: Signature-Input\n  description: RFC 9421 HTTP Message Signature with tag=\"web-bot-auth\" (also send Signature\n    and Signature-Agent). Registration only.\n  sources:\n  - openapi/duami-ai-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/duami-ai/authentication/duami-ai-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Artificial Intelligence
- Marketplace
- Agents
- Live
- Directory
---
