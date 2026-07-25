---
api_key_in:
- header
api_specs:
- filename: parallel-chat-api-beta-api-openapi.yml
  format: yaml
  label: Parallel Chat API (Beta) API
  slug: parallel-chat-api-beta-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/parallel/refs/heads/main/openapi/parallel-chat-api-beta-api-openapi.yml
- filename: parallel-extract-api-openapi.yml
  format: yaml
  label: Parallel Extract API
  slug: parallel-extract-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/parallel/refs/heads/main/openapi/parallel-extract-api-openapi.yml
- filename: parallel-findall-api-openapi.yml
  format: yaml
  label: Parallel FindAll API
  slug: parallel-findall-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/parallel/refs/heads/main/openapi/parallel-findall-api-openapi.yml
- filename: parallel-monitor-api-openapi.yml
  format: yaml
  label: Parallel Monitor API
  slug: parallel-monitor-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/parallel/refs/heads/main/openapi/parallel-monitor-api-openapi.yml
- filename: parallel-search-api-openapi.yml
  format: yaml
  label: Parallel Search API
  slug: parallel-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/parallel/refs/heads/main/openapi/parallel-search-api-openapi.yml
- filename: parallel-tasks-api-openapi.yml
  format: yaml
  label: Parallel Tasks API
  slug: parallel-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/parallel/refs/heads/main/openapi/parallel-tasks-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Parallel Authentication
name_suffix: Authentication
oauth_flows: []
overview: Parallel secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Parallel
provider_slug: parallel
scheme_count: 1
schemes:
- in: header
  name: ApiKeyAuth
  parameter: x-api-key
  sources:
  - openapi/parallel-openapi-original.json
  type: apiKey
slug: parallel-authentication
source_filename: parallel-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: derived\nsource: openapi/parallel-openapi-original.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  sources:\n  - openapi/parallel-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/parallel/refs/heads/main/authentication/parallel-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Ai
- Web Search
- Agents
- Deep Research
- Web Extraction
- Data Enrichment
- Web Monitoring
- LLM Tools
---
