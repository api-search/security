---
api_key_in:
- header
api_specs:
- filename: langgraph-openapi.json
  format: json
  label: LangSmith Deployment Control Plane API
  slug: control-plane
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/langgraph/refs/heads/main/openapi/langgraph-openapi.json
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
