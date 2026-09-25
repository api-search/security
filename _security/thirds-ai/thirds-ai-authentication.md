---
anonymous_access: false
api_key_in:
- cookie
api_specs:
- filename: thirds-ai-openapi.yml
  format: yaml
  label: thirds.ai REST API
  slug: thirdsai-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thirds-ai/refs/heads/main/openapi/thirds-ai-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Thirds Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: thirds.ai secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: thirds.ai
provider_slug: thirds-ai
scheme_count: 2
schemes:
- description: A browser session. Browser writes also require the matching x-csrf-token header from GET /v1/me.
  in: cookie
  name: sessionCookie
  parameter: __Host-thirds_session
  sources:
  - openapi/thirds-ai-openapi.yml
  type: apiKey
- description: 'An API key''s secret, sent as "Authorization: Bearer thirds_sk_v1_...".'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/thirds-ai-openapi.yml
  type: http
slug: thirds-ai-authentication
source_filename: thirds-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-18'\nmethod: derived\nsource: openapi/thirds-ai-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - cookie\nschemes:\n- name: sessionCookie\n  type: apiKey\n  in: cookie\n  parameter: __Host-thirds_session\n  description: A browser session. Browser writes also require the matching x-csrf-token header\n    from GET /v1/me.\n  sources:\n  - openapi/thirds-ai-openapi.yml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'An API key''s secret, sent as \"Authorization: Bearer thirds_sk_v1_...\".'\n  sources:\n  - openapi/thirds-ai-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/thirds-ai/refs/heads/main/authentication/thirds-ai-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- pdf-automation
- image-automation
- Document Generation
- HTML to PDF
- HTML to Image
- template-rendering
- Branded Content
- Developer Tools
- MCP Server
- Agent-Native
- marketing-ops
---
