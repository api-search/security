---
api_key_in: []
api_specs:
- filename: letta-openapi.json
  format: json
  label: Letta Cloud API
  slug: cloud
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/letta/refs/heads/main/openapi/letta-openapi.json
- filename: letta-openapi.json
  format: json
  label: Letta Self-Hosted Server
  slug: self-hosted
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/letta/refs/heads/main/openapi/letta-openapi.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Letta Authentication
name_suffix: Authentication
oauth_flows: []
overview: Letta secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Letta
provider_slug: letta
scheme_count: 1
schemes:
- name: bearerAuth
  scheme: bearer
  sources:
  - openapi/letta-openapi.json
  - openapi/letta-openapi.yml
  type: http
slug: letta-authentication
source_filename: letta-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/letta-openapi.json, openapi/letta-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/letta-openapi.json\n  - openapi/letta-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/letta/refs/heads/main/authentication/letta-authentication.yml
summary_line: http · 1 scheme
tags:
- AI
- Agents
- Stateful Agents
- Memory
- MemGPT
- Continual Learning
- MCP
- Multi-Agent
- RAG
- Open Source
---
