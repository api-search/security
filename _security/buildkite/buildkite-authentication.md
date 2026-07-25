---
api_key_in: []
api_specs:
- filename: buildkite-accesstoken-api-openapi.yml
  format: yaml
  label: Buildkite AccessToken API
  slug: buildkite-accesstoken-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/buildkite/refs/heads/main/openapi/buildkite-accesstoken-api-openapi.yml
- filename: buildkite-agents-api-openapi.yml
  format: yaml
  label: Buildkite Agents API
  slug: buildkite-agents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/buildkite/refs/heads/main/openapi/buildkite-agents-api-openapi.yml
- filename: buildkite-agenttokens-api-openapi.yml
  format: yaml
  label: Buildkite AgentTokens API
  slug: buildkite-agenttokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/buildkite/refs/heads/main/openapi/buildkite-agenttokens-api-openapi.yml
- filename: buildkite-annotations-api-openapi.yml
  format: yaml
  label: Buildkite Annotations API
  slug: buildkite-annotations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/buildkite/refs/heads/main/openapi/buildkite-annotations-api-openapi.yml
- filename: buildkite-artifacts-api-openapi.yml
  format: yaml
  label: Buildkite Artifacts API
  slug: buildkite-artifacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/buildkite/refs/heads/main/openapi/buildkite-artifacts-api-openapi.yml
- filename: buildkite-builds-api-openapi.yml
  format: yaml
  label: Buildkite Builds API
  slug: buildkite-builds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/buildkite/refs/heads/main/openapi/buildkite-builds-api-openapi.yml
- filename: buildkite-clusters-api-openapi.yml
  format: yaml
  label: Buildkite Clusters API
  slug: buildkite-clusters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/buildkite/refs/heads/main/openapi/buildkite-clusters-api-openapi.yml
- filename: buildkite-emojis-api-openapi.yml
  format: yaml
  label: Buildkite Emojis API
  slug: buildkite-emojis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/buildkite/refs/heads/main/openapi/buildkite-emojis-api-openapi.yml
- filename: buildkite-jobs-api-openapi.yml
  format: yaml
  label: Buildkite Jobs API
  slug: buildkite-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/buildkite/refs/heads/main/openapi/buildkite-jobs-api-openapi.yml
- filename: buildkite-meta-api-openapi.yml
  format: yaml
  label: Buildkite Meta API
  slug: buildkite-meta-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/buildkite/refs/heads/main/openapi/buildkite-meta-api-openapi.yml
- filename: buildkite-organizations-api-openapi.yml
  format: yaml
  label: Buildkite Organizations API
  slug: buildkite-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/buildkite/refs/heads/main/openapi/buildkite-organizations-api-openapi.yml
- filename: buildkite-pipelines-api-openapi.yml
  format: yaml
  label: Buildkite Pipelines API
  slug: buildkite-pipelines-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/buildkite/refs/heads/main/openapi/buildkite-pipelines-api-openapi.yml
- filename: buildkite-pipelinetemplates-api-openapi.yml
  format: yaml
  label: Buildkite PipelineTemplates API
  slug: buildkite-pipelinetemplates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/buildkite/refs/heads/main/openapi/buildkite-pipelinetemplates-api-openapi.yml
- filename: buildkite-queues-api-openapi.yml
  format: yaml
  label: Buildkite Queues API
  slug: buildkite-queues-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/buildkite/refs/heads/main/openapi/buildkite-queues-api-openapi.yml
- filename: buildkite-rules-api-openapi.yml
  format: yaml
  label: Buildkite Rules API
  slug: buildkite-rules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/buildkite/refs/heads/main/openapi/buildkite-rules-api-openapi.yml
- filename: buildkite-teams-api-openapi.yml
  format: yaml
  label: Buildkite Teams API
  slug: buildkite-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/buildkite/refs/heads/main/openapi/buildkite-teams-api-openapi.yml
- filename: buildkite-user-api-openapi.yml
  format: yaml
  label: Buildkite User API
  slug: buildkite-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/buildkite/refs/heads/main/openapi/buildkite-user-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Buildkite Authentication
name_suffix: Authentication
oauth_flows: []
overview: Buildkite secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Buildkite
provider_slug: buildkite
scheme_count: 1
schemes:
- description: Bearer token issued from your Buildkite Personal Access Tokens page.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/buildkite-openapi.yml
  type: http
slug: buildkite-authentication
source_filename: buildkite-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/buildkite-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Bearer token issued from your Buildkite Personal Access Tokens page.\n  sources:\n  - openapi/buildkite-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/buildkite/refs/heads/main/authentication/buildkite-authentication.yml
summary_line: http · 1 scheme
tags:
- DevOps
- CI/CD
- Pipelines
- Agents
- Self-Hosted
- GraphQL
- Test Engine
---
