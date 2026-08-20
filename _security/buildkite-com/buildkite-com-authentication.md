---
api_key_in: []
api_specs:
- filename: buildkite-com-access-token-api-openapi.yml
  format: yaml
  label: Buildkite Access Token API
  slug: buildkite-com-access-token-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/buildkite-com/refs/heads/main/openapi/buildkite-com-access-token-api-openapi.yml
- filename: buildkite-com-agent-tokens-api-openapi.yml
  format: yaml
  label: Buildkite Agent Tokens API
  slug: buildkite-com-agent-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/buildkite-com/refs/heads/main/openapi/buildkite-com-agent-tokens-api-openapi.yml
- filename: buildkite-com-agents-api-openapi.yml
  format: yaml
  label: Buildkite Agents API
  slug: buildkite-com-agents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/buildkite-com/refs/heads/main/openapi/buildkite-com-agents-api-openapi.yml
- filename: buildkite-com-annotations-api-openapi.yml
  format: yaml
  label: Buildkite Annotations API
  slug: buildkite-com-annotations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/buildkite-com/refs/heads/main/openapi/buildkite-com-annotations-api-openapi.yml
- filename: buildkite-com-artifacts-api-openapi.yml
  format: yaml
  label: Buildkite Artifacts API
  slug: buildkite-com-artifacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/buildkite-com/refs/heads/main/openapi/buildkite-com-artifacts-api-openapi.yml
- filename: buildkite-com-builds-api-openapi.yml
  format: yaml
  label: Buildkite Builds API
  slug: buildkite-com-builds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/buildkite-com/refs/heads/main/openapi/buildkite-com-builds-api-openapi.yml
- filename: buildkite-com-clusters-api-openapi.yml
  format: yaml
  label: Buildkite Clusters API
  slug: buildkite-com-clusters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/buildkite-com/refs/heads/main/openapi/buildkite-com-clusters-api-openapi.yml
- filename: buildkite-com-emojis-api-openapi.yml
  format: yaml
  label: Buildkite Emojis API
  slug: buildkite-com-emojis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/buildkite-com/refs/heads/main/openapi/buildkite-com-emojis-api-openapi.yml
- filename: buildkite-com-jobs-api-openapi.yml
  format: yaml
  label: Buildkite Jobs API
  slug: buildkite-com-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/buildkite-com/refs/heads/main/openapi/buildkite-com-jobs-api-openapi.yml
- filename: buildkite-com-meta-api-openapi.yml
  format: yaml
  label: Buildkite Meta API
  slug: buildkite-com-meta-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/buildkite-com/refs/heads/main/openapi/buildkite-com-meta-api-openapi.yml
- filename: buildkite-com-metrics-api-openapi.yml
  format: yaml
  label: Buildkite Metrics API
  slug: buildkite-com-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/buildkite-com/refs/heads/main/openapi/buildkite-com-metrics-api-openapi.yml
- filename: buildkite-com-organizations-api-openapi.yml
  format: yaml
  label: Buildkite Organizations API
  slug: buildkite-com-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/buildkite-com/refs/heads/main/openapi/buildkite-com-organizations-api-openapi.yml
- filename: buildkite-com-pipeline-templates-api-openapi.yml
  format: yaml
  label: Buildkite Pipeline Templates API
  slug: buildkite-com-pipeline-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/buildkite-com/refs/heads/main/openapi/buildkite-com-pipeline-templates-api-openapi.yml
- filename: buildkite-com-pipelines-api-openapi.yml
  format: yaml
  label: Buildkite Pipelines API
  slug: buildkite-com-pipelines-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/buildkite-com/refs/heads/main/openapi/buildkite-com-pipelines-api-openapi.yml
- filename: buildkite-com-queues-api-openapi.yml
  format: yaml
  label: Buildkite Queues API
  slug: buildkite-com-queues-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/buildkite-com/refs/heads/main/openapi/buildkite-com-queues-api-openapi.yml
- filename: buildkite-com-rules-api-openapi.yml
  format: yaml
  label: Buildkite Rules API
  slug: buildkite-com-rules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/buildkite-com/refs/heads/main/openapi/buildkite-com-rules-api-openapi.yml
- filename: buildkite-com-stacks-api-openapi.yml
  format: yaml
  label: Buildkite Stacks API
  slug: buildkite-com-stacks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/buildkite-com/refs/heads/main/openapi/buildkite-com-stacks-api-openapi.yml
- filename: buildkite-com-teams-api-openapi.yml
  format: yaml
  label: Buildkite Teams API
  slug: buildkite-com-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/buildkite-com/refs/heads/main/openapi/buildkite-com-teams-api-openapi.yml
- filename: buildkite-com-user-api-openapi.yml
  format: yaml
  label: Buildkite User API
  slug: buildkite-com-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/buildkite-com/refs/heads/main/openapi/buildkite-com-user-api-openapi.yml
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
- Webhook
---
