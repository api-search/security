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
name: Aireiter Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: AIReiter secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: AIReiter
provider_slug: aireiter-com
scheme_count: 2
schemes:
- description: 'Authorization: Bearer <api-key>'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/aireiter-com-openapi.json
  type: http
- in: header
  name: apiKeyHeader
  parameter: x-api-key
  sources:
  - openapi/aireiter-com-openapi.json
  type: apiKey
slug: aireiter-com-authentication
source_filename: aireiter-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: derived\nsource: openapi/aireiter-com-openapi.json\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'Authorization: Bearer <api-key>'\n  sources:\n  - openapi/aireiter-com-openapi.json\n- name: apiKeyHeader\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  sources:\n  - openapi/aireiter-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/aireiter-com/authentication/aireiter-com-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- AI
- Multimodal
- Generation
- OpenAI-Compatible
- Credit-Pricing
---
