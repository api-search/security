---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: airia-openapi.yml
  format: yaml
  label: Airia Web APIs
  slug: airia-web-apis
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airia/refs/heads/main/openapi/airia-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Airia Authentication
name_suffix: Authentication
oauth_flows: []
overview: Airia secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Airia
provider_slug: airia
scheme_count: 2
schemes:
- description: API Key Authentication
  in: header
  name: ApiKey
  parameter: X-API-Key
  sources:
  - openapi/airia-openapi.yml
  type: apiKey
- description: Cookie based Authentication
  in: header
  name: Cookies
  parameter: Cookie
  sources:
  - openapi/airia-openapi.yml
  type: apiKey
slug: airia-authentication
source_filename: airia-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: derived\nsource: openapi/airia-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKey\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: API Key Authentication\n  sources:\n  - openapi/airia-openapi.yml\n- name: Cookies\n  type: apiKey\n  in: header\n  parameter: Cookie\n  description: Cookie based Authentication\n  sources:\n  - openapi/airia-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/airia/refs/heads/main/authentication/airia-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Company
- Enterprise AI
- AI Agents
- AI Governance
- AI Security
- MCP
- MCP Gateway
- Agent Orchestration
- LLM Gateway
- AI Discovery
- Red Teaming
- Guardrails
- Knowledge Retrieval
- RAG
- Agent-Native
---
