---
api_key_in: []
api_specs:
- filename: toolhouse-openapi-original.yml
  format: yaml
  label: Toolhouse Platform API
  slug: platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toolhouse/refs/heads/main/openapi/toolhouse-openapi-original.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Toolhouse Authentication
name_suffix: Authentication
oauth_flows: []
overview: Toolhouse secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Toolhouse
provider_slug: toolhouse
scheme_count: 1
schemes:
- name: HTTPBearer
  scheme: bearer
  sources:
  - openapi/toolhouse-openapi-original.yml
  type: http
slug: toolhouse-authentication
source_filename: toolhouse-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/toolhouse-openapi-original.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: HTTPBearer\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/toolhouse-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/toolhouse/refs/heads/main/authentication/toolhouse-authentication.yml
summary_line: http · 1 scheme
tags:
- Agent Infrastructure
- AI Agents
- AI Workers
- Backend as a Service
- MCP
- MCP Discovery
- RAG
- Tools
- Workers API
---
