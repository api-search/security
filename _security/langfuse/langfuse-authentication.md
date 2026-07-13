---
api_key_in: []
api_specs:
- filename: langfuse-openapi.yml
  format: yaml
  label: Langfuse Tracing API
  slug: langfuse-tracing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/langfuse/refs/heads/main/openapi/langfuse-openapi.yml
- filename: langfuse-openapi.yml
  format: yaml
  label: Langfuse Observations API
  slug: langfuse-observations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/langfuse/refs/heads/main/openapi/langfuse-openapi.yml
- filename: langfuse-openapi.yml
  format: yaml
  label: Langfuse Metrics API
  slug: langfuse-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/langfuse/refs/heads/main/openapi/langfuse-openapi.yml
- filename: langfuse-openapi.yml
  format: yaml
  label: Langfuse Prompt Management API
  slug: langfuse-prompts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/langfuse/refs/heads/main/openapi/langfuse-openapi.yml
- filename: langfuse-openapi.yml
  format: yaml
  label: Langfuse Datasets API
  slug: langfuse-datasets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/langfuse/refs/heads/main/openapi/langfuse-openapi.yml
- filename: langfuse-openapi.yml
  format: yaml
  label: Langfuse Evaluations API
  slug: langfuse-evaluations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/langfuse/refs/heads/main/openapi/langfuse-openapi.yml
- filename: langfuse-openapi.yml
  format: yaml
  label: Langfuse Scores API
  slug: langfuse-scores-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/langfuse/refs/heads/main/openapi/langfuse-openapi.yml
- filename: langfuse-openapi.yml
  format: yaml
  label: Langfuse Organizations & Projects API
  slug: langfuse-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/langfuse/refs/heads/main/openapi/langfuse-openapi.yml
- filename: langfuse-openapi.yml
  format: yaml
  label: Langfuse Instance Management API
  slug: langfuse-instance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/langfuse/refs/heads/main/openapi/langfuse-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Langfuse Authentication
name_suffix: Authentication
oauth_flows: []
overview: Langfuse secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Langfuse
provider_slug: langfuse
scheme_count: 1
schemes:
- name: BasicAuth
  scheme: basic
  sources:
  - openapi/langfuse-openapi.yml
  type: http
slug: langfuse-authentication
source_filename: langfuse-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/langfuse-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BasicAuth\n  type: http\n  scheme: basic\n  sources:\n  - openapi/langfuse-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/langfuse/refs/heads/main/authentication/langfuse-authentication.yml
summary_line: http · 1 scheme
tags:
- AI
- LLM
- Observability
- Open Source
- Evaluations
---
