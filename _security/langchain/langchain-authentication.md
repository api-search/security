---
api_key_in:
- header
api_specs:
- filename: langchain-openapi.json
  format: json
  label: LangSmith API
  slug: langsmith
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/langchain/refs/heads/main/openapi/langchain-openapi.json
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Langchain Authentication
name_suffix: Authentication
oauth_flows: []
overview: LangChain secures its APIs with apiKey and http across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: LangChain
provider_slug: langchain
scheme_count: 4
schemes:
- in: header
  name: API Key
  parameter: X-API-Key
  sources:
  - openapi/langchain-openapi.json
  type: apiKey
- in: header
  name: Tenant ID
  parameter: X-Tenant-Id
  sources:
  - openapi/langchain-openapi.json
  type: apiKey
- description: Bearer tokens are used to authenticate from the UI. Must also specify x-tenant-id or x-organization-id (for org scoped apis).
  name: Bearer Auth
  scheme: bearer
  sources:
  - openapi/langchain-openapi.json
  type: http
- in: header
  name: Organization ID
  parameter: X-Organization-Id
  sources:
  - openapi/langchain-openapi.json
  type: apiKey
slug: langchain-authentication
source_filename: langchain-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/langchain-openapi.json\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: API Key\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  sources:\n  - openapi/langchain-openapi.json\n- name: Tenant ID\n  type: apiKey\n  in: header\n  parameter: X-Tenant-Id\n  sources:\n  - openapi/langchain-openapi.json\n- name: Bearer Auth\n  type: http\n  scheme: bearer\n  description: Bearer tokens are used to authenticate from the UI. Must also specify x-tenant-id\n    or x-organization-id (for org scoped apis).\n  sources:\n  - openapi/langchain-openapi.json\n- name: Organization ID\n  type: apiKey\n  in: header\n  parameter: X-Organization-Id\n  sources:\n  - openapi/langchain-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/langchain/refs/heads/main/authentication/langchain-authentication.yml
summary_line: apiKey/http · 4 schemes
tags:
- Agents
- Artificial Intelligence
- Large Language Models
- LLM Observability
- Tracing
- Evaluation
---
