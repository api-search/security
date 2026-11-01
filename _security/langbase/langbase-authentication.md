---
anonymous_access: false
api_key_in: []
api_specs:
- filename: langbase-agent-api-openapi.yml
  format: yaml
  label: Langbase Agent API
  slug: langbase-agent-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/langbase/openapi/langbase-agent-api-openapi.yml
- filename: langbase-chunker-api-openapi.yml
  format: yaml
  label: Langbase Chunker API
  slug: langbase-chunker-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/langbase/openapi/langbase-chunker-api-openapi.yml
- filename: langbase-embed-api-openapi.yml
  format: yaml
  label: Langbase Embed API
  slug: langbase-embed-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/langbase/openapi/langbase-embed-api-openapi.yml
- filename: langbase-memory-api-openapi.yml
  format: yaml
  label: Langbase Memory API
  slug: langbase-memory-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/langbase/openapi/langbase-memory-api-openapi.yml
- filename: langbase-parser-api-openapi.yml
  format: yaml
  label: Langbase Parser API
  slug: langbase-parser-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/langbase/openapi/langbase-parser-api-openapi.yml
- filename: langbase-pipes-api-openapi.yml
  format: yaml
  label: Langbase Pipes API
  slug: langbase-pipes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/langbase/openapi/langbase-pipes-api-openapi.yml
- filename: langbase-threads-api-openapi.yml
  format: yaml
  label: Langbase Threads API
  slug: langbase-threads-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/langbase/openapi/langbase-threads-api-openapi.yml
- filename: langbase-tools-api-openapi.yml
  format: yaml
  label: Langbase Tools API
  slug: langbase-tools-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/langbase/openapi/langbase-tools-api-openapi.yml
- filename: langbase-beta-api-openapi.yml
  format: yaml
  label: Langbase Beta API
  slug: langbase-beta-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/langbase/openapi/langbase-beta-api-openapi.yml
- filename: langbase-health-api-openapi.yml
  format: yaml
  label: Langbase Health API
  slug: langbase-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/langbase/openapi/langbase-health-api-openapi.yml
- filename: langbase-images-api-openapi.yml
  format: yaml
  label: Langbase Images API
  slug: langbase-images-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/langbase/openapi/langbase-images-api-openapi.yml
- filename: langbase-langbase-api-api-openapi.yml
  format: yaml
  label: Langbase Langbase API
  slug: langbase-langbase-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/langbase/openapi/langbase-langbase-api-api-openapi.yml
- filename: langbase-models-api-openapi.yml
  format: yaml
  label: Langbase Models API
  slug: langbase-models-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/langbase/openapi/langbase-models-api-openapi.yml
- filename: langbase-routes-api-openapi.yml
  format: yaml
  label: Langbase Routes API
  slug: langbase-routes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/langbase/openapi/langbase-routes-api-openapi.yml
- filename: langbase-traces-api-openapi.yml
  format: yaml
  label: Langbase Traces API
  slug: langbase-traces-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/langbase/openapi/langbase-traces-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
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
source_yaml_url: https://artifacts.apis.io/langbase/authentication/langbase-authentication.yml
summary_line: http · 1 scheme
tags:
- Artificial Intelligence
- Agents
- RAG
- LLM
- Serverless
---
