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
- oauth2
description: Buildkite authenticates every API with Bearer-style tokens. The REST and GraphQL APIs use a user/organization API access token carrying granular scopes; the Agent API uses per-cluster Agent Tokens. A JWT public-key-pair signing method for the REST API is in preview. The remote MCP server additionally supports OAuth. Scope surface is captured in scopes/buildkite-com-scopes.yml.
kind: authentication
layout: security
method: searched
name: Buildkite Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: Buildkite secures its APIs with http and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Buildkite
provider_slug: buildkite-com
scheme_count: 3
schemes:
- applies_to:
  - REST API
  - GraphQL API
  bearerFormat: API access token
  header: 'Authorization: Bearer <token>'
  name: bearerAuth
  note: Token scopes gate access (read_builds, write_pipelines, ...); GraphQL access is a separate boolean toggle. A JWT public-key signature method is in preview.
  scheme: bearer
  scoped: true
  sources:
  - openapi/buildkite-rest-api-openapi.yml
  type: http
- applies_to:
  - Agent API
  bearerFormat: Agent Token (sent as `Token <value>`)
  header: 'Authorization: Token <value>'
  name: agentToken
  note: Issued per cluster; used by the Buildkite Agent to register and run jobs.
  scheme: bearer
  sources:
  - openapi/buildkite-agent-api-openapi.yml
  type: http
- applies_to:
  - Remote MCP Server
  name: oauth
  note: The hosted MCP server (mcp.buildkite.com/mcp) uses OAuth with short-lived (12h) access tokens; the /direct endpoint accepts API-token pass-through instead.
  type: oauth2
slug: buildkite-com-authentication
source_filename: buildkite-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-06-20'\nmethod: searched\nsource: openapi/buildkite-rest-api-openapi.yml, openapi/buildkite-agent-api-openapi.yml\ndocs: https://buildkite.com/docs/apis/managing-api-tokens\ndescription: >-\n  Buildkite authenticates every API with Bearer-style tokens. The REST and GraphQL\n  APIs use a user/organization API access token carrying granular scopes; the Agent\n  API uses per-cluster Agent Tokens. A JWT public-key-pair signing method for the REST\n  API is in preview. The remote MCP server additionally supports OAuth. Scope surface\n  is captured in scopes/buildkite-com-scopes.yml.\nsummary:\n  types:\n  - http\n  - oauth2\n  http_schemes:\n  - bearer\n  scoped: true\n  scopes: scopes/buildkite-com-scopes.yml\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: API access token\n  applies_to: [REST API, GraphQL API]\n  header: \"Authorization: Bearer <token>\"\n  scoped: true\n  note: >-\n    Token scopes gate access (read_builds, write_pipelines,\
  \ ...); GraphQL access is a\n    separate boolean toggle. A JWT public-key signature method is in preview.\n  sources:\n  - openapi/buildkite-rest-api-openapi.yml\n- name: agentToken\n  type: http\n  scheme: bearer\n  bearerFormat: Agent Token (sent as `Token <value>`)\n  applies_to: [Agent API]\n  header: \"Authorization: Token <value>\"\n  note: Issued per cluster; used by the Buildkite Agent to register and run jobs.\n  sources:\n  - openapi/buildkite-agent-api-openapi.yml\n- name: oauth\n  type: oauth2\n  applies_to: [Remote MCP Server]\n  note: >-\n    The hosted MCP server (mcp.buildkite.com/mcp) uses OAuth with short-lived (12h)\n    access tokens; the /direct endpoint accepts API-token pass-through instead.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/buildkite-com/refs/heads/main/authentication/buildkite-com-authentication.yml
summary_line: http/oauth2 · 3 schemes
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
