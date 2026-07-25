---
api_key_in: []
api_specs:
- filename: toolhouse-agent-runs-api-openapi.yml
  format: yaml
  label: Toolhouse Agent Runs API
  slug: toolhouse-agent-runs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toolhouse/refs/heads/main/openapi/toolhouse-agent-runs-api-openapi.yml
- filename: toolhouse-api-keys-api-openapi.yml
  format: yaml
  label: Toolhouse API Keys API
  slug: toolhouse-api-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toolhouse/refs/heads/main/openapi/toolhouse-api-keys-api-openapi.yml
- filename: toolhouse-backoffice-api-openapi.yml
  format: yaml
  label: Toolhouse Backoffice API
  slug: toolhouse-backoffice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toolhouse/refs/heads/main/openapi/toolhouse-backoffice-api-openapi.yml
- filename: toolhouse-logs-api-openapi.yml
  format: yaml
  label: Toolhouse Logs API
  slug: toolhouse-logs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toolhouse/refs/heads/main/openapi/toolhouse-logs-api-openapi.yml
- filename: toolhouse-metrics-api-openapi.yml
  format: yaml
  label: Toolhouse Metrics API
  slug: toolhouse-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toolhouse/refs/heads/main/openapi/toolhouse-metrics-api-openapi.yml
- filename: toolhouse-sdk-api-api-openapi.yml
  format: yaml
  label: Toolhouse SDK API API
  slug: toolhouse-sdk-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toolhouse/refs/heads/main/openapi/toolhouse-sdk-api-api-openapi.yml
- filename: toolhouse-user-api-api-openapi.yml
  format: yaml
  label: Toolhouse User API API
  slug: toolhouse-user-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toolhouse/refs/heads/main/openapi/toolhouse-user-api-api-openapi.yml
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
