---
anonymous_access: false
api_key_in: []
api_specs:
- filename: haystack-ai-files-api-openapi.yml
  format: yaml
  label: Haystack / deepset Files API
  slug: haystack-ai-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/haystack-ai/refs/heads/main/openapi/haystack-ai-files-api-openapi.yml
- filename: haystack-ai-pipelines-api-openapi.yml
  format: yaml
  label: Haystack / deepset Pipelines API
  slug: haystack-ai-pipelines-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/haystack-ai/refs/heads/main/openapi/haystack-ai-pipelines-api-openapi.yml
- filename: haystack-ai-search-api-openapi.yml
  format: yaml
  label: Haystack / deepset Search API
  slug: haystack-ai-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/haystack-ai/refs/heads/main/openapi/haystack-ai-search-api-openapi.yml
- filename: haystack-ai-workspaces-api-openapi.yml
  format: yaml
  label: Haystack / deepset Workspaces API
  slug: haystack-ai-workspaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/haystack-ai/refs/heads/main/openapi/haystack-ai-workspaces-api-openapi.yml
- filename: haystack-ai-config-api-openapi.yml
  format: yaml
  label: Haystack / deepset Config API
  slug: haystack-ai-config-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/haystack-ai/refs/heads/main/openapi/haystack-ai-config-api-openapi.yml
- filename: haystack-ai-dashboard-api-openapi.yml
  format: yaml
  label: Haystack / deepset Dashboard API
  slug: haystack-ai-dashboard-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/haystack-ai/refs/heads/main/openapi/haystack-ai-dashboard-api-openapi.yml
- filename: haystack-ai-openai-api-openapi.yml
  format: yaml
  label: Haystack / deepset Openai API
  slug: haystack-ai-openai-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/haystack-ai/refs/heads/main/openapi/haystack-ai-openai-api-openapi.yml
- filename: haystack-ai-status-api-openapi.yml
  format: yaml
  label: Haystack / deepset Status API
  slug: haystack-ai-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/haystack-ai/refs/heads/main/openapi/haystack-ai-status-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
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
- Artificial Intelligence
- LLM
- RAG
- Open Source
- Orchestration
---
