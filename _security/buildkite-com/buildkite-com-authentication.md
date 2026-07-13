---
api_key_in: []
api_specs:
- filename: buildkite-rest-api-openapi.yml
  format: yaml
  label: Buildkite REST API
  slug: buildkite-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/buildkite-com/refs/heads/main/openapi/buildkite-rest-api-openapi.yml
- filename: buildkite-agent-api-openapi.yml
  format: yaml
  label: Buildkite Agent API
  slug: buildkite-agent-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/buildkite-com/refs/heads/main/openapi/buildkite-agent-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Buildkite Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: Buildkite secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Buildkite
provider_slug: buildkite-com
scheme_count: 1
schemes:
- bearerFormat: Agent Token (sent as `Token <value>`)
  name: agentToken
  scheme: bearer
  sources:
  - openapi/buildkite-agent-api-openapi.yml
  - openapi/buildkite-rest-api-openapi.yml
  type: http
slug: buildkite-com-authentication
source_filename: buildkite-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/buildkite-agent-api-openapi.yml, openapi/buildkite-rest-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: agentToken\n  type: http\n  scheme: bearer\n  bearerFormat: Agent Token (sent as `Token <value>`)\n  sources:\n  - openapi/buildkite-agent-api-openapi.yml\n  - openapi/buildkite-rest-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/buildkite-com/refs/heads/main/authentication/buildkite-com-authentication.yml
summary_line: http · 1 scheme
tags:
- CI/CD
- Continuous Integration
- Continuous Delivery
- DevOps
- Pipelines
- Hybrid CI
- Build Automation
- Test Engine
- Package Registries
- Agents
- GraphQL
- REST
- MCP
- Webhooks
---
