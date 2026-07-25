---
api_key_in:
- header
api_specs:
- filename: langgraph-agent-connections-v2-api-openapi.yml
  format: yaml
  label: LangGraph Agent Connections (v2) API
  slug: langgraph-agent-connections-v2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/langgraph/refs/heads/main/openapi/langgraph-agent-connections-v2-api-openapi.yml
- filename: langgraph-auth-service-v2-api-openapi.yml
  format: yaml
  label: LangGraph Auth Service (v2) API
  slug: langgraph-auth-service-v2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/langgraph/refs/heads/main/openapi/langgraph-auth-service-v2-api-openapi.yml
- filename: langgraph-deployments-v2-api-openapi.yml
  format: yaml
  label: LangGraph Deployments (v2) API
  slug: langgraph-deployments-v2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/langgraph/refs/heads/main/openapi/langgraph-deployments-v2-api-openapi.yml
- filename: langgraph-integrations-v1-api-openapi.yml
  format: yaml
  label: LangGraph Integrations (v1) API
  slug: langgraph-integrations-v1-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/langgraph/refs/heads/main/openapi/langgraph-integrations-v1-api-openapi.yml
- filename: langgraph-listeners-v2-api-openapi.yml
  format: yaml
  label: LangGraph Listeners (v2) API
  slug: langgraph-listeners-v2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/langgraph/refs/heads/main/openapi/langgraph-listeners-v2-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Langgraph Authentication
name_suffix: Authentication
oauth_flows: []
overview: LangGraph secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: LangGraph
provider_slug: langgraph
scheme_count: 1
schemes:
- in: header
  name: LangSmith API Key
  parameter: X-Api-Key
  sources:
  - openapi/langgraph-openapi.json
  type: apiKey
slug: langgraph-authentication
source_filename: langgraph-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/langgraph-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: LangSmith API Key\n  type: apiKey\n  in: header\n  parameter: X-Api-Key\n  sources:\n  - openapi/langgraph-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/langgraph/refs/heads/main/authentication/langgraph-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Agents
- Artificial Intelligence
- Large Language Models
- Workflows
- Orchestration
---
