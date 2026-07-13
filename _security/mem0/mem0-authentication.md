---
api_key_in:
- header
api_specs:
- filename: mem0-openapi.json
  format: json
  label: Mem0 Platform API
  slug: platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mem0/refs/heads/main/openapi/mem0-openapi.json
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
- Vector
- LangChain
- CrewAI
- AutoGen
- LlamaIndex
- Open Source
- Infrastructure
---
