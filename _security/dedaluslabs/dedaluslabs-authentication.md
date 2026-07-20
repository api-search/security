---
api_key_in:
- header
api_specs:
- filename: dedaluslabs-agents-openapi-original.json
  format: json
  label: Dedalus Agents API
  slug: dedalus-agents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dedaluslabs/refs/heads/main/openapi/dedaluslabs-agents-openapi-original.json
- filename: dedaluslabs-machines-openapi-original.yml
  format: yaml
  label: Dedalus Cloud Services (Machines) API
  slug: dedalus-cloud-services-machines-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dedaluslabs/refs/heads/main/openapi/dedaluslabs-machines-openapi-original.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Dedaluslabs Authentication
name_suffix: Authentication
oauth_flows: []
overview: Dedalus Labs secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Dedalus Labs
provider_slug: dedaluslabs
scheme_count: 2
schemes:
- name: Bearer
  scheme: bearer
  sources:
  - openapi/dedaluslabs-agents-openapi-original.json
  - openapi/dedaluslabs-machines-openapi-original.yml
  type: http
- description: Dedalus API key. Alternative to Bearer token.
  in: header
  name: ApiKeyAuth
  parameter: x-api-key
  sources:
  - openapi/dedaluslabs-machines-openapi-original.yml
  type: apiKey
slug: dedaluslabs-authentication
source_filename: dedaluslabs-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: derived\nsource: openapi/dedaluslabs-agents-openapi-original.json, openapi/dedaluslabs-machines-openapi-original.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: Bearer\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/dedaluslabs-agents-openapi-original.json\n  - openapi/dedaluslabs-machines-openapi-original.yml\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: Dedalus API key. Alternative to Bearer token.\n  sources:\n  - openapi/dedaluslabs-machines-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dedaluslabs/refs/heads/main/authentication/dedaluslabs-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Company
- AI
- Agents
- MCP
- Model Context Protocol
- LLM
- Inference
- Gateway
- Compute
- Sandbox
- Developer Tools
---
