---
api_key_in: []
api_specs:
- filename: langbase-openapi.yml
  format: yaml
  label: Langbase Pipes API
  slug: langbase-pipes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/langbase/refs/heads/main/openapi/langbase-openapi.yml
- filename: langbase-openapi.yml
  format: yaml
  label: Langbase Agent API
  slug: langbase-agent-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/langbase/refs/heads/main/openapi/langbase-openapi.yml
- filename: langbase-openapi.yml
  format: yaml
  label: Langbase Memory API
  slug: langbase-memory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/langbase/refs/heads/main/openapi/langbase-openapi.yml
- filename: langbase-openapi.yml
  format: yaml
  label: Langbase Threads API
  slug: langbase-threads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/langbase/refs/heads/main/openapi/langbase-openapi.yml
- filename: langbase-openapi.yml
  format: yaml
  label: Langbase Tools API
  slug: langbase-tools-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/langbase/refs/heads/main/openapi/langbase-openapi.yml
- filename: langbase-openapi.yml
  format: yaml
  label: Langbase Parser API
  slug: langbase-parser-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/langbase/refs/heads/main/openapi/langbase-openapi.yml
- filename: langbase-openapi.yml
  format: yaml
  label: Langbase Chunker API
  slug: langbase-chunker-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/langbase/refs/heads/main/openapi/langbase-openapi.yml
- filename: langbase-openapi.yml
  format: yaml
  label: Langbase Embed API
  slug: langbase-embed-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/langbase/refs/heads/main/openapi/langbase-openapi.yml
- filename: langbase-openapi.yml
  format: yaml
  label: Langbase Workflows API
  slug: langbase-workflows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/langbase/refs/heads/main/openapi/langbase-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Langbase Authentication
name_suffix: Authentication
oauth_flows: []
overview: Langbase secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Langbase
provider_slug: langbase
scheme_count: 1
schemes:
- bearerFormat: apiKey
  name: api_key
  scheme: bearer
  sources:
  - openapi/langbase-openapi.yml
  type: http
slug: langbase-authentication
source_filename: langbase-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/langbase-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: api_key\n  type: http\n  scheme: bearer\n  bearerFormat: apiKey\n  sources:\n  - openapi/langbase-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/langbase/refs/heads/main/authentication/langbase-authentication.yml
summary_line: http · 1 scheme
tags:
- AI
- Agents
- RAG
- LLM
- Serverless
---
