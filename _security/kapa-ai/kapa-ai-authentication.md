---
api_key_in:
- header
api_specs:
- filename: kapa-ai-openapi.yml
  format: yaml
  label: kapa.ai Query Chat API
  slug: kapa-ai-query-chat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kapa-ai/refs/heads/main/openapi/kapa-ai-openapi.yml
- filename: kapa-ai-openapi.yml
  format: yaml
  label: kapa.ai Threads Conversations API
  slug: kapa-ai-threads-conversations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kapa-ai/refs/heads/main/openapi/kapa-ai-openapi.yml
- filename: kapa-ai-openapi.yml
  format: yaml
  label: kapa.ai Search and Retrieval API
  slug: kapa-ai-search-retrieval-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kapa-ai/refs/heads/main/openapi/kapa-ai-openapi.yml
- filename: kapa-ai-openapi.yml
  format: yaml
  label: kapa.ai Projects API
  slug: kapa-ai-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kapa-ai/refs/heads/main/openapi/kapa-ai-openapi.yml
- filename: kapa-ai-openapi.yml
  format: yaml
  label: kapa.ai Analytics API
  slug: kapa-ai-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kapa-ai/refs/heads/main/openapi/kapa-ai-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Kapa Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: kapa.ai secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: kapa.ai
provider_slug: kapa-ai
scheme_count: 1
schemes:
- description: kapa.ai project API key, created in the API Keys tab of the platform.
  in: header
  name: ApiKeyAuth
  parameter: X-API-KEY
  sources:
  - openapi/kapa-ai-openapi.yml
  type: apiKey
slug: kapa-ai-authentication
source_filename: kapa-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/kapa-ai-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-KEY\n  description: kapa.ai project API key, created in the API Keys tab of the platform.\n  sources:\n  - openapi/kapa-ai-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kapa-ai/refs/heads/main/authentication/kapa-ai-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- AI
- Answer Engine
- RAG
- Documentation
- Developer Tools
---
