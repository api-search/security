---
api_key_in:
- header
api_specs:
- filename: julep-agents-api-openapi.yml
  format: yaml
  label: Julep Agents API
  slug: julep-agents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/julep/refs/heads/main/openapi/julep-agents-api-openapi.yml
- filename: julep-docs-api-openapi.yml
  format: yaml
  label: Julep Docs API
  slug: julep-docs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/julep/refs/heads/main/openapi/julep-docs-api-openapi.yml
- filename: julep-embed-api-openapi.yml
  format: yaml
  label: Julep Embed API
  slug: julep-embed-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/julep/refs/heads/main/openapi/julep-embed-api-openapi.yml
- filename: julep-executions-api-openapi.yml
  format: yaml
  label: Julep Executions API
  slug: julep-executions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/julep/refs/heads/main/openapi/julep-executions-api-openapi.yml
- filename: julep-files-api-openapi.yml
  format: yaml
  label: Julep Files API
  slug: julep-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/julep/refs/heads/main/openapi/julep-files-api-openapi.yml
- filename: julep-jobs-api-openapi.yml
  format: yaml
  label: Julep Jobs API
  slug: julep-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/julep/refs/heads/main/openapi/julep-jobs-api-openapi.yml
- filename: julep-projects-api-openapi.yml
  format: yaml
  label: Julep Projects API
  slug: julep-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/julep/refs/heads/main/openapi/julep-projects-api-openapi.yml
- filename: julep-responses-api-openapi.yml
  format: yaml
  label: Julep Responses API
  slug: julep-responses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/julep/refs/heads/main/openapi/julep-responses-api-openapi.yml
- filename: julep-secrets-api-openapi.yml
  format: yaml
  label: Julep Secrets API
  slug: julep-secrets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/julep/refs/heads/main/openapi/julep-secrets-api-openapi.yml
- filename: julep-sessions-api-openapi.yml
  format: yaml
  label: Julep Sessions API
  slug: julep-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/julep/refs/heads/main/openapi/julep-sessions-api-openapi.yml
- filename: julep-tasks-api-openapi.yml
  format: yaml
  label: Julep Tasks API
  slug: julep-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/julep/refs/heads/main/openapi/julep-tasks-api-openapi.yml
- filename: julep-users-api-openapi.yml
  format: yaml
  label: Julep Users API
  slug: julep-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/julep/refs/heads/main/openapi/julep-users-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Julep Authentication
name_suffix: Authentication
oauth_flows: []
overview: Julep secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Julep
provider_slug: julep
scheme_count: 2
schemes:
- in: header
  name: ApiKeyAuth
  parameter: Authorization
  sources:
  - openapi/julep-openapi-original.yml
  type: apiKey
- in: header
  name: ApiKeyAuth_
  parameter: X-Auth-Key
  sources:
  - openapi/julep-openapi-original.yml
  type: apiKey
slug: julep-authentication
source_filename: julep-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: derived\nsource: openapi/julep-openapi-original.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  sources:\n  - openapi/julep-openapi-original.yml\n- name: ApiKeyAuth_\n  type: apiKey\n  in: header\n  parameter: X-Auth-Key\n  sources:\n  - openapi/julep-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/julep/refs/heads/main/authentication/julep-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Company
- AI Agents
- LLM
- Agents
- Workflows
- RAG
- Memory
- Orchestration
- Developer Tools
- Open-Source
---
