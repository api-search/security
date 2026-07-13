---
api_key_in: []
api_specs:
- filename: graphite-dev-openapi.yml
  format: yaml
  label: Graphite GitHub App
  slug: graphite-github-app
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/graphite-dev/refs/heads/main/openapi/graphite-dev-openapi.yml
- filename: graphite-dev-openapi.yml
  format: yaml
  label: Graphite CLI (gt)
  slug: graphite-cli
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/graphite-dev/refs/heads/main/openapi/graphite-dev-openapi.yml
- filename: graphite-dev-openapi.yml
  format: yaml
  label: Graphite GT MCP Server
  slug: graphite-mcp
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/graphite-dev/refs/heads/main/openapi/graphite-dev-openapi.yml
- filename: graphite-dev-openapi.yml
  format: yaml
  label: Graphite Agent (Diamond) AI Code Review
  slug: graphite-agent-diamond
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/graphite-dev/refs/heads/main/openapi/graphite-dev-openapi.yml
- filename: graphite-dev-openapi.yml
  format: yaml
  label: Graphite Merge Queue
  slug: graphite-merge-queue
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/graphite-dev/refs/heads/main/openapi/graphite-dev-openapi.yml
- filename: graphite-dev-openapi.yml
  format: yaml
  label: Graphite Insights
  slug: graphite-insights
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/graphite-dev/refs/heads/main/openapi/graphite-dev-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Graphite Dev Authentication
name_suffix: Authentication
oauth_flows: []
overview: Graphite secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Graphite
provider_slug: graphite-dev
scheme_count: 1
schemes:
- description: Graphite auth token registered via `gt auth`, used by the CLI to act on the user's behalf.
  name: graphiteAuthToken
  scheme: bearer
  sources:
  - openapi/graphite-dev-openapi.yml
  type: http
slug: graphite-dev-authentication
source_filename: graphite-dev-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/graphite-dev-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: graphiteAuthToken\n  type: http\n  scheme: bearer\n  description: Graphite auth token registered via `gt auth`, used by the CLI to act on the user's\n    behalf.\n  sources:\n  - openapi/graphite-dev-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/graphite-dev/refs/heads/main/authentication/graphite-dev-authentication.yml
summary_line: http · 1 scheme
tags:
- Code Review
- Stacked PRs
- Merge Queue
- AI Code Review
- Developer Tools
- GitHub
---
