---
api_key_in:
- header
api_specs:
- filename: langsmith-openapi.json
  format: json
  label: LangSmith Tracing API
  slug: langsmith-tracing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/langsmith/refs/heads/main/openapi/langsmith-openapi.json
- filename: langsmith-openapi.json
  format: json
  label: LangSmith Datasets API
  slug: langsmith-datasets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/langsmith/refs/heads/main/openapi/langsmith-openapi.json
- filename: langsmith-openapi.json
  format: json
  label: LangSmith Evaluations API
  slug: langsmith-evaluations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/langsmith/refs/heads/main/openapi/langsmith-openapi.json
- filename: langsmith-openapi.json
  format: json
  label: LangSmith Prompt Hub API
  slug: langsmith-prompts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/langsmith/refs/heads/main/openapi/langsmith-openapi.json
- filename: langsmith-openapi.json
  format: json
  label: LangSmith Feedback API
  slug: langsmith-feedback-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/langsmith/refs/heads/main/openapi/langsmith-openapi.json
- filename: langsmith-openapi.json
  format: json
  label: LangSmith Annotation Queues API
  slug: langsmith-annotation-queues-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/langsmith/refs/heads/main/openapi/langsmith-openapi.json
- filename: langsmith-openapi.json
  format: json
  label: LangSmith Fleet (Agent Deployment) API
  slug: langsmith-fleet-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/langsmith/refs/heads/main/openapi/langsmith-openapi.json
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Langsmith Authentication
name_suffix: Authentication
oauth_flows: []
overview: LangSmith secures its APIs with apiKey and http across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: LangSmith
provider_slug: langsmith
scheme_count: 4
schemes:
- in: header
  name: API Key
  parameter: X-API-Key
  sources:
  - openapi/langsmith-openapi.json
  type: apiKey
- in: header
  name: Tenant ID
  parameter: X-Tenant-Id
  sources:
  - openapi/langsmith-openapi.json
  type: apiKey
- description: Bearer tokens are used to authenticate from the UI. Must also specify x-tenant-id or x-organization-id (for org scoped apis).
  name: Bearer Auth
  scheme: bearer
  sources:
  - openapi/langsmith-openapi.json
  type: http
- in: header
  name: Organization ID
  parameter: X-Organization-Id
  sources:
  - openapi/langsmith-openapi.json
  type: apiKey
slug: langsmith-authentication
source_filename: langsmith-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/langsmith-openapi.json\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: API Key\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  sources:\n  - openapi/langsmith-openapi.json\n- name: Tenant ID\n  type: apiKey\n  in: header\n  parameter: X-Tenant-Id\n  sources:\n  - openapi/langsmith-openapi.json\n- name: Bearer Auth\n  type: http\n  scheme: bearer\n  description: Bearer tokens are used to authenticate from the UI. Must also specify x-tenant-id\n    or x-organization-id (for org scoped apis).\n  sources:\n  - openapi/langsmith-openapi.json\n- name: Organization ID\n  type: apiKey\n  in: header\n  parameter: X-Organization-Id\n  sources:\n  - openapi/langsmith-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/langsmith/refs/heads/main/authentication/langsmith-authentication.yml
summary_line: apiKey/http · 4 schemes
tags:
- AI
- LLM
- Observability
- Evaluations
- LangChain
---
