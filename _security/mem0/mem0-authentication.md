---
api_key_in:
- header
api_specs:
- filename: mem0-agents-api-openapi.yml
  format: yaml
  label: Mem0 agents API
  slug: mem0-agents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mem0/refs/heads/main/openapi/mem0-agents-api-openapi.yml
- filename: mem0-apps-api-openapi.yml
  format: yaml
  label: Mem0 apps API
  slug: mem0-apps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mem0/refs/heads/main/openapi/mem0-apps-api-openapi.yml
- filename: mem0-entities-api-openapi.yml
  format: yaml
  label: Mem0 entities API
  slug: mem0-entities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mem0/refs/heads/main/openapi/mem0-entities-api-openapi.yml
- filename: mem0-events-api-openapi.yml
  format: yaml
  label: Mem0 events API
  slug: mem0-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mem0/refs/heads/main/openapi/mem0-events-api-openapi.yml
- filename: mem0-exports-api-openapi.yml
  format: yaml
  label: Mem0 exports API
  slug: mem0-exports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mem0/refs/heads/main/openapi/mem0-exports-api-openapi.yml
- filename: mem0-feedback-api-openapi.yml
  format: yaml
  label: Mem0 feedback API
  slug: mem0-feedback-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mem0/refs/heads/main/openapi/mem0-feedback-api-openapi.yml
- filename: mem0-memories-api-openapi.yml
  format: yaml
  label: Mem0 memories API
  slug: mem0-memories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mem0/refs/heads/main/openapi/mem0-memories-api-openapi.yml
- filename: mem0-organizations-api-openapi.yml
  format: yaml
  label: Mem0 organizations API
  slug: mem0-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mem0/refs/heads/main/openapi/mem0-organizations-api-openapi.yml
- filename: mem0-project-api-openapi.yml
  format: yaml
  label: Mem0 Project API
  slug: mem0-project-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mem0/refs/heads/main/openapi/mem0-project-api-openapi.yml
- filename: mem0-projects-api-openapi.yml
  format: yaml
  label: Mem0 projects API
  slug: mem0-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mem0/refs/heads/main/openapi/mem0-projects-api-openapi.yml
- filename: mem0-runs-api-openapi.yml
  format: yaml
  label: Mem0 runs API
  slug: mem0-runs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mem0/refs/heads/main/openapi/mem0-runs-api-openapi.yml
- filename: mem0-stats-api-openapi.yml
  format: yaml
  label: Mem0 stats API
  slug: mem0-stats-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mem0/refs/heads/main/openapi/mem0-stats-api-openapi.yml
- filename: mem0-users-api-openapi.yml
  format: yaml
  label: Mem0 users API
  slug: mem0-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mem0/refs/heads/main/openapi/mem0-users-api-openapi.yml
- filename: mem0-webhooks-api-openapi.yml
  format: yaml
  label: Mem0 webhooks API
  slug: mem0-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mem0/refs/heads/main/openapi/mem0-webhooks-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Mem0 Authentication
name_suffix: Authentication
oauth_flows: []
overview: Mem0 secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Mem0
provider_slug: mem0
scheme_count: 1
schemes:
- description: 'API key authentication. Prefix your Mem0 API key with ''Token ''. Example: ''Token your_api_key'''
  in: header
  name: ApiKeyAuth
  parameter: Authorization
  sources:
  - openapi/mem0-openapi.json
  type: apiKey
slug: mem0-authentication
source_filename: mem0-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/mem0-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: 'API key authentication. Prefix your Mem0 API key with ''Token ''. Example: ''Token\n    your_api_key'''\n  sources:\n  - openapi/mem0-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mem0/refs/heads/main/authentication/mem0-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Memory
- AI Agents
- Agent Memory
- Context
- LLMs
- Retrieval
- Vectors
- LangChain
- CrewAI
- AutoGen
- LlamaIndex
- Open-Source
- Infrastructure
---
