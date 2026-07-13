---
api_key_in: []
api_specs:
- filename: runloop-devbox-api-openapi.yml
  format: yaml
  label: Runloop Devbox API
  slug: runloop-devbox-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/runloop-ai/refs/heads/main/openapi/runloop-devbox-api-openapi.yml
- filename: runloop-blueprint-api-openapi.yml
  format: yaml
  label: Runloop Blueprint API
  slug: runloop-blueprint-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/runloop-ai/refs/heads/main/openapi/runloop-blueprint-api-openapi.yml
- filename: runloop-benchmark-api-openapi.yml
  format: yaml
  label: Runloop Benchmark API
  slug: runloop-benchmark-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/runloop-ai/refs/heads/main/openapi/runloop-benchmark-api-openapi.yml
- filename: runloop-scenario-api-openapi.yml
  format: yaml
  label: Runloop Scenario API
  slug: runloop-scenario-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/runloop-ai/refs/heads/main/openapi/runloop-scenario-api-openapi.yml
- filename: runloop-agents-api-openapi.yml
  format: yaml
  label: Runloop Agents API
  slug: runloop-agents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/runloop-ai/refs/heads/main/openapi/runloop-agents-api-openapi.yml
- filename: runloop-axons-api-openapi.yml
  format: yaml
  label: Runloop Axons API
  slug: runloop-axons-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/runloop-ai/refs/heads/main/openapi/runloop-axons-api-openapi.yml
- filename: runloop-objects-api-openapi.yml
  format: yaml
  label: Runloop Storage Objects API
  slug: runloop-objects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/runloop-ai/refs/heads/main/openapi/runloop-objects-api-openapi.yml
- filename: runloop-secrets-api-openapi.yml
  format: yaml
  label: Runloop Secrets API
  slug: runloop-secrets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/runloop-ai/refs/heads/main/openapi/runloop-secrets-api-openapi.yml
- filename: runloop-network-policies-api-openapi.yml
  format: yaml
  label: Runloop Network Policies API
  slug: runloop-network-policies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/runloop-ai/refs/heads/main/openapi/runloop-network-policies-api-openapi.yml
- filename: runloop-gateway-configs-api-openapi.yml
  format: yaml
  label: Runloop Gateway Configs API
  slug: runloop-gateway-configs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/runloop-ai/refs/heads/main/openapi/runloop-gateway-configs-api-openapi.yml
- filename: runloop-mcp-configs-api-openapi.yml
  format: yaml
  label: Runloop MCP Configs API
  slug: runloop-mcp-configs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/runloop-ai/refs/heads/main/openapi/runloop-mcp-configs-api-openapi.yml
- filename: runloop-apikeys-api-openapi.yml
  format: yaml
  label: Runloop API Keys API
  slug: runloop-apikeys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/runloop-ai/refs/heads/main/openapi/runloop-apikeys-api-openapi.yml
- filename: runloop-executions-api-openapi.yml
  format: yaml
  label: Runloop Executions Streaming API
  slug: runloop-executions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/runloop-ai/refs/heads/main/openapi/runloop-executions-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Runloop Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Runloop secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Runloop
provider_slug: runloop-ai
scheme_count: 1
schemes:
- name: bearerAuth
  scheme: bearer
  sources:
  - openapi/runloop-agents-api-openapi.yml
  - openapi/runloop-api-openapi.yml
  - openapi/runloop-apikeys-api-openapi.yml
  - openapi/runloop-axons-api-openapi.yml
  - openapi/runloop-benchmark-api-openapi.yml
  - openapi/runloop-blueprint-api-openapi.yml
  - openapi/runloop-devbox-api-openapi.yml
  - openapi/runloop-executions-api-openapi.yml
  - openapi/runloop-gateway-configs-api-openapi.yml
  - openapi/runloop-mcp-configs-api-openapi.yml
  - openapi/runloop-network-policies-api-openapi.yml
  - openapi/runloop-objects-api-openapi.yml
  - openapi/runloop-scenario-api-openapi.yml
  - openapi/runloop-secrets-api-openapi.yml
  type: http
slug: runloop-ai-authentication
source_filename: runloop-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/runloop-agents-api-openapi.yml, openapi/runloop-api-openapi.yml, openapi/runloop-apikeys-api-openapi.yml,\n  openapi/runloop-axons-api-openapi.yml, openapi/runloop-benchmark-api-openapi.yml, openapi/runloop-blueprint-api-openapi.yml,\n  openapi/runloop-devbox-api-openapi.yml, openapi/runloop-executions-api-openapi.yml, openapi/runloop-gateway-configs-api-openapi.yml,\n  openapi/runloop-mcp-configs-api-openapi.yml, openapi/runloop-network-policies-api-openapi.yml,\n  openapi/runloop-objects-api-openapi.yml ...\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/runloop-agents-api-openapi.yml\n  - openapi/runloop-api-openapi.yml\n  - openapi/runloop-apikeys-api-openapi.yml\n  - openapi/runloop-axons-api-openapi.yml\n  - openapi/runloop-benchmark-api-openapi.yml\n  - openapi/runloop-blueprint-api-openapi.yml\n  - openapi/runloop-devbox-api-openapi.yml\n  -\
  \ openapi/runloop-executions-api-openapi.yml\n  - openapi/runloop-gateway-configs-api-openapi.yml\n  - openapi/runloop-mcp-configs-api-openapi.yml\n  - openapi/runloop-network-policies-api-openapi.yml\n  - openapi/runloop-objects-api-openapi.yml\n  - openapi/runloop-scenario-api-openapi.yml\n  - openapi/runloop-secrets-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/runloop-ai/refs/heads/main/authentication/runloop-ai-authentication.yml
summary_line: http · 1 scheme
tags:
- AI
- AI Agents
- Coding Agents
- Sandboxes
- Devboxes
- Code Execution
- Evaluation
- Benchmarks
- SWE-Bench
- MCP
- Snapshots
- microVM
- Enterprise
- SOC 2
---
