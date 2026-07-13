---
api_key_in: []
api_specs:
- filename: haystack-ai-openapi.yml
  format: yaml
  label: deepset Cloud API - Pipelines
  slug: deepset-cloud-pipelines-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/haystack-ai/refs/heads/main/openapi/haystack-ai-openapi.yml
- filename: haystack-ai-openapi.yml
  format: yaml
  label: deepset Cloud API - Search
  slug: deepset-cloud-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/haystack-ai/refs/heads/main/openapi/haystack-ai-openapi.yml
- filename: haystack-ai-openapi.yml
  format: yaml
  label: deepset Cloud API - Files
  slug: deepset-cloud-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/haystack-ai/refs/heads/main/openapi/haystack-ai-openapi.yml
- filename: haystack-ai-openapi.yml
  format: yaml
  label: deepset Cloud API - Workspaces
  slug: deepset-cloud-workspaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/haystack-ai/refs/heads/main/openapi/haystack-ai-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Haystack Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Haystack / deepset secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Haystack / deepset
provider_slug: haystack-ai
scheme_count: 1
schemes:
- description: API key generated in the deepset AI Platform UI, sent as a Bearer token.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/haystack-ai-openapi.yml
  type: http
slug: haystack-ai-authentication
source_filename: haystack-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/haystack-ai-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: API key generated in the deepset AI Platform UI, sent as a Bearer token.\n  sources:\n  - openapi/haystack-ai-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/haystack-ai/refs/heads/main/authentication/haystack-ai-authentication.yml
summary_line: http · 1 scheme
tags:
- AI
- LLM
- RAG
- Open Source
- Orchestration
---
